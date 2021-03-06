---
TOCTitle: 'MS10-APR'
Title: Microsoft Security Bulletin Summary für April 2010
ms:assetid: 'ms10-apr'
ms:contentKeyID: 61225079
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms10-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für April 2010
==================================================

Veröffentlicht: Dienstag, 13. April 2010 | Aktualisiert: Dienstag, 13. Juli 2010

**Version:** 4.0

In diesem Bulletin Summary sind die im April 2010 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für April 2010 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 8. April 2010 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 14. April 2010 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im April](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032427721&eventcategory=4&culture=en-us&countrycode=us). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://www.microsoft.com/germany/technet/sicherheit/bulletins/aktuell/default.mspx)

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
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx">MS10-019</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows können Remotecodeausführung ermöglichen (981210)</strong><br />
<br />
Dieses Update behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in der Windows Authenticode Verification, die Remotecodeausführung ermöglichen können. Ein Angreifer, dem es gelingt, eine dieser Sicherheitsanfälligkeiten auszunutzen, kann vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx">MS10-020</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SMB-Client können Remotecodeausführung ermöglichen (980232)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich und mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete SMB-Antwort auf eine vom Client initiierte SMB-Anforderung sendet. Um diese Sicherheitsanfälligkeiten auszunutzen, muss ein Angreifer den Benutzer dazu verleiten, eine SMB-Verbindung zu einem speziell gestalteten SMB-Server zu initiieren.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx">MS10-025</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Windows Media-Diensten kann Remotecodeausführung ermöglichen (980858)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Media-Diensten, die auf Microsoft Windows 2000 Server ausgeführt werden. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einem Microsoft Windows 2000 Server-System, auf dem Windows Media-Dienste ausgeführt werden, ein speziell gestaltetes Transportinformationspaket sendet. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen. Unter Microsoft Windows 2000 Server sind Windows Media-Dienste eine optionale Komponente und nicht standardmäßig installiert.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx">MS10-026</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft MPEG Layer-3-Codec kann Remotecodeausführung ermöglichen (977816)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft MPEG Layer-3-Audiocodecs. Die Sicherheitsanfälligkeit kann eine Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete AVI-Datei öffnet, die einen MPEG Layer-3-Audiostream enthält. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx">MS10-027</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Media Player kann Remotecodeausführung ermöglichen (979402)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Media Player. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn Windows Media Player speziell gestaltete Medieninhalte öffnet, die auf einer schädlichen Website gehostet werden. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx">MS10-021</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (979683)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx">MS10-022</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in VBScript kann Remotecodeausführung ermöglichen (981169)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in VBScript unter Microsoft Windows, die eine Remotecodeausführung ermöglichen kann. Dieses Sicherheitsupdate wird für Microsoft Windows 2000, Windows XP und Windows Server 2003 als Hoch eingestuft. Unter Windows Server 2008, Windows Vista, Windows 7 und Windows Server 2008 R2 kann der anfällige Code nicht ausgenutzt werden, aber da der Code vorhanden ist, wird dieses Update als Tiefenverteidigungsmaßnahme bereitgestellt und weist keine Bewertung des Schweregrads auf.<br />
<br />
Die Sicherheitsanfälligkeit kann eine Remotecodeausführung ermöglichen, wenn eine schädliche Website ein speziell gestaltetes Dialogfeld auf einer Webseite anzeigt und ein Benutzer die F1-Taste drückt, woraufhin das Windows-Hilfesystem mit einer vom Angreifer bereitgestellten Windows-Hilfedatei gestartet wird. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-023.mspx">MS10-023</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office Publisher kann Remotecodeausführung ermöglichen (981160)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office Publisher, die Remotecodeausführung ermöglichen kann, wenn ein Benutzer eine speziell gestaltete Publisher-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx">MS10-024</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Exchange und Windows SMTP-Dienst können Denial-of-Service ermöglichen (981832)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Exchange und Windows SMTP-Dienst. Die schwerwiegendere dieser Sicherheitsanfälligkeiten kann Denial-of-Service ermöglichen, wenn ein Angreifer einem Computer, auf dem der SMTP-Dienst ausgeführt wird, eine speziell gestaltete DNS-Antwort sendet. Standardmäßig ist die SMTP-Komponente auf Windows Server 2003, Windows Server 2003 x64 Edition und Windows XP Professional x64 Edition nicht installiert.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Exchange</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-028.mspx">MS10-028</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Visio können Remotecodeausführung ermöglichen (980094)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office Visio. Die Sicherheitsanfälligkeiten können eine Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Visio-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx">MS10-029</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in der Windows ISATAP-Komponente können Spoofing ermöglichen (978338)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Dieses Sicherheitsupdate wird für Windows XP, Windows Server 2003, Windows Vista und Windows Server 2008 als Mittel eingestuft. Windows 7 und Windows Server 2008 R2 sind nicht betroffen, weil diese Betriebssysteme die von diesem Sicherheitsupdate bereitgestellte Funktion bereits enthalten.<br />
<br />
Diese Sicherheitsanfälligkeit kann einem Angreifer ermöglichen, eine IPv4-Adresse vorzutäuschen, die Filtergeräte umgehen kann, die die IPv4-Quelladresse verwenden. Das Sicherheitsupdate behebt die Sicherheitsanfälligkeit, indem geändert wird, wie der Windows TCP/IP-Stapel die IPv6-Quelladresse in einem getunnelten ISATAP-Paket prüft.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Mittel</a><br />
Spoofing</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach absteigender Bewertung der Ausnutzbarkeit und dann CVE ID aufgeführt. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259.aspx).

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel der Sicherheitsanfälligkeit</th>
<th style="border:1px solid black;" >CVE-ID</th>
<th style="border:1px solid black;" >Ausnutzbarkeitsindex – Bewertung</th>
<th style="border:1px solid black;" >Wichtige Hinweise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx">MS10-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Windows-Kernel bezüglich Speicherzuordnung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0236">CVE-2010-0236</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx">MS10-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Windows-Kernel bezüglich Erstellung des symbolischen Links</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0237">CVE-2010-0237</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-028.mspx">MS10-028</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Visio bezüglich Speicherbeschädigung bei Attributüberprüfung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0254">CVE-2010-0254</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx">MS10-027</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Media Player bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0268">CVE-2010-0268</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx">MS10-025</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Media-Diensten durch stapelbasierten Pufferüberlauf</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0478">CVE-2010-0478</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-023.mspx">MS10-023</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Pufferüberlauf bei TextBox-Verarbeitung während Microsoft Office Publisher-Dateikonvertierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0479">CVE-2010-0479</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx">MS10-026</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MPEG Layer-3-Audiodecoder bezüglich Stapelüberlaufs</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0480">CVE-2010-0480</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx">MS10-022</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich VBScript und Drücken der Hilfetaste</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0483">CVE-2010-0483</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich<br />
<br />
Für Windows Server 2008, Windows 7 und Windows Server 2008 R2:<br />
<a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>3</strong></a> - Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet, wie in der <a href="https://www.microsoft.com/germany/technet/sicherheit/empfehlungen/981169.mspx">Microsoft-Sicherheitsempfehlung 981169</a> beschrieben.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-028.mspx">MS10-028</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Visio bezüglich Speicherbeschädigung bei Indexberechnung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0256">CVE-2010-0256</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx">MS10-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMB-Client bei Transaktionen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0270">CVE-2010-0270</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx">MS10-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMB-Client bezüglich Analyse von Antworten</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0476">CVE-2010-0476</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx">MS10-019</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in WinVerifyTrust bei Signaturüberprüfung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0486">CVE-2010-0486</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx">MS10-019</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Cabview bezüglich Beschädigung bei Überprüfung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0487">CVE-2010-0487</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx">MS10-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMB-Client bezüglich unvollständiger Antwort</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3676">CVE-2009-3676</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet, wie in der <a href="https://www.microsoft.com/germany/technet/sicherheit/empfehlungen/977544.mspx">Microsoft-Sicherheitsempfehlung 977544</a> beschrieben.<br />
<br />
Die wahrscheinliche Auswirkung ist Denial-of-Service.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx">MS10-024</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMTP-Server bezüglich MX-Eintrag</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0024">CVE-2010-0024</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Die wahrscheinliche Auswirkung ist Denial-of-Service</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx">MS10-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMB-Client bezüglich Speicherzuordnung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0269">CVE-2010-0269</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx">MS10-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMB-Client bezüglich Nachrichtengröße</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0477">CVE-2010-0477</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Die wahrscheinliche Auswirkung ist Denial-of-Service</td>
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-019**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-020**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-025**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-026**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-027**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-021**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-022**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-029**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx)
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
[Authenticode Signature Verification 5.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d7538166-35ee-4c6b-be8c-e83a1fc6cd77)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 5.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=13846177-f25f-4dd4-9fe9-ac43e1d4d73d)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=67ccac04-e5c8-4381-9d1a-9b676dd516a6)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4:](https://www.microsoft.com/technet/security/bulletin/%5Ehttps://www.microsoft.com/download/details.aspx?displaylang=de&familyid=73b3d681-26bb-49c1-849e-1f72484cb978)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f6394fc2-b9d0-46cf-9265-a0d4aeb1448f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Player 9-Reihe](https://www.microsoft.com/download/details.aspx?familyid=c0b8b362-a321-4ac9-be98-15c71bb7a043)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=c5f4577e-7546-40e9-8bcd-be11c1b260a6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[VBScript 5.1](https://www.microsoft.com/download/details.aspx?familyid=421be318-f217-4d12-b7a5-833093189073)<sup>[1]</sup>
(KB981350)  
(Hoch)  
[VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=421be318-f217-4d12-b7a5-833093189073)  
(KB981350)  
(Hoch)  
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=d5fc47a4-cecb-4817-aafb-45f335061be3)  
(KB981349)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=88a0e872-01de-495b-8eec-d105a970daa7)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-019**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-020**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-025**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-026**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-027**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-021**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-022**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-029**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx)
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
Keine
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 5.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2a01ddf0-f3ea-47c8-ada2-e69f6c1b5f96)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6c3ac102-2107-4726-98be-4fbf6b858bfb)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=dec38c02-3d4a-41c5-8954-e57f56b8fa5b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b1582a74-4a7b-4540-beb1-7c89c86eae87)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Player 9-Reihe unter Windows XP Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5c748c6d-84d1-45a9-8a33-9372eb5504d5)  
(Kritisch)  
[Windows Media Player 9-Reihe unter Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=9e4277b4-2dc5-4163-a6aa-7e07dd32b721)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=142710fd-9cd4-4dd0-aaba-2aace03c008f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=aa8ff157-a7b3-4787-80c9-5bc453f0f1c9) unter Windows XP Service Pack 2  
(KB981350)  
(Hoch)  
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=cb21d276-65e9-4c8f-96e3-cf6dc36d0133)  
(KB981349)  
(Hoch)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=ba7ef6e5-80ba-4281-a611-6e5be008c1b4)  
(KB981332)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=de447b76-ec89-426b-ac54-3ae3855d1159)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9dc3e1c2-2e9d-4d86-9fce-446c409ad613)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 5.1](https://www.microsoft.com/download/details.aspx?familyid=9bbff00c-f8f4-4a44-98f2-18a868986ae1)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?familyid=e64e487e-2727-4396-b0c9-6eaf000214d2)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c5a21239-a9a3-4ec5-9de8-7d2fc16fc6b8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-Codecs](https://www.microsoft.com/download/details.aspx?familyid=8afca317-a647-44aa-a771-5d85cd5d62ea)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3c0cb02e-3484-4cdf-8c64-c697ad3e2889)  
(Hoch)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=896c738d-4058-440f-8d4f-16c678610cd1)  
(KB981350)  
(Hoch)  
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=d7e8b930-8708-4f0b-b22b-961c2cbc2673)  
(KB981349)  
(Hoch)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=153fd9c1-0f8e-4492-87d1-f0381e7feb23)  
(KB981332)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4f9a696d-2712-4777-a642-e78a38336e8a)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d872bd77-f491-4706-8ff5-081ac0bf3d6f)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-019**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-020**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-025**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-026**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-027**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-021**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-022**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-029**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx)
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
Keine
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 5.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0e7e3deb-f078-4953-9642-675ec69267f2)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7ae9b1d0-0dbe-4abd-b315-10cea4ceccd7)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1189304f-d626-426d-960c-a86dc2d2b528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9f89746c-181e-4177-a851-ec1826e78b6d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0a7ea2d0-61ce-4b68-ad82-d917b1a56f9d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=28b035b8-d56e-4e93-b811-9a82cf1d4ba9)  
(KB981350)  
(Hoch)  
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=a142a553-85fc-40e0-9426-8d58f6a4333c)  
(KB981349)  
(Hoch)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=72754e1b-3d09-4b9d-8794-689c45a37f66)  
(KB981332)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f781e9e4-87d4-4243-9d44-256424d75fec)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=cd007a6c-04b3-490c-aff4-d5af3e69d477)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 5.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=99a3f6da-728f-421c-ab41-c4c4751934a4)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1709fd4e-d7c6-4cbb-8b71-a96b8d6eee58)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=52e4f66b-b76c-46a1-aeff-74efa21fc743)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b97e7ea1-a163-4ce4-8cbc-5f933773c4b2)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1fc66f54-260a-4219-a0b4-056ba9dd0abe)  
(Hoch)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=339ddf48-8949-4857-9ef6-1ddcc7c5f8b8)  
(KB981350)  
(Hoch)  
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=a489b4e3-78d2-411b-b27c-5987b8fc91d1)  
(KB981349)  
(Hoch)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=72c3013b-f72f-422b-8a89-2246dea4b378)  
(KB981332)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=644ff070-237b-4a73-b2e2-9fffdafa3927)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=19cfddfe-e8da-4564-9730-babfae4a3ebb)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 5.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=06832599-1e9b-4792-8c7b-7b5b3a3d6277)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=811a2b28-655d-4b5d-821e-5a90d556dba3)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=b2b6d8b1-63cc-459c-b5fa-1355386273c8)  
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
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=8dcb8be8-fb78-4518-aa7e-f8b17f7dfb86)  
(Hoch)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=9a8bee82-5f7f-490e-a1eb-481f6d4fc4f5)  
(KB981350)  
(Hoch)  
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=7d542ac6-8a5b-4dd7-8688-2b5feb563636)  
(KB981349)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=56c8238d-8b04-4aa5-8719-40550cd7325c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=916f1b09-e79e-4347-9fbc-c0cf07de397d)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-019**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-020**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-025**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-026**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-027**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-021**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-022**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-029**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx)
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
Keine
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a52225a7-6005-4f2b-8291-db20558f23f8)  
(KB978601  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6145e2b2-36fd-4360-bd5b-2bd11890fc52)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=25eeaeb3-c0a3-4a02-9912-acd0342648ba)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0e7140bb-42d3-48b3-9f4b-d55b17770de8)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista](https://www.microsoft.com/download/details.aspx?familyid=86d7b054-af4f-4d8a-9873-cb5246466374)  
(Hoch)  
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=86d7b054-af4f-4d8a-9873-cb5246466374)  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=ee5c42c6-16bb-48bf-95c2-c188bb17d04b)  
(KB981349)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=f2a37dbf-4a95-4e8d-a474-ecacd9aee690)  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=196055a6-15d1-4da8-b33d-501e69bf5176)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9ba7468c-23a4-4994-9a5a-22e96ef586f3)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5b7efa82-0feb-413a-9f8e-212e7432cd99)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=394c1caa-97e4-47a3-9aac-a4a88508bd31)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b885aef4-3a5d-4c3e-bef6-5efef2965752)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition](https://www.microsoft.com/download/details.aspx?familyid=7c84aa24-6331-427a-969c-27f7d39db3d7)  
(Hoch)  
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c84aa24-6331-427a-969c-27f7d39db3d7)  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=ea5c5e9c-0ecd-47bc-912d-5adc00d1aa21)  
(KB981349)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=79093796-4ea9-4c6c-92cc-3fd63c5db918)  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7c1d1622-1b67-438d-aae4-1a3954974a36)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-019**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-020**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-025**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-026**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-027**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-021**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-022**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-029**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx)
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=97ffeec8-8b6d-4a30-97b0-4bff2ba5e91d)\*  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f111735b-68b0-4bcc-9dd8-818a5eca3400)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=51c9c420-4507-4911-a8f5-82331a696882)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8e9c04c9-898f-4ed2-949d-f4343cc0d9f6)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=25e3ce7f-53a0-4049-a65c-011d2143c4c2)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=dbe89813-0a45-463b-928c-1e58f7bb596a)\*\*  
(KB981349)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=527d6376-efc9-436b-835b-219d38bb28f0)\*\*  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e29ead69-000a-4982-a25c-f3981eda381a)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=61ece7bc-e9fa-4ede-ba7d-9e5a4c64b9be)\*  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=49f9f740-023a-4291-becf-838a1d282321)\*  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=91c08251-0085-44cb-9e9c-9a1a84374caf)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=61c26a1f-c885-4474-9843-204c41628889)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 Codecs](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d6f2e1ae-48d3-4d2c-b329-32cff00afee5)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8b99e54d-955b-4a06-9a04-b2f4596efd72)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=9db62357-557d-40cd-9826-b7baa6c9de65)\*\*  
(KB981349)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=0c384dbc-21b7-4cbc-b68f-ced971d9b791)\*\*  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8f922e64-e3a6-46fe-9a81-b2813ea6a330)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72e7c7ea-55ef-457b-a03a-49aa9dea2e84)\*  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bd60779a-8bb1-4107-a344-9b09a50e96ff)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=eb116688-1d6e-4e20-948e-1d347af5d985)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=bcf8b919-08a9-487f-8dfd-3ca24328c4f3)  
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
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b1f9746d-61a2-406f-b707-60646bd5b5bb)  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=84c5aaae-9417-42a1-834f-22c1ad46a12f)  
(KB981349)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8c48302c-a1d6-41bc-ad24-7ce7332d4842)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-019**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-020**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-025**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-026**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-027**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-021**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-022**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-029**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx)
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
Keine
</td>
<td style="border:1px solid black;">
Keine
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
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8d4a6c65-e171-4570-8f3f-118f06910baf)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f0dbac52-0f0e-40bc-9371-17fa594424d5)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=389184c5-9001-497d-bdf4-81f97ecb617f)  
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
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=ff58d80c-33ce-4d9e-aaa5-0b1841458931)  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=c3f76835-0053-4e53-a451-14255e7a4fc0)  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
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
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=cf8c6721-05c2-4680-93b4-be36f09c6d15)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b23efe7d-bca4-4d49-9104-6ae39dc5daa9)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=f3495dae-71f3-421d-a191-d26965f26ad1)  
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
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=7f1dc055-2ec9-407a-9e69-da12338587e3)  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=998164b7-4b8c-468b-8d39-f242633c8838)  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-019**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-019.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-020**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-020.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-025**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-025.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-026**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-026.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-027**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-027.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-021**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-021.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-022**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-022.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-029**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-029.mspx)
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
Keine
</td>
<td style="border:1px solid black;">
Keine
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
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=94dfdaae-8464-4de6-a401-7eb70b3bb34f)\*  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a2979c02-2a80-4b84-bf6c-4798064bdf28)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=cd1a046e-915d-4904-b753-5a24be10c504)\*  
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
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=28389c1d-2a12-4bef-a59b-726bb6449c8b)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=c4039d40-a0c7-4183-ab50-04f690d1c5dc)\*\*  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=eb27cd2b-d514-4405-8650-259a42e35155)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Authenticode Signature Verification 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=40f622d2-48e7-4eb2-9430-bbd218cb5208)  
(KB978601)  
(Kritisch)  
[Shellerweiterung von Kabinettdatei-Viewer 6.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5e416d4b-5de7-4688-80c6-245de159e0ce)  
(KB979309)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=541e9e2f-ec1d-42b2-aae5-481c0d435169)  
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
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=d4ea3984-5183-47f1-814e-29cb6c90ae06)  
(Mittel)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=8174463c-5c5e-4095-90c8-fd1e898d4ba5)  
(KB981332)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den MSDN-Artikeln [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) und [Server Core für Windows Server 2008 R2](https://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den MSDN-Artikeln [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) und [Server Core für Windows Server 2008 R2](https://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweise für MS10-022**

<sup>[1]</sup>Dieses Sicherheitsupdate aktualisiert Ihre Installation von VBScript 5.1 auf VBScript 5.6.

<sup>[2]</sup>Bewertungen des Schweregrads treffen nicht auf dieses Update zu, da diese Software nicht von der Sicherheitsanfälligkeit betroffen ist, die in diesem Bulletin erörtert wird. Als Tiefenverteidigungsmaßnahme zum Schutz vor möglicherweise in der Zukunft entdeckten Sicherheitsanfälligkeiten empfiehlt Microsoft jedoch den Benutzern dieser Software, dieses Sicherheitsupdate zu installieren.

**Hinweis für MS10-024**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

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
[**MS10-023**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-023.mspx)
</td>
<td style="border:1px solid black;">
[**MS10-028**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-028.mspx)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=943b3830-70d5-46c5-bffc-1b494434b5f7)  
(KB980466)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2002 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2d563cbc-d8f7-486b-8c54-25d168085376)  
(KB979364)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=7c2f4610-77bb-4d72-847b-1a06c523b137)  
(KB980469)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=803a7ea0-a9da-46dd-9548-0177d3774be7)  
(KB979356)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2007 Service Pack 1 und Microsoft Office Publisher 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=10ca2f71-0ab2-4344-b7fd-bbbd6a783a96)  
(KB980470)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2007 Service Pack 1 und Microsoft Office Visio 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=56fe020f-4444-4a43-aa98-e99a622f6a69)  
(KB979365)  
(Hoch)
</td>
</tr>
</table>
 

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
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-024**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-024.mspx)
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
Microsoft Exchange Server 2000
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2000 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e47c90a0-c9c8-43b7-bec7-34107ddde294)  
(KB976703)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2003
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bc8391f8-5335-496b-ad4c-bae38509be4a)  
(KB976702)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2007 Service Pack 1 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6a894b4e-12b6-4a91-9555-d813956b6aac)  
(KB981407)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Microsoft Exchange Server 2007 Service Pack 2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b8f7f872-16d5-49d6-9867-adc01351c06f)  
(KB981383)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2010 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7dcf2390-dff7-4e3a-acca-03f4d43fb79a)  
(KB981401)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
</tr>
</table>
 
