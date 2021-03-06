---
TOCTitle: 'MS09-OCT'
Title: Microsoft Security Bulletin Summary für Oktober 2009
ms:assetid: 'ms09-oct'
ms:contentKeyID: 61225077
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-oct(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Oktober 2009
====================================================

Veröffentlicht: Dienstag, 13. Oktober 2009 | Aktualisiert: Dienstag, 22. Juni 2010

**Version:** 4.2

In diesem Bulletin Summary sind die im Oktober 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Oktober 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 8. Oktober 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 14. Oktober 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im Oktober.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032407488&culture=en-us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://www.microsoft.com/germany/technet/sicherheit/bulletins/aktuell/default.mspx)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=163970">MS09-050</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SMBv2 können Remotecodeausführung ermöglichen (975517)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete und zwei vertraulich gemeldete Sicherheitsanfälligkeiten in SMBv2 (Server Message Block Version 2). Die schwerste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer ein speziell gestaltetes SMB-Paket an einen Computer sendet, der den Serverdienst ausführt. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=125438">MS09-051</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows Media Runtime können Remotecodeausführung ermöglichen (975682)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Windows Media Runtime. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Mediendatei öffnet oder speziell gestalteten Streaming-Inhalt von einer Website oder einer beliebigen Anwendung empfängt, die Webinhalte übermittelt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=163913">MS09-052</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Media Player kann Remotecodeausführung ermöglichen (974112)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Media Player. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn eine speziell gestaltete ASF-Datei mit Windows Media Player 6.4 wiedergegeben wird. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der lokale Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=163979">MS09-054</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (974455)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit in Internet Explorer. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, können diese Sicherheitsanfälligkeiten Remotecodeausführung ermöglichen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Firefox-Benutzer, die das Plug-In der Windows Presentation Foundation (WPF) ausführen und es nicht deaktiviert haben, sollten dieses Sicherheitsupdate ebenfalls installieren. Weitere Informationen zu diesem Problem finden Sie im Abschnitt „Häufig gestellte Fragen (FAQs)“ zur Sicherheitsanfälligkeit bei der Verarbeitung von HTML-Komponenten – CVE-2009-2529.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx">MS09-055</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate von ActiveX-Kill Bits (973525)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit, die mehrere ActiveX-Steuerelemente betrifft und derzeit ausgenutzt wird. Die Sicherheitsanfälligkeit wirkt sich auf ActiveX-Steuerelemente aus, die unter Verwendung der anfälligen Version der Microsoft Active Template Library (ATL) kompiliert wurden. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer in Internet Explorer eine speziell gestaltete Webseite anzeigt, die das ActiveX-Steuerelement instanziiert. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=160633">MS09-060</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in ActiveX-Steuerelementen der Microsoft Active Template Library (ATL) für Microsoft Office können Remotecodeausführung ermöglichen (973965)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in ActiveX-Steuerelementen für Microsoft Office, die mit einer anfälligen Version der Microsoft Active Template Library (ATL) kompiliert wurden. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Komponente oder ein Steuerelement lädt. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=160527">MS09-061</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft .NET Common Language Runtime können Remotecodeausführung ermöglichen (974378)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft .NET Framework und Microsoft Silverlight. Die Sicherheitsanfälligkeiten können Remotecodeausführung auf einem Clientsystem ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAPs) oder Silverlight-Anwendungen ausführen kann, oder wenn es einem Angreifer gelingt, einen Benutzer zu verleiten, eine speziell gestaltete .NET-Anwendung auszuführen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die Sicherheitsanfälligkeiten können auch Remotecodeausführung auf einem Serversystem ermöglichen, auf dem IIS ausgeführt wird, wenn jener Server die Verarbeitung von ASP.NET-Seiten zulässt und ein Angreifer erfolgreich eine speziell gestaltete ASP.NET-Seite auf den Server hochlädt und ausführt, wie es in einem Webhosting-Szenario der Fall sein kann. Microsoft .NET-Anwendungen, Silverlight-Anwendungen, XBAPs und ASP.NET-Seiten, die nicht schädlich sind, sind durch diese Sicherheitsanfälligkeit nicht gefährdet.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework,<br />
Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=161342">MS09-062</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows GDI+. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Bilddatei mithilfe betroffener Software anzeigt oder eine Website durchsucht, die speziell gestaltete Inhalte enthält. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer,<br />
Microsoft .NET Framework,<br />
Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft-Entwicklertools,<br />
Microsoft Forefront</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=164004">MS09-053</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im FTP-Dienst für Internetinformationsdienste können Remotecodeausführung ermöglichen (975254)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete Sicherheitsanfälligkeiten im FTP-Dienst in Microsoft Internet Information Services (IIS) 5.0, Microsoft Internet Information Services (IIS) 5.1, Microsoft Internet Information Services (IIS) 6.0 und Microsoft Internet Information Services (IIS) 7.0. Für IIS 7.0 ist nur der FTP-Dienst 6.0 betroffen. Die Sicherheitsanfälligkeiten können Remotecodeausführung (RCE) auf Systemen ermöglichen, auf denen der FTP-Dienst unter IIS 5.0 ausgeführt wird, oder Denial-of-Service (DoS) auf Systemen, auf denen der FTP-Dienst unter IIS 5.0, IIS 5.1, IIS 6.0 oder IIS 7.0 ausgeführt wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=163830">MS09-056</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows Crypto-API können Spoofing ermöglichen (974571)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Spoofing ermöglichen, wenn ein Angreifer Zugriff auf das Zertifikat erhält, das vom Endbenutzer zur Authentifizierung verwendet wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Spoofing</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=163832">MS09-057</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Indexdienst kann Remotecodeausführung ermöglichen (969059)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Remotecodeausführung ermöglichen, wenn ein Angreifer eine manipulierte Webseite einrichtet, die den Indexdienst durch einen Aufruf an dessen ActiveX-Komponente aufruft. Dieser Aufruf kann eine schädliche URL enthalten, durch die die Sicherheitsanfälligkeit ausgenutzt wird. Der Angreifer erhält mit den Berechtigungen des Benutzers, der die Webseite verwendet, Zugriff auf das Clientsystem. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=162442">MS09-058</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (971486)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten im Windows-Kernel. Die schwerste dieser Sicherheitsanfälligkeiten kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei dem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um eine dieser Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=163843">MS09-059</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Subsystemdienst für die lokale Sicherheitsautorität kann Denial-of-Service ermöglichen (975467)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer während des NTLM-Authentifizierungsprozesses ein speziell gestaltetes schädliches Paket sendet.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID geordnet.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259.aspx).
  
| Kennung des Bulletins                                                                   | Titel des Bulletins                                                                                                                                                    | CVE-ID                                                                           | Ausnutzbarkeitsindex – Bewertung                                                                                     | Wichtige Hinweise                                                                                                                                                                                                                                                                                                                                                                                                                        |  
|-----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-050](https://go.microsoft.com/fwlink/?linkid=163970)                               | Sicherheitsanfälligkeiten in SMBv2 können Remotecodeausführung ermöglichen (975517)                                                                                    | [CVE-2009-2526](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2526) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen eingeschränkten Denial-of-Service-Angriff.                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-050](https://go.microsoft.com/fwlink/?linkid=163970)                               | Sicherheitsanfälligkeiten in SMBv2 können Remotecodeausführung ermöglichen (975517)                                                                                    | [CVE-2009-2532](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2532) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-050](https://go.microsoft.com/fwlink/?linkid=163970)                               | Sicherheitsanfälligkeiten in SMBv2 können Remotecodeausführung ermöglichen (975517)                                                                                    | [CVE-2009-3103](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3103) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Es wurde Angreifercode wurde veröffentlicht.                                                                                                                                                                                                                                                                                                                                                                                             |  
| [MS09-051](https://go.microsoft.com/fwlink/?linkid=125438)                               | Sicherheitsanfälligkeiten in Windows Media Runtime können Remotecodeausführung ermöglichen (975682)                                                                    | [CVE-2009-0555](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0555) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-051](https://go.microsoft.com/fwlink/?linkid=125438)                               | Sicherheitsanfälligkeiten in Windows Media Runtime können Remotecodeausführung ermöglichen (975682)                                                                    | [CVE-2009-2525](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2525) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-052](https://go.microsoft.com/fwlink/?linkid=163913)                               | Sicherheitsanfälligkeit in Windows Media Player kann Remotecodeausführung ermöglichen (974112)                                                                         | [CVE-2009-2527](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2527) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-053](https://go.microsoft.com/fwlink/?linkid=164004)                               | Sicherheitsanfälligkeiten im FTP-Dienst für Internetinformationsdienste können Remotecodeausführung ermöglichen (975254)                                               | [CVE-2009-2521](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2521) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff. Es wurde Angreifercode wurde veröffentlicht.                                                                                                                                                                                                                                                                                                      |  
| [MS09-053](https://go.microsoft.com/fwlink/?linkid=164004)                               | Sicherheitsanfälligkeiten im FTP-Dienst für Internetinformationsdienste können Remotecodeausführung ermöglichen (975254)                                               | [CVE-2009-3023](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3023) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Es wurde Angreifercode wurde veröffentlicht.                                                                                                                                                                                                                                                                                                                                                                                             |  
| [MS09-054](https://go.microsoft.com/fwlink/?linkid=163979)                               | Kumulatives Sicherheitsupdate für Internet Explorer (974455)                                                                                                           | [CVE-2009-1547](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1547) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-054](https://go.microsoft.com/fwlink/?linkid=163979)                               | Kumulatives Sicherheitsupdate für Internet Explorer (974455)                                                                                                           | [CVE-2009-2529](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2529) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-054](https://go.microsoft.com/fwlink/?linkid=163979)                               | Kumulatives Sicherheitsupdate für Internet Explorer (974455)                                                                                                           | [CVE-2009-2530](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2530) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Auf Systemen mit Microsoft Windows 2000 wird der Ausnutzbarkeitsindex aufgrund des Mangels an Heapschutz auf [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) erhöht: Konsistenter Angreifercode wahrscheinlich.                                                                                                                                                                                                       |  
| [MS09-054](https://go.microsoft.com/fwlink/?linkid=163979)                               | Kumulatives Sicherheitsupdate für Internet Explorer (974455)                                                                                                           | [CVE-2009-2531](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2531) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     |                                                                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-055](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx) | Kumulatives Sicherheitsupdate von ActiveX-Kill Bits (973525)                                                                                                           | [CVE-2009-2493](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Keine                                                                                                                | (Diese Sicherheitsanfälligkeit wurde bereits im Ausnutzbarkeitsindex im [Bulletin Summary von Juli](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-jul.mspx) bewertet. Diese Sicherheitsanfälligkeit wurde erstmalig in [MS09-035](https://go.microsoft.com/fwlink/?linkid=158131) behoben.) Siehe die gleiche CVE-Nummer in [MS09-060](https://go.microsoft.com/fwlink/?linkid=160633).                               |  
| [MS09-056](https://go.microsoft.com/fwlink/?linkid=163830)                               | Sicherheitsanfälligkeiten in Windows Crypto-API können Spoofing ermöglichen (974571)                                                                                   | [CVE-2009-2510](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2510) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dies ist eine Sicherheitsanfälligkeit durch Spoofing.                                                                                                                                                                                                                                                                                                                                                                                    |  
| [MS09-056](https://go.microsoft.com/fwlink/?linkid=163830)                               | Sicherheitsanfälligkeiten in Windows Crypto-API können Spoofing ermöglichen (974571)                                                                                   | [CVE-2009-2511](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2511) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dies ist eine Sicherheitsanfälligkeit durch Spoofing.                                                                                                                                                                                                                                                                                                                                                                                    |  
| [MS09-057](https://go.microsoft.com/fwlink/?linkid=163832)                               | Sicherheitsanfälligkeit im Indexdienst kann Remotecodeausführung ermöglichen (969059)                                                                                  | [CVE-2009-2507](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2507) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-058](https://go.microsoft.com/fwlink/?linkid=162442)                               | Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (971486)                                                                    | [CVE-2009-2515](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2515) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-058](https://go.microsoft.com/fwlink/?linkid=162442)                               | Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (971486)                                                                    | [CVE-2009-2516](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2516) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Diese Sicherheitsanfälligkeit verursacht eine Denial-of-Service-Bedingung, wenn mit einer Netzwerkfreigabe darauf abgezielt wird, und eine Erhöhung von Berechtigungen, wenn sie lokal mit einem lokalen System als Ziel ausgenutzt wird.                                                                                                                                                                                                |  
| [MS09-058](https://go.microsoft.com/fwlink/?linkid=162442)                               | Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (971486)                                                                    | [CVE-2009-2517](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2517) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-059](https://go.microsoft.com/fwlink/?linkid=163843)                               | Sicherheitsanfälligkeit im Subsystemdienst für die lokale Sicherheitsautorität kann Denial-of-Service ermöglichen (975467)                                             | [CVE-2009-2524](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2524) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen eingeschränkten Denial-of-Service-Angriff.                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-060](https://go.microsoft.com/fwlink/?linkid=160633)                               | Sicherheitsanfälligkeiten in ActiveX-Steuerelementen der Microsoft Active Template Library (ATL) für Microsoft Office können Remotecodeausführung ermöglichen (973965) | [CVE-2009-0901](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0901) | Keine                                                                                                                | (Diese Sicherheitsanfälligkeit wurde bereits im Ausnutzbarkeitsindex im [Bulletin Summary von Juli](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-jul.mspx) bewertet. Diese Sicherheitsanfälligkeit wurde erstmalig in [MS09-035](https://go.microsoft.com/fwlink/?linkid=158131) behoben.)                                                                                                                          |  
| [MS09-060](https://go.microsoft.com/fwlink/?linkid=160633)                               | Sicherheitsanfälligkeiten in ActiveX-Steuerelementen der Microsoft Active Template Library (ATL) für Microsoft Office können Remotecodeausführung ermöglichen (973965) | [CVE-2009-2493](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Keine                                                                                                                | (Diese Sicherheitsanfälligkeit wurde bereits im Ausnutzbarkeitsindex im [Bulletin Summary von Juli](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-jul.mspx) bewertet. Diese Sicherheitsanfälligkeit wurde erstmalig in [MS09-035](https://go.microsoft.com/fwlink/?linkid=158131) behoben.) Siehe die gleiche CVE-Nummer in [MS09-055](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx). |  
| [MS09-060](https://go.microsoft.com/fwlink/?linkid=160633)                               | Sicherheitsanfälligkeiten in ActiveX-Steuerelementen der Microsoft Active Template Library (ATL) für Microsoft Office können Remotecodeausführung ermöglichen (973965) | [CVE-2009-2495](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2495) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.                                                                                                                                                                                                                                                                                                                                           |  
| [MS09-061](https://go.microsoft.com/fwlink/?linkid=160527)                               | Sicherheitsanfälligkeiten in Microsoft .NET Common Language Runtime können Remotecodeausführung ermöglichen (974378)                                                   | [CVE-2009-0090](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0090) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-061](https://go.microsoft.com/fwlink/?linkid=160527)                               | Sicherheitsanfälligkeiten in Microsoft .NET Common Language Runtime können Remotecodeausführung ermöglichen (974378)                                                   | [CVE-2009-0091](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0091) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-061](https://go.microsoft.com/fwlink/?linkid=160527)                               | Sicherheitsanfälligkeiten in Microsoft .NET Common Language Runtime können Remotecodeausführung ermöglichen (974378)                                                   | [CVE-2009-2497](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2497) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Das Potenzial für Angriffe mit Auswirkungen auf das Internet ist vorhanden.                                                                                                                                                                                                                                                                                                                                                              |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-2500](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2500) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-2501](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2501) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-2502](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2502) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-2503](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2503) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-2504](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2504) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-2518](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2518) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-2528](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2528) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-062](https://go.microsoft.com/fwlink/?linkid=161342)                               | Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (957488)                                                                                     | [CVE-2009-3126](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3126) | [**2**](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                                                                                                                                  |
  
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
</tr>
<tr>
<th colspan="13" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-050**](https://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](https://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](https://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](https://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx)
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](https://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](https://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](https://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](https://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](https://go.microsoft.com/fwlink/?linkid=163843)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Keine**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[DirectShow WMA Voice Codec](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8f850a82-61f9-447b-a0aa-a2c192cc5d2e)  
(KB954155)  
(Kritisch)  
[Audio Compression Manager](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6dfd5405-cabe-4bd7-9330-b6bde1d99194)  
(KB975025)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](https://www.microsoft.com/download/details.aspx?familyid=13035ef7-7e47-487c-8b7c-7795d33ce7de)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=26515c7b-d7a6-4405-96b5-a518dcb39d38)  
(Kritisch)  
[Microsoft Internet Explorer 6 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8154ba37-0fbc-4d31-9d6e-0b21586ad65a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=edfea805-9544-4dc0-a52c-d7594205657b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=f3fef608-dafb-4b37-a65a-9cc4ae8e2c4c)  
(KB958869)  
(Kritisch)  
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ecf78619-80fa-417d-852b-1b5b2cf574e2)  
(KB971108)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3e534aa8-29c2-4379-9f57-931a6ff47418)  
(KB971110)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e6f5e730-85cc-4c08-a50d-c456b1e9f5bc)  
(KB971111)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7fecd367-aaff-458b-91bc-8925c8e57528)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=52b9198d-b65f-467a-a5ab-141e23d64a86)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=b34d94b5-b828-4e16-a636-04344c60d945)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bdfa6583-28a2-4d6b-91d2-157a8518b664)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="13" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-050**](https://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](https://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](https://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](https://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx)
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](https://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](https://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](https://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](https://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](https://go.microsoft.com/fwlink/?linkid=163843)
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
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[DirectShow WMA Voice Codec](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4516c219-e357-485e-a52b-23dcb8ee49d8)  
(KB954155)  
(Kritisch)  
(Nur Windows XP Service Pack 2)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=746d3440-5a6a-421e-9286-7b534a1dfe54)  
(KB954155)  
(Kritisch)  
(Nur Windows XP Service Pack 3)  
[Audio Compression Manager](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6ecc7129-8caa-4daf-a8e2-8f3536225fb3)  
(KB975025)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](https://www.microsoft.com/download/details.aspx?familyid=b2efe1ac-d8d7-41bb-b87d-fc5e22afef0f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9aacf890-afb4-46a7-a13f-dd9fe3c0ca4a)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=dc166dc6-577f-4d8d-94df-dd963233dd85)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8799159d-df69-49f6-9db5-49147690ce0c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=171d43d3-669c-4923-b266-e47591833c05)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1bc56c26-1c7c-47e3-94f4-37af7e00392c)  
(KB953295)  
(Kritisch)  
(Nur Tablet PC Edition 2005 und Media Center Edition 2005)  
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e2acde20-a6d3-4135-b6eb-1214f743d474)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2ae0bdd4-f8b2-420a-b1ac-d2cdaa87c828)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=9c5ab624-e37b-418a-a919-d8f652b15679)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=768fd74e-0a2f-4353-ac22-65d0d6321739)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=cece4c55-0756-4357-9d2d-6709e8426068)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e997ea40-668e-40df-bd50-0ca53437b375)<sup>[1]</sup>
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[DirectShow WMA Voice Codec](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?familyid=4729de51-8fd8-46c6-b4ad-9c9f25202684)  
(KB954155)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) in Windows Media Format SDK 9.5 x64 Edition  
(KB954155)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?familyid=a866a490-6d3a-4ecd-acf4-770312ba2fd6) in Windows Media Format SDK 11  
(KB954155)  
(Kritisch)  
[Audio Compression Manager](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](https://www.microsoft.com/download/details.aspx?familyid=a9e7dfd8-7ba1-4f14-8e60-92ef00d91467)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=89a2cf2a-a7a2-4d4b-aa6f-24dde288d500)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=bd54e595-25f2-4839-a838-2a0f809bde2b)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=77b18fc2-e769-47c6-8e72-916716a49e58)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c08623bf-94bc-4c50-8c10-f50fb8448a0b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ad92503a-8c91-4d73-98b0-942d7961637d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=819dd2d1-cad5-4784-9baf-185d8a76df5d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ad29696d-4611-4a12-9dfa-74fa6866b759)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=270ec100-5ba1-4f8c-aa36-105d30ad57bf)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5459b7d4-1fab-4a04-ab9d-b8323505c1e2)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17008892-7950-44c4-850d-002c8d73495f)<sup>[1]</sup>
(Hoch)
</td>
</tr>
<tr>
<th colspan="13" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-050**](https://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](https://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](https://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](https://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx)
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](https://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](https://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](https://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](https://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](https://go.microsoft.com/fwlink/?linkid=163843)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[DirectShow WMA Voice Codec](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=00b3cb86-c9eb-4fbe-987e-2b0d94271d87)  
(KB954155)  
(Kritisch)  
[Audio Compression Manager](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ab1803ff-2371-487f-a7b6-95747c46ba4e)  
(KB975025)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](https://www.microsoft.com/download/details.aspx?familyid=5f82d01c-573e-425e-b9f2-86a54f377b19)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8101625d-ee93-46e5-aec2-3bdbf2d86472)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4647bcf1-69fb-4ad6-9e03-7bc22d8a914b)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9eae7eca-1a6f-4397-a6e2-7dda6b9d5276)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f3249c99-82e4-45dc-a254-28e647e822c8)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d1b4a58b-f0b1-4400-a6e6-0255b0513bd1) (KB953298)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=414466a4-39a0-476d-9a43-ae7674cbd6a0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=48256ea3-b433-4e84-9019-22300069cfc1)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=78072164-84d1-44da-8ede-2a9d212d47a9)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1e3f3842-f8fd-4969-a2cf-706db38d7580)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9dff4662-7771-4bdc-87ec-7899d79b3a55)<sup>[1]</sup>
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[DirectShow WMA Voice Codec](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=13ba4839-7fa9-4bbb-95f6-3fafb6c49f20)  
(KB954155)  
(Kritisch)  
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) in Windows Media Format SDK 9.5 x64 Edition  
(KB954155)  
(Kritisch)  
[Audio Compression Manager](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](https://www.microsoft.com/download/details.aspx?familyid=65e9036e-2e1b-40ff-a84b-c507107bcce8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2f966053-01eb-4a23-a9d5-71deac2498ea)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e7d77bd9-8317-42f3-9ad1-a0b8bfa65b53)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=708a549d-11fd-43bf-a6e1-309e3205d59d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1ad3f7b3-58d5-4507-ae20-a265e47cee9c)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eb95e8d9-6ef5-4526-99d2-507e50de049b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=61bded07-201e-4815-ac1e-468bf907e063)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8aa1f97d-ad53-4450-bb93-4a147dd10a87)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=95286b8d-4b53-4e6c-af59-e9e18fad3559)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8df7a2d9-2f97-4f18-84e8-415a1632cf09)<sup>[1]</sup>
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
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
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=79a1a94d-3b47-47e9-9476-2f591c3f6a59)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=07e66c09-2cd7-47ba-bf87-d3da602184b4)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=575e75d9-e348-4fbb-9eaa-43240e4d715e)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=a678ceb9-a37a-4c29-8bd1-f209922990e5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b99d4d9b-e0cc-4a8c-ad99-6a53958b37c8)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=2ede1eb9-7f5f-411d-bbc3-5db46d80e0bb)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=fb5678b9-5ef1-42db-902e-c9ea02880e0a)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=83c77015-7f96-4c0d-bd56-60aef90ea2f8)<sup>[1]</sup>
(Hoch)
</td>
</tr>
<tr>
<th colspan="13" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-050**](https://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](https://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](https://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](https://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx)
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](https://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](https://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](https://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](https://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](https://go.microsoft.com/fwlink/?linkid=163843)
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
Keine
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=29842c0c-8930-4b5f-83c6-1a718974b63f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f17ee0ea-f1e2-49f4-9f90-60296246ddfe)  
(KB954155)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f6995616-2a84-4c26-9599-26f1314873ed)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e8f6014f-950b-4e11-a105-51d298069f1a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7313c03b-8844-4086-a0cc-43dfdb3ca48c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=19aa01f3-026d-4264-85f8-216d0597969b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bb96eb1c-66a2-4276-9773-eea22179bcd4)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8b5a9a95-9439-40c8-acef-000b919daa04)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=04ae306b-0d0d-4767-ab54-cc11aec477ed)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Mittel)
</td>
<td style="border:1px solid black;">
Wie oben
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=62ed5d0a-5ca6-4942-80c9-7808b14cb6b5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=26905f12-92c7-4d45-99e7-227f03d2cb82)  
(KB954155)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b3de5236-afdd-436e-8648-5382d564cc99)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=85978f28-5fc0-481b-9b03-2021c785889b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7216bcb1-ff16-402b-ad1b-1500d46d0157)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=8f5f0c1d-1dd6-47fa-aef2-d3c96c8fc06e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bce096c8-833b-45c8-99cd-1280f0744f2f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4a60f789-1a4a-49a8-8d13-fda989ed40be)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=58c995ca-f308-4e07-8e60-2e542384d95d)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Mittel)
</td>
<td style="border:1px solid black;">
Wie oben
</td>
</tr>
<tr>
<th colspan="13" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-050**](https://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](https://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](https://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](https://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx)
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](https://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](https://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](https://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](https://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](https://go.microsoft.com/fwlink/?linkid=163843)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ff6bfcf3-76c9-4c45-b57d-22f94458dd6e)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2eaa9857-a147-4f31-9bf4-b9e2cf4c15c3)\*\*  
(KB954155)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72dd580e-eb53-41da-a5c0-a392ad388bfc)\*\*  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1baf7e96-ba3e-47e7-8ea3-eb092e653a39)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=51eb56fa-8204-45f3-86d7-6d03a2c8d78d)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=fd1694af-8873-43aa-9243-91f7cde452b7)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d9c5039f-d0cf-4d84-850f-f2f7701dcb79)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f9b487af-fe73-42a8-b240-d59c4321f95b)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=71aec6f6-a36b-465e-8885-b094dfd30423)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f2f617c2-f149-4e9b-bfdd-08ed0f3f99db)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=71aec6f6-a36b-465e-8885-b094dfd30423)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Wie oben
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=aff6f9c7-4a72-48f2-b750-204d796c7daa)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=70aabba3-53d6-4b52-be83-6d3f3869ecbd)\*\*  
(KB954155)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0111d741-bda4-4a50-a12b-d3337ff4441d)\*\*  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7a4b755b-7fa0-43aa-8862-c1d0c7d94c2c)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=131b047a-ae93-4a99-83e5-71d5a79e96ea)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=41bc4cdb-273a-4a6e-80d9-c8ce20e32da9)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=db969ddc-708e-42b7-9956-6c27bf346bbb)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0d8a2a3e-d7d4-47fb-8364-16fce28e4d38)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=deb84cb8-2ba3-47e3-9185-2bbc5b0a7e18)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Wie oben
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7b70108b-7f59-4898-ab4e-76be990de878)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e81f30b7-ef05-4488-b62a-d330e17129cf)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3d16c5bf-ee5c-4220-9755-5cb92eac2aae)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=30e5410d-0942-4964-9037-52330488efda)  
(KB974291)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)  
(KB974469)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=a4f42085-1cb9-4b8d-a931-85be71fdf06d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a221451a-cb4e-4a43-a225-4b1e86e87525)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8962f0b6-f346-4e88-9d83-4d15b699dd9d)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4aac0e3e-9b49-4a4a-ab17-707ff03b4d9b)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)  
(KB974470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Wie oben
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Mittel)
</td>
<td style="border:1px solid black;">
Wie oben
</td>
</tr>
<tr>
<th colspan="13" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-050**](https://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](https://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](https://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](https://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx)
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](https://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](https://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](https://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](https://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](https://go.microsoft.com/fwlink/?linkid=163843)
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
Windows 7 für 32-Bit-Systeme
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
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=89d1fb78-68cd-48dd-afc2-15a79ebe9fde)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b64bcc14-38a7-45b9-8f85-acc573777506)  
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
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=ad6f06d5-27db-445d-a8b2-c42adc90afc0)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=35b85783-90df-4f67-a3cb-02351432133e)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
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
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=10d9f7ac-65f4-437c-91cc-171632c69b0e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=809e29f3-ec68-4a2b-b04e-11759dd16001)  
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
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=70cd0270-77e9-492a-82d9-798364640c10)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=97010f2c-6c10-4fda-84fd-6c8749968db5)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="13" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-050**](https://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](https://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](https://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](https://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms09-055.mspx)
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](https://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](https://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](https://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](https://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](https://go.microsoft.com/fwlink/?linkid=163843)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows Server 2008 R2 für x64-basierte Systeme
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
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f50307d6-7869-4996-9ff7-23f87d08994b)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bcd2b944-6852-48f2-820b-cce7d195e391)\*\*  
(Niedrig)
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
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ce78c019-ec08-4ec6-abec-334f5ec5cb76)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=597ac3a7-e02d-49a5-9b8e-d097e867acea)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
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
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=9b6a28ae-b3f2-42b0-8209-e3950ec37abb)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=85e76e55-3766-4ffe-9a18-8655de935b7c)  
(Niedrig)
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
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=6442a77a-3c0d-4beb-b2d2-2885376c2135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=abc94857-37d8-4bb8-ad9e-46e687fca40e)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den MSDN-Artikeln [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) und [Server Core für Windows Server 2008 R2](https://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den MSDN-Artikeln [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) und [Server Core für Windows Server 2008 R2](https://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS09-061**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweise für MS09-062**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweis für MS09-059**

<sup>[1]</sup>Dieses Betriebssystem ist nur betroffen, wenn KB968389, „Erweiterter Authentifizierungsschutz“ (siehe [Microsoft-Sicherheitsempfehlung 973811](https://www.microsoft.com/germany/technet/sicherheit/empfehlungen/973811.mspx)) installiert wurde. Weitere Informationen finden Sie in dem entsprechenden Eintrag im Abschnitt „Häufig gestellte Fragen (FAQs) im Zusammenhang mit diesem Sicherheitsupdate“ in [MS09-059](https://go.microsoft.com/fwlink/?linkid=163843).

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
Microsoft Office Suites, Systeme und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-060**](https://go.microsoft.com/fwlink/?linkid=160633)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=04878c2c-eb97-426f-be08-89036a6799db)  
(KB973702)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=79e2b2e8-d5e8-4014-b489-720af2b5083d)  
(KB973705)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2007 Service Pack 1 und Microsoft Office Outlook 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d39234a3-c62c-44ba-a626-3179a183ca09)  
(KB972363)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office System 2007 Service Pack 1 und Microsoft Office System 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Andere Microsoft Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-060**](https://go.microsoft.com/fwlink/?linkid=160633)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=920ee70b-c5c1-47b5-8f33-938ffe14eea4)  
(KB975365)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Visio Viewer
</td>
<td style="border:1px solid black;">
Microsoft Visio 2002 Viewer<sup>[1]</sup>
(Kritisch)  
Microsoft Office Visio 2003 Viewer<sup>[1]</sup>
(Kritisch)  
[Microsoft Office Visio Viewer 2007 Service Pack 1 and Microsoft Office Visio Viewer 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d20004c5-dd01-459e-8120-5f127e20c085)  
(KB973709)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio Viewer 2007 Service Pack 1 and Microsoft Office Visio Viewer 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer, Microsoft Office Excel Viewer und Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Word Viewer 2003 Service Pack 3 und Microsoft Office Excel Viewer 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Hoch)  
[Microsoft Office Excel Viewer Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Hoch)  
[PowerPoint Viewer 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](https://www.microsoft.com/download/details.aspx?familyid=6f96de9a-62d8-428f-9567-51d55c129be6)  
(KB973636)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für MS09-060**

<sup>[1]</sup>Microsoft empfiehlt Benutzern von Microsoft Visio Viewer 2002 und Microsoft Visio Viewer 2003, auf Microsoft Office Visio Viewer 2007 Service Pack 2 zu aktualisieren.

**Hinweise für MS09-062**

<sup>[2]</sup>Diese Updates sind identisch.

<sup>[3]</sup>Diese Updates sind identisch.

\[4\]Diese Updates sind identisch.

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
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2000 Reporting Services Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
Nicht anwendbar  
QFE-Update:  
[SQL Server 2000 Reporting Services Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=33554f96-5af7-4683-a537-9db293b67b8d)  
(KB970899)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 x64 Edition Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 x64 Edition Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 für Itanium-basierte Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweis für MS09-062**

<sup>[1]</sup>Benutzer von SQL Server 2005 Service Pack 2, bei denen eine Reporting Services-Abhängigkeit zu SharePoint besteht, müssen außerdem das [Microsoft SQL Server 2005 Reporting Services Add-in für Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=%20f4d4d0ae-e5d4-4ed1-8d78-7137578161ce&displaylang=de) vom Microsoft Download Center installieren.

<sup>[2]</sup>Benutzer von SQL Server 2005 Service Pack 3, bei denen eine Reporting Services-Abhängigkeit zu SharePoint besteht, müssen außerdem das [Microsoft SQL Server 2005 Reporting Services Add-in für Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=%20648766ac-2a35-4238-a3f4-c26d7077f2a9&displaylang=de) vom Microsoft Download Center installieren.

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
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](https://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> bei Installation unter Mac  
(KB970363)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](https://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> bei Installation unter allen Versionen von Microsoft Windows-Clients  
(KB970363)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](https://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> bei Installation unter allen Versionen von Microsoft Windows-Servern\*\*  
(KB970363)  
(Mittel)
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
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
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
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=9e3b52d3-b211-4d62-891c-ae8f2e4ffc6c)  
(KB971022)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e186aeed-e9d7-4a02-84b3-bbed116ca060)  
(KB971023)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](https://www.microsoft.com/download/details.aspx?familyid=4fa10c93-ce20-43df-a725-ef4c77353747)  
(KB972221)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b904dee8-8a26-43f8-8ca9-86ad12cfdb52)  
(KB972222)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 Service Pack 1 unter Microsoft Windows 2000 Service Pack 4  
(KB971104)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e5d0d515-4b36-4025-bc6f-1c5cdf09e1af)  
bei Installation unter Microsoft Windows 2000 Service Pack 4  
(KB971104)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2 unter Microsoft Windows 2000 Service Pack 4  
(KB971105)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2a930f56-59ac-49a6-830f-bfae7c540ec7)  
bei Installation unter Microsoft Windows 2000 Service Pack 4  
(KB971105)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Report Viewer
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-061**](https://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package](https://www.microsoft.com/download/details.aspx?familyid=0dfaf300-2b53-4678-a779-0d805ddfe538)  
(KB971117)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Report Viewer 2008 Redistributable Package
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package](https://www.microsoft.com/download/details.aspx?familyid=42ed040f-cf94-4754-b0b3-c8016fbcbe22)  
(KB971118)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Report Viewer 2008 Redistributable Package Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6aaa74bd-a46e-4478-b4e1-2063d18d2d42)  
(KB971119)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Platform SDK Redistributable: GDI+
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Platform SDK Redistributable: GDI+](https://www.microsoft.com/download/details.aspx?familyid=6a63ab9c-df12-4d41-933c-be590feaa05a)  
(KB975337)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
</table>
 
**Hinweise für MS09-061**

<sup>[1]</sup>Dieser Download aktualisiert Microsoft Silverlight 2 auf Microsoft Silverlight 3, wodurch die im Bulletin beschriebene Sicherheitsanfälligkeit behoben wird.

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den MSDN-Artikeln [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) und [Server Core für Windows Server 2008 R2](https://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweise für MS09-062**

<sup>[2]</sup>Die Bewertungen des Schweregrads gelten nicht für dieses Update, da Microsoft keine Angriffsmethoden im Zusammenhang mit den in diesem Bulletin diskutierten Sicherheitsanfälligkeiten identifiziert hat, die spezifisch für diese Software wären. Dieses Sicherheitsupdate wird jedoch Entwicklern angeboten, die diese Software verwenden, um eine eigene aktualisierte Version ihrer Anwendungen zu veröffentlichen.

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
Microsoft Forefront Security
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-062**](https://go.microsoft.com/fwlink/?linkid=161342)
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
Microsoft Forefront Client Security 1.0
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Client Security 1.0](https://www.microsoft.com/download/details.aspx?familyid=c0ce624c-8df3-4223-8a7a-5cba4ac334a8)  
bei Installation unter Microsoft Windows 2000 Service Pack 4  
(KB975962)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS09-062**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) und [Windows Update](https://go.microsoft.com/fwlink/?linkid=21130) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Hinweis:** Am 1. August 2009 hat Microsoft den Support für Office Update und das Inventurprogramm für Office-Update eingestellt. Verwenden Sie [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747), um weiterhin die aktuellen Updates für Microsoft Office-Produkte zu erhalten. Weitere Informationen finden Sie in [Informationen zum Microsoft Office Update: Häufig gestellte Fragen (FAQs)](https://office.microsoft.com/de-de/downloads/fx010402221031.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 für Windows 2000 und neuere Betriebssysteme schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](https://technet.microsoft.com/de-de/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch das Sicherheitsupdate-Inventurprogramm (SUIT) verwenden, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/download/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) und im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Microsoft Application Compatibility Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   [Matthieu Suiche](https://www.msuiche.net/) vom [Netherlands Forensics Institute](https://www.nederlandsforensischinstituut.nl/) für den Hinweis auf ein in MS09-050 beschriebenes Problem.
-   Ivan Fratric von [Zero Day Initiative](https://www.zerodayinitiative.com/) und Jun Xie von [McAfee Avert Labs](https://www.avertlabs.com/) für den Hinweis auf ein in MS09-051 beschriebenes Problem.
-   Vinay Anantharaman von [Adobe Systems, Inc.](https://www.adobe.com/) für den Hinweis auf ein in MS09-051 beschriebenes Problem.
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf ein in MS09-052 beschriebenes Problem.
-   Skylined von [Google Inc.](https://www.google.com/) für den Hinweis auf ein in MS09-054 beschriebenes Problem.
-   Mark Dowd von [IBM ISS X-Force](https://www.iss.net/) für den Hinweis auf ein in MS09-054 beschriebenes Problem.
-   [TippingPoint](https://www.tippingpoint.com/) und die [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-054 beschriebenes Problem.
-   Sam Thomas von eshu.co.uk, der mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in MS09-054 beschriebenes Problem.
-   Ian Wright und Jean Luc Giraud von [Citrix](https://www.citrix.com/) für die Zusammenarbeit mit uns an einem in MS09-056 beschriebenen Problem.
-   Dan Kaminsky von [IOActive](https://www.ioactive.com/) für den Hinweis auf zwei in MS09-056 beschriebene Probleme.
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf ein in MS09-057 beschriebenes Problem.
-   Tavis Ormandy und Neel Mehta von [Google Inc.](https://www.google.com/) für den Hinweis auf zwei in MS09-058 beschriebene Probleme.
-   Das [NSFocus Security Team](https://www.nsfocus.com/) für den Hinweis auf ein in MS09-058 beschriebenes Problem.
-   David Dewey von [IBM ISS X-Force](https://www.iss.net/) für den Hinweis auf ein in MS09-060 beschriebenes Problem.
-   Ryan Smith von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf zwei in MS09-060 beschriebene Probleme.
-   [Pavel Minaev](https://int19h.org/) für den Hinweis auf ein in MS09-061 beschriebenes Problem.
-   Jeroen Frijters von [Sumatra](https://www.sumatra.nl/) für den Hinweis auf ein in MS09-061 beschriebenes Problem.
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf ein in MS09-062 beschriebenes Problem.
-   Thomas Garnier von [SkyRecon](https://www.skyrecon.com/) für den Hinweis auf ein in MS09-062 beschriebenes Problem.
-   Wushi von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS09-062 beschriebenes Problem.
-   Ivan Fratric von [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-062 beschriebenes Problem.
-   Tavis Ormandy von [Google Inc.](https://www.google.com/) für den Hinweis auf zwei in MS09-062 beschriebene Probleme.
-   Carlo Di Dato (alias shinnai) für den Hinweis auf ein in MS09-062 beschriebenes Problem.
-   Marsu Pilami von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS09-062 beschriebenes Problem.
-   Carsten H. Eiram von [Secunia](https://secunia.com/) für den Hinweis auf ein in MS09-062 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (13. Oktober 2009): Bulletin Summary veröffentlicht.
-   V1.1 (14. Oktober 2009): Der Downloadlink für Windows XP x64 Edition Service Pack 2 für MS09-055 wurde korrigiert.
-   V1.2 (18. Oktober 2009): Die Kurzzusammenfassung für MS09-054 wurde überarbeitet, um Anleitungen für Firefox-Benutzer bereitzustellen.
-   V2.0 (28. Oktober 2009): Microsoft Office Visio Viewer 2007, Microsoft Office Visio Viewer 2007 Service Pack 1 und Microsoft Office Visio Viewer 2007 Service Pack 2 wurden als betroffene Software für MS09-062 hinzugefügt, und für MS09-062 wurden Hinweise für Benutzer von SQL Server 2005 hinzugefügt, bei denen eine Reporting Services-Abhängigkeit zu SharePoint besteht.
-   V3.0 (2. November 2009): Das Bulletin wurde überarbeitet, um die Verfügbarkeit eines Hotfixes für MS09-054 anzukündigen, mit dem Anwendungskompatibilitätsprobleme behoben werden. Benutzer, die dieses Update bereits installiert haben, können den Hotfix aus Microsoft Knowledge Base-Artikel 976749 installieren.
-   V3.1 (4. November 2009): Fehlerhafte Verweise in MS09-060 and MS09-062 auf die ursprünglich veröffentlichte Version von Microsoft Office Visio Viewer 2007 als betroffene Software wurden entfernt.
-   V4.0 (10. November 2009): Das Bulletin wurde überarbeitet, um die erneute Veröffentlichung des Updates für Audio Compression Manager unter Microsoft Windows 2000 Service Pack 4 in MS09-051 zur Behebung eines Erkennungsproblems mitzuteilen. Dies ist lediglich eine Erkennungsänderung. Die Binärdateien wurden nicht verändert. Benutzer, die ihre Systeme erfolgreich aktualisiert haben, müssen dieses Update nicht erneut installieren.
-   V4.1 (12. Januar 2010): Microsoft Expression Web, Microsoft Expression Web 2, Microsoft Office Groove 2007 und Microsoft Office Groove 2007 Service Pack 1 wurden aus der betroffenen Software für MS09-062 entfernt.
-   V4.2 (22 Juni 2010): Das .NET Framework 1.1 Service Pack 1 wurde als eine betroffene Komponente von Windows 7 und Windows Server 2008 R2 für MS09-061 entfernt.

*Built at 2014-04-18T01:50:00Z-07:00*