**Hinweise für MS10-024**

<sup>[1]</sup>Bewertungen des Schweregrads treffen nicht auf dieses Update zu, da diese Software nicht von der Sicherheitsanfälligkeit betroffen ist, die in diesem Bulletin erörtert wird. Microsoft empfiehlt Benutzern dieser Software jedoch, dieses Update zu installieren, das eine Tiefenverteidigungsmaßnahme beinhaltet, die DNS-Transaktionen, die vom SMTP-Dienst initiiert werden, zusätzliche Quellportentropie hinzufügt.

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

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](https://technet.microsoft.com/de-de/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch das Sicherheitsupdate-Inventurprogramm (SUIT) verwenden, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) verfügbar) installieren.

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

-   Mark Rabinovich von [Visuality Systems Ltd.](https://www.visualitynq.com/) für den Hinweis auf ein in MS10-020 beschriebenes Problem.
-   Laurent Gaffié von [stratsec](https://www.stratsec.net/) für den Hinweis auf drei in MS10-020 beschriebene Probleme.
-   Matthew „j00ru“ Jurczyk und Gynvael Coldwind von [Hispasec](https://www.hispasec.com/) [Virustotal](https://www.virustotal.com/) für den Hinweis auf fünf in MS10-021 beschriebene Probleme.
-   Tavis Ormandy von [Google Inc.](https://www.google.com/) für den Hinweis auf zwei in MS10-021 beschriebene Probleme.
-   Martin Tofall von [Obsidium Software](https://www.obsidium.de/) für den Hinweis auf ein in MS10-021 beschriebenes Problem.
-   Lionel d'Hauenens in Zusammenarbeit mit [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) für den Hinweis auf ein in MS10-023 beschriebenes Problem.
-   Fabien Perigaud von [CERT-LEXSI](https://cert.lexsi.com/) für den Hinweis auf ein in MS10-025 beschriebenes Problem.
-   Fabien Perigaud von [CERT-LEXSI](https://cert.lexsi.com/), [VUPEN Vulnerability Research Team](https://www.vupen.com/), Vulnerability Research Team, [TELUS Security Labs](https://telussecuritylabs.com/), [Core Security Technologies](https://www.coresecurity.com/) und [NSFOCUS Security Team](https://www.nsfocus.com/) für die Zusammenarbeit mit uns und für die Bereitstellung von Details zu einem Qualitätsproblem im ursprünglichen Sicherheitsupdate für MS10-025
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf ein in MS10-026 beschriebenes Problem.
-   Einer Person, die mit [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS10-027 beschriebenes Problem
-   Bing Liu von Fortinets [FortiGuard Labs](https://www.fortiguard.com/) für den Hinweis auf zwei in MS10-028 beschriebene Probleme.
-   Gabi Nakibly vom National EW Research & Simulation Center (bei Rafael) für den Hinweis auf ein in MS10-029 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (13. April 2010): Bulletin Summary veröffentlicht.
-   V1.1 (14. April 2010): Die Neustartanforderung für MS10-025 im Abschnitt **Kurzzusammenfassungen** wurde korrigiert. Es wurde ein Hinweis für die Server Core-Installationen von Windows Server 2008 und Windows Server 2008 R2 korrigiert, da er nur für das KB978601-Update für MS10-019 gilt.
-   V2.0 (21. April 2010): Das Bulletin Summary wurde überarbeitet, um Benutzer darüber zu informieren, dass das ursprüngliche Sicherheitsupdate für MS10-025 Systeme nicht vor der im Bulletin beschriebenen Sicherheitsanfälligkeit schützt. Microsoft empfiehlt, dass Benutzer eine der in MS10-025 beschriebenen Problemumgehungen anwenden, um die Auswirkungen auf betroffene Systeme zu verringern, bis ein überarbeitetes Sicherheitsupdate zur Verfügung gestellt wird.
-   V3.0 (27. April 2010): Überarbeitet, um das erneut veröffentlichte Sicherheitsupdate für MS10-025 anzubieten.
-   V4.0 (13. Juli 2010): Überarbeitet, um das erneut veröffentlichte Sicherheitsupdate für Windows Server 2008 und Windows Server 2008 R2 für MS10-024 anzubieten.

*Built at 2014-04-18T01:50:00Z-07:00*
