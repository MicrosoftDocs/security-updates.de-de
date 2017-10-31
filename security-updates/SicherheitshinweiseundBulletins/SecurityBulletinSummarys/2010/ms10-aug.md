---
TOCTitle: 'MS10-AUG'
Title: Microsoft Security Bulletin Summary für August 2010
ms:assetid: 'ms10-aug'
ms:contentKeyID: 61225080
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms10-aug(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für August 2010
===================================================

Veröffentlicht: Montag, 2. August 2010 | Aktualisiert: Mittwoch, 1. September 2010

**Version:** 2.1

In diesem Bulletin Summary sind die im August 2010 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für August 2010 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 5. August 2010 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 11. August 2010 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. Registrieren Sie sich jetzt für das [Security Bulletin-Webcast im August](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454431&eventcategory=4&culture=en-us&countrycode=us). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://www.microsoft.com/germany/technet/sicherheit/bulletins/aktuell/default.mspx)

Für das außerplanmäßige Security Bulletin, [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393), das erstmalig in Version 1.0 dieses Bulletin Summary angekündigt wurde, hat Microsoft eine entsprechende Bulletin Advance Notification am 30. Juli 2010 veröffentlicht und ein Bulletin-Webcast am 2. August 2010 gehostet. Dieser [Webcast vom 2. August 2010](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032456779&culture=en-us) ist auf Nachfrage erhältlich. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://www.microsoft.com/germany/technet/sicherheit/bulletins/aktuell/default.mspx)

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197393">MS10-046</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Shell kann Remotecodeausführung ermöglichen (2286198)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Windows Shell. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn das Symbol einer speziell gestalteten Verknüpfung angezeigt wird. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197104">MS10-049</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SChannel können Remotecodeausführung ermöglichen (980436)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und eine vertraulich gemeldete Sicherheitsanfälligkeit im SChannel-Sicherheitspaket (Secure Channel) in Windows. Die schwerwiegendere dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Website besucht, die entworfen wurde, um diese Sicherheitsanfälligkeiten über einen Internetwebbrowser auszunutzen. Ein Angreifer kann Endbenutzer jedoch nicht zum Besuch solcher Websites zwingen. Er muss den Benutzer zu einem Besuch dieser Webseite verleiten. Zu diesem Zweck wird der Benutzer normalerweise dazu gebracht, in einer E-Mail oder einer Instant Messenger-Anfrage auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196268">MS10-051</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft XML Core Services kann Remotecodeausführung ermöglichen (2079403)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft XML Core Services. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Ein Angreifer kann Benutzer nicht zum Besuch dieser Websites zwingen. Er muss den Benutzer zum Besuch dieser Website verleiten. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194432">MS10-052</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft MPEG Layer-3-Codecs kann Remotecodeausführung ermöglichen  (2115168)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft MPEG Layer-3-Audiocodecs. Diese Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Mediendatei öffnet oder speziell gestalteten Streaming-Inhalt von einer Website oder einer beliebigen Anwendung empfängt, die Webinhalte übermittelt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196549">MS10-053</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2183461)</strong><br />
<br />
Dieses Sicherheitsupdate behebt sechs vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190318">MS10-054</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SMB-Server können Remotecodeausführung ermöglichen (982214)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Angreifer ein speziell gestaltetes SMB-Paket erstellt und das Paket an ein betroffenes System sendet. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden, mit denen versucht wird, diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194906">MS10-055</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Cinepak Codec kann Remotecodeausführung ermöglichen (982665)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Cinepak Codec. Diese Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Mediendatei öffnet oder speziell gestalteten Streaming-Inhalt von einer Website oder einer beliebigen Anwendung empfängt, die Webinhalte übermittelt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196938">MS10-056</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (2269638)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete RTF-E-Mail-Nachricht öffnet oder in der Vorschau anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179830">MS10-060</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft .NET Common Language Runtime und in Microsoft Silverlight können Remotecodeausführung ermöglichen (2265906)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft .NET Framework und Microsoft Silverlight. Die Sicherheitsanfälligkeiten können auf einem Clientsystem Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAPs) oder Silverlight-Anwendungen ausführen kann, oder wenn es einem Angreifer gelingt, einen Benutzer dazu zu verleiten, eine speziell gestaltete Microsoft .NET-Anwendung auszuführen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die Sicherheitsanfälligkeiten können auch Remotecodeausführung auf einem Serversystem ermöglichen, auf dem IIS ausgeführt wird, wenn dieser Server die Verarbeitung von ASP.NET-Seiten zulässt und ein Angreifer erfolgreich eine speziell gestaltete ASP.NET-Seite auf den Server hochlädt und ausführt, wie es in einem Webhosting-Szenario der Fall sein kann.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework, Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=195812">MS10-047</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (981852)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194552">MS10-048</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Erhöhung von Berechtigungen ermöglichen (2160329)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete und vier vertraulich gemeldete Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern. Die schwerste dieser Sicherheitsanfälligkeiten kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei dem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197103">MS10-050</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Movie Maker kann Remotecodeausführung ermöglichen (981997)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Movie Maker. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete Movie Maker-Projektdatei sendet und den Benutzer dazu verleitet, die speziell gestaltete Datei zu öffnen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196275">MS10-057</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office Excel kann Remotecodeausführung ermöglichen (2269707)</strong> <br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der angemeldete Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194562">MS10-058</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in TCP/IP können Erhöhung von Berechtigungen ermöglichen (978886)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendere dieser Sicherheitsanfälligkeiten kann aufgrund eines Fehlers in der Verarbeitung eines bestimmten Eingabepuffers die Erhöhung von Berechtigungen ermöglichen. Ein Angreifer, der sich beim Zielsystem anmelden kann, kann diese Sicherheitsanfälligkeit ausnutzen und mit Berechtigungen auf Systemebene beliebigen Code ausführen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196444">MS10-059</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Feature „Ablaufverfolgung für Dienste“ können Erhöhung von Berechtigungen ermöglichen (982799)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und eine vertraulich gemeldete Sicherheitsanfälligkeit im Feature „Ablaufverfolgung für Dienste“. Die Sicherheitsanfälligkeiten können die Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach absteigender Bewertung der Ausnutzbarkeit und dann CVE ID aufgeführt. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259.aspx).
  
| Kennung des Bulletins                                     | Titel der Sicherheitsanfälligkeit                                                                                         | CVE-ID                                                                           | Ausnutzbarkeitsindex – Bewertung                                                                                     | Wichtige Hinweise                                                                                                                                                                                    |  
|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Sicherheitsanfälligkeit in Microsoft Silverlight bezüglich Speicherbeschädigung                                           | [CVE-2010-0019](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0019) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-052](http://go.microsoft.com/fwlink/?linkid=194432) | Sicherheitsanfälligkeit in MPEG Layer-3-Audiodecoder bezüglich Pufferüberlaufs                                            | [CVE-2010-1882](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1882) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | Sicherheitsanfälligkeit bei der Dateninitialisierung im Windows-Kernel                                                    | [CVE-2010-1888](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1888) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Sicherheitsanfälligkeit in Windows-Netzwerken bezüglich Ganzzahlüberlaufs                                                 | [CVE-2010-1893](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1893) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Sicherheitsanfälligkeit in Win32k bezüglich Ausnahmebehandlung                                                            | [CVE-2010-1894](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1894) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.**                                                                                                                                         |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Sicherheitsanfälligkeit in Win32k bezüglich Poolüberlaufs                                                                 | [CVE-2010-1895](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1895) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Sicherheitsanfälligkeit in Win32k bei Überprüfung der Benutzereingaben                                                    | [CVE-2010-1896](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1896) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Sicherheitsanfälligkeit in Win32k bei Fenstererstellung                                                                   | [CVE-2010-1897](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1897) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Sicherheitsanfälligkeit in Microsoft Silverlight und Microsoft .NET Framework CLR bezüglich Delegaten virtueller Methoden | [CVE-2010-1898](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1898) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Sicherheitsanfälligkeit in Word bei der Datensatzanalyse                                                                  | [CVE-2010-1900](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1900) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch RTF-Analysemodul in Word                                     | [CVE-2010-1901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1901) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-055](http://go.microsoft.com/fwlink/?linkid=194906) | Sicherheitsanfälligkeit in Cinepak Codec bezüglich Dekomprimierung                                                        | [CVE-2010-2553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2553) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-059](http://go.microsoft.com/fwlink/?linkid=196444) | Sicherheitsanfälligkeit in der Ablaufverfolgung bezüglich Speicherbeschädigung                                            | [CVE-2010-2555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2555) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung aufgrund von Nichtinitialisierung                                  | [CVE-2010-2557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2557) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | Es ist wahrscheinlicher, dass diese Sicherheitsanfälligkeit in Internet Explorer 6 ausgenutzt wird, und zwar aufgrund des Mangels der Datenausführungsverhinderung als schadensbegrenzende Maßnahme. |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung bei HTML-Layout                                                    | [CVE-2010-2560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2560) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-057](http://go.microsoft.com/fwlink/?linkid=196275) | Sicherheitsanfälligkeit in Excel bezüglich Speicherbeschädigung                                                           | [CVE-2010-2562](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2562) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-050](http://go.microsoft.com/fwlink/?linkid=197103) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Movie Maker                                                     | [CVE-2010-2564](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2564) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                              |  
| [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393) | Sicherheitsanfälligkeit durch Laden eines Verknüpfungssymbols                                                             | [CVE-2010-2568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2568) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**                                                                                                                   |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | „Double Free“-Sicherheitsanfälligkeit im Windows-Kernel                                                                   | [CVE-2010-1889](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1889) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | (Keine)                                                                                                                                                                                              |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Sicherheitsanfälligkeit durch Pufferüberlauf bei RTF-Analyse in Word                                                      | [CVE-2010-1902](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1902) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | Windows Vista und Windows 7 sind aufgrund zusätzlicher schadensbegrenzender Maßnahmen in Heaps weniger anfällig.                                                                                     |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung und verknüpfter HTML-Objekte in Word                               | [CVE-2010-1903](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1903) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | (Keine)                                                                                                                                                                                              |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Sicherheitsanfälligkeit durch Überlauf des SMB-Pools                                                                      | [CVE-2010-2550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2550) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | Eine Ausnutzung führt eher zu einem Denial-of-Service als zu einer Codesausführung.                                                                                                                  |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung aufgrund von Nichtinitialisierung                                  | [CVE-2010-2556](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2556) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | (Keine)                                                                                                                                                                                              |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung aufgrund einer Racebedingung                                       | [CVE-2010-2558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2558) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | (Keine)                                                                                                                                                                                              |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung aufgrund von Nichtinitialisierung                                  | [CVE-2010-2559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2559) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | (Keine)                                                                                                                                                                                              |  
| [MS10-051](http://go.microsoft.com/fwlink/?linkid=196268) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung bei der Bearbeitung von Antworten in Msxml2.XMLHTTP.3.0            | [CVE-2010-2561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2561) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | (Keine)                                                                                                                                                                                              |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Sicherheitsanfälligkeit in SChannel bezüglich Remotecodeausführung durch fehlerhafte Zertifikatanforderung                | [CVE-2010-2566](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2566) | [**2**  –](http://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich    | Ausnutzung führt wahrscheinlich zu einem Denial-of-Service. Remotecodeausführung unwahrscheinlich.                                                                                                   |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Sicherheitsanfälligkeit bei TLS/SSL-Neuverhandlung                                                                        | [CVE-2009-3555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3555) | [**3**](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dies ist eine Sicherheitsanfälligkeit durch Spoofing. Sie wurde in der [Microsoft-Sicherheitsempfehlung 977377](http://technet.microsoft.com/security/advisory/977377) beschrieben .                 |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Sicherheitsanfälligkeit bei domänenübergreifenden Ereignishandlern                                                        | [CVE-2010-1258](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1258) | [**3**](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.                                                                                                       |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Sicherheitsanfälligkeit in IPv6 bezüglich Speicherbeschädigung                                                            | [CVE-2010-1892](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1892) | [**3**](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.                                                                                                               |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Sicherheitsanfälligkeit bei Überprüfung der SMB-Variablen                                                                 | [CVE-2010-2551](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2551) | [**3**](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.                                                                                                               |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Sicherheitsanfälligkeit durch Auslastung des SMB-Stacks                                                                   | [CVE-2010-2552](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2552) | [**3**](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.                                                                                                               |
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=12361875-b453-45e8-852b-90f2727894fd)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ff00381c-e74b-48e5-9dd9-34dbedd906a2)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=dbdbbe5e-2ef9-4704-80c4-27ef28fd95ef)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=08159149-17de-4640-8818-cb7bd4811531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=bc949915-4e16-4897-a295-2f99102548ab)  
(Kritisch)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b489f8c-ada0-4051-8284-0a941c04d2ed)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1662780f-370a-425b-9917-c601eb54a375)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6e5e16f8-c140-4a1d-b898-8417a6bfd4d8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5ddb5e34-f97a-47c6-96c8-ba2ed06ccb77)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e3574047-5ce5-4461-94aa-4eb3258d5e71)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=deeac521-d3a2-4019-8176-c9228e733cf4)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b211664b-434d-4626-816f-c77510cfd44d)<sup>[1]</sup>
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
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?&amp;familyid=3b44bd67-48e2-497f-9165-42a702e2cc0d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaffa70c-6f2b-4e66-b1bc-64bdbbbcd34f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=4d4e8eeb-a0b2-41c6-9ee4-3f4beb44195e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b7f28d7a-6b27-4059-865b-5fd55edb6299)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=96b7a562-af16-4f0d-840c-838fb12e7419)  
(Kritisch)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5296fb82-c446-4681-a9a0-0f80a2e248be)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=f8ae3978-bad6-4201-8357-2d212ab703ef)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd6cc359-e72e-46ec-a08b-763934e3e115)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5cff5d6e-11a5-40ed-92ac-e12d287919e6)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6c5455e-bc31-4842-aef4-ebff92324323)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=decb1fe6-adc8-44f7-89c5-f25767f0cefe)<sup>[1]</sup>
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
<th colspan="14" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Keine
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=32fe91ef-5a8d-4095-90ee-2ca216696b09)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f76d68df-97e5-489c-a5f6-0c378c1f62ae)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=31ce233e-4d2d-404b-84a8-683319ba8ef7)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9c2110ec-7e6c-4e73-9785-0a8196095ea0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b0370e1e-dedf-4fe8-a06c-0e0f0a674205)  
(Kritisch)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8753ae27-60a4-475a-b8bc-6a7764480295)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=772e765d-0502-4b0b-bde8-d4f62b96db64)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=230e8559-e6df-49d5-acb5-b0cd4bde0bf4)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=59395f00-90f4-4b68-8dd3-03ff611c1bc8)  
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
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=923de214-c4fa-41e6-8307-2c5a37f13e8e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4543bcf0-3505-407b-a5a9-6250ece6fbac)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4d784b57-8564-4e7e-8f61-f897398e7ea5)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=fdfad4ca-37c4-4ac5-bebc-a5ad61299503)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d92f5e69-43cf-4615-aa3b-41f9f40bb57b)  
(Kritisch)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=fd3e9d06-1f8b-4ef7-84f6-61e85a1767b8)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=863edf45-0d3b-4408-a47c-258dc4a4fd94)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=03804f59-748e-4832-98e4-2d88564bd10a)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9ef1c600-bb93-4800-81b8-8c64b369c194)  
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
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=63aa5f8a-fe47-4892-b905-b54e4f3b6580)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9ef992c3-96e9-4533-b844-07424a6054b3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d87ac8b3-41fb-4cdd-b305-181a0024d85c)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=782e2963-4a52-4a1d-b99a-34ba841038a7)  
(Kritisch)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5e730064-8270-4d63-b497-c5ebeddea1fc)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e4f4f8b3-7a39-4d77-a46b-02c86ad159c3)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f96b8154-9976-41b0-b9d7-d79887fe9364)  
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
<th colspan="14" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=52748886-6280-4247-8cbd-f64db229ee66)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=aca69406-f795-4398-968f-959fe3a74e89)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=bbfaadf8-ab38-456c-956a-ea18c64236c9)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=535c563e-cdac-4e3d-96b0-9947ea22deca)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2062566b-8b81-43c2-875d-9c06d4e3fa82)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9087a3aa-aa55-41f6-8c4c-f322e4aa8681)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=60c81415-b61e-44a4-8dd9-cedec99eb70f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Kritisch)  
Nur Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Kritisch)  
Nur Windows Vista Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4486f97c-4cf8-4236-bfc3-b50e72e2a5c1)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c9345207-7242-4b71-bf80-b52031e08f8c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8aded9dd-08d6-4b19-955f-0d8414868cf9)<sup>[1]</sup>
(Hoch)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a1d8ed0d-a3b5-416a-ab8b-77501da62132)<sup>[2]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4684c4df-0a5c-4dba-82e5-059378737118)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=dfb31aa2-7457-4581-9e28-7984a360edf4)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=37648e95-05c2-4802-9a0f-660200baa229)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e2835ed1-5ca6-4347-8ff1-e694b1ac49ff)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=577131cd-1229-4746-89d7-84d75f29e1f0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=cd1185e3-ca22-4197-a53b-e7a2806ac352)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=65b04e29-8e39-46de-94e8-b653969b1ffd)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=10c9d5f1-53ed-459b-a663-e69bdb845a6b)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=469b732d-ca62-4a48-bb55-99f2ae4ddcf5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b547898e-f8a9-49dc-b49d-cffec5a001bc)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1620e7ac-3913-478d-8120-e9f46d98f453)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4baff9ae-dd25-4942-b45e-f281d0e1f4ac)<sup>[1]</sup>
(Hoch)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0a226592-8f98-4f67-ac60-1d00cbc56598)<sup>[2]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=18152cd4-815f-425f-8694-fbabcbe80609)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=110f932f-d13c-4486-a295-e6068d5d8d7a)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
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
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3aabd189-7d4c-4c9f-8854-f33127b1c309)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6e0253d4-f0c0-4f28-ba08-6907c2fcb339)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=73b5f45c-c9d6-491f-8483-98838b2a7c04)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8239cb9e-bb5a-4157-8038-33d0b329eaee)\*\*  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=409b9298-1e7d-48cf-9872-ffbdc56ebe53)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a94e2e38-116a-4b63-9328-6c33e63bbbfe)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für 32-Bit-Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=611765ab-b3f3-45db-92b2-ee040b9cfd27)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a8b1a3f7-7147-494e-bfc0-b1979b9578e6)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=844404be-f2e8-47bc-9650-9e2bbe383814)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4c9b3e60-e166-40c9-8938-3cba0a399c47)\*  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=29c6fc2d-d318-4a63-9ab2-82e84272aaf2)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a96891ff-8771-47b3-81bb-8640adb6c098)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=43ece408-4aa7-4819-b3f6-7f0719ed3213)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5ef8abf0-c89e-4911-8d77-42400d9a398f)\*\*  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9b869bab-0797-4f83-8c64-23dda9983c8d)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=602dd3f6-0d09-4546-b1db-d7b6b04edb66)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für x64-basierte Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=131f3512-1585-462e-a4f1-3f359aac44bd)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c1c25cb7-7e82-4c14-9666-aff52dd308b4)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=08491c73-66b1-4c4c-8740-ea596a730fc1)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=fa84e547-2190-402f-9467-2450deeff565)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=cfe227b5-6660-49f8-9d71-a997dd83de0b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3b16a422-0ee9-4eab-9cfe-e7688ffa0d76)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b6faee94-e821-432d-bfa2-9008664566af)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2f1eee63-2cca-4ec5-b196-36de3c0054cf)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=24d8f0a3-51a9-46c1-b870-a2239bf600e4)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für Itanium-basierte Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=972efd3a-ec1e-49b2-835e-76f4b21b5b79)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=45fe5135-aa89-4f60-8cdb-ec0edc9a7e77)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8aa12902-c234-4fd9-bba3-6767eafc38fc)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=84f89dca-108c-4956-9aa2-866e17a872fc)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=22e62b5c-e4c1-47d0-ae4a-8bd2d70d0a0a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=71716507-7080-4102-991e-6afc7cc377d5)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=31d0f5ac-2cff-42a1-8f18-128bbfc4e57d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ecaf42e0-a288-40c1-8602-21e967a87408)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8d58ebc4-a5f9-4318-a6f1-168c1bcdae3c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2e782ac9-b5d5-490e-a01a-7d4481eab224)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a7d60864-5942-47ed-a6f3-1c07b4833a14)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=68bddf4b-b597-477e-80e4-9293d7160496)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3a5a088e-644a-4a0e-9a09-0370bcd97688)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ce6233f3-2ee5-4329-908d-ba9b28ecc553)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9499f771-c388-4de3-a5c7-8cc8b00b4395)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c457d8ec-83b7-446f-b77c-e47d4187e616)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a4f6d7c2-b475-4900-82f0-75f5be0b7b63)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ca57a47a-9111-4abe-9356-4962ca2c1d65)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ad1ddf94-d714-4b36-8256-42bf79d03a90)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=24751193-592f-4c44-a8d6-f4112d4f011b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b00ec47c-402e-4207-a4c9-6c1900f254f8)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5ff09e03-d662-4b23-ab26-d25ca2ba58df)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=163fe2bd-f999-47c1-9a35-c4fc868bda51)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=146270fa-cd6f-440a-aa3e-e93af0bff447)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0d9dd09b-db40-462b-88b0-4dbb8180e81f)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c9aeea25-ca14-4b42-9018-a27c9d8899c4)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a48cdac5-4d78-49b5-a6d8-ecf6c58cace2)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e7757bbc-3ef0-421d-ab57-0083a302c77b)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=52642a8d-1081-4496-848e-9b03baf3fdac)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)\*  
(KB983590)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c1ad1248-07f1-42d4-baa4-8a20837ec7b4)\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6bbc9cb1-0b59-4473-adf9-2ce2f0f94c0a)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a1f95600-34e5-44b3-b2cb-b2b2cbf645cb)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=333fb6e4-f867-4dcb-beb3-2d88e428ca2e)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ce2bb5d4-f661-44e3-ac28-0b81f7b72670)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b7c2e91f-ca8a-4237-99c8-ca53c91cf73e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b4d3210e-f3ad-4dbb-9390-6e98eeb99eaa)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7b457d04-03a9-4eb0-ba6a-ab45267e4f74)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=783fb42c-3698-4b1d-a692-3ff319578931)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f23dec0f-a33b-4d8c-a86d-0e9368ae7ff5)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2543191a-09cb-4417-bbb2-aac4d9a2a756)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c3cd7f2f-e198-4fbd-a65d-21a1bf51eb61)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=62034ecb-a6bd-46c5-a03d-9642880bc2d6)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweise für MS10-050**

<sup>[1]</sup>Diese Versionen von Windows Movie Maker werden mit den angegebenen Betriebssystemen geliefert.

<sup>[2]</sup>Windows Movie Maker 2.6 ist ein optionaler Download, der unter den angegebenen Betriebssystemen installiert werden kann.

**Hinweis für MS10-060**

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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=978eb887-25b6-4dde-a2ec-d2d1e7f1a434)  
(KB2251389)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=032e1530-8736-4e1c-a704-967679227619)  
(KB2264397)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4360bcec-0731-4d4a-89eb-7d28a4607f06)  
(KB2251399)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7cecbce3-bbb7-47d1-bda3-64d7e0f69f62)  
(KB2264403)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0d7210a3-662e-41e7-affc-ae94f9d89388)<sup>[1]</sup>
(KB2251419)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Open XML-Dateiformatkonverter für Mac
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=39fe2229-9201-4270-bdc1-20bc8e30a766)  
(KB2251437)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ed5b9671-651d-41f3-aed3-93ee8a28657f)  
(KB2277947)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=feb121ad-e5f6-40e2-bf12-045ae5c2a754)  
(KB2092914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis für MS10-056**

<sup>[1]</sup>Für Microsoft Office Excel 2007 Service Pack 2 müssen Benutzer zusätzlich zum Sicherheitsupdatepaket KB2251419 auch das Sicherheitsupdate für Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2 (KB2277947) installieren, um vor den in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten geschützt zu sein.

#### Microsoft Entwicklertools und Software

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
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 2
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> bei Installation unter Mac  
(KB982926)  
(Kritisch)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> bei Installation unter allen Versionen von Microsoft Windows-Clients  
(KB982926)  
(Kritisch)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> bei Installation unter allen Versionen von Microsoft Windows-Servern\*\*  
(KB982926)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 3
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> bei Installation unter Mac OS  
(KB978464)  
(Kritisch)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> bei Installation unter allen Versionen von Microsoft Windows-Clients  
(KB978464)  
(Kritisch)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> bei Installation unter allen Versionen von Microsoft Windows-Servern\*\*  
(KB978464)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweise für MS10-060**

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

<sup>[1]</sup>Dieser Download aktualisiert Microsoft Silverlight 2 auf eine neuere Version, die nicht von den in dem Bulletin beschriebenen Sicherheitsanfälligkeiten betroffen ist.

<sup>[2]</sup>Dieses Update aktualisiert Microsoft Silverlight auf einen späteren Build, der nicht von den in dem Bulletin beschriebenen Sicherheitsanfälligkeiten nicht betroffen ist.

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) und [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Hinweis:** Am 1. August 2009 hat Microsoft den Support für Office Update und das Inventurprogramm für Office Update eingestellt. Verwenden Sie [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), um weiterhin die aktuellen Updates für Microsoft Office-Produkte zu erhalten. Weitere Informationen finden Sie in [Informationen zum Microsoft Office Update: Häufig gestellte Fragen (FAQs)](http://office.microsoft.com/de-de/downloads/fx010402221031.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](http://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Windows Server Update Services (WSUS) ermöglichen IT-Administratoren, die aktuellen Microsoft-Produktupdates für Computer bereitzustellen, die das Windows-Betriebssystem ausführen. Weitere Informationen zum Bereitstellen dieser Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie im TechNet-Artikel [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](http://technet.microsoft.com/de-de/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch das Sicherheitsupdate-Inventurprogramm (SUIT) verwenden, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](http://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=24da89e9-b581-47b0-b45e-492dd6da2971&amp;displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086/de).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Sergey I. Ulasen und Oleg Kupreev von [VirusBlokAda](http://www.anti-virus.by/) für den Hinweis auf ein in MS10-046 beschriebenes Problem.
-   Andreas Marx und Maik Morgenstern von [AV-Test](http://www.av-test.org/) für den Hinweis auf ein in MS10-046 beschriebenes Problem
-   Will Dormann von [CERT/CC](http://www.cert.org) für die Zusammenarbeit mit uns an einem in MS10-046 beschriebenen Problem
-   Niels Teusink für die Zusammenarbeit mit uns an einem in MS10-046 beschriebenen Problem
-   Stefan Kanthak für die Zusammenarbeit mit uns an einem in MS10-046 beschriebenen Problem
-   Tavis Ormandy von [Google Inc.](http://www.google.com/) für den Hinweis auf drei in MS10-047 beschriebene Probleme.
-   Tavis Ormandy von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS10-048 beschriebenes Problem.
-   Matthieu Suiche von [MoonSols](http://moonsols.com/) für den Hinweis auf zwei in MS10-048 beschriebene Probleme.
-   Matthieu Suiche von [MoonSols](http://moonsols.com/) für die Zusammenarbeit mit uns an den in MS10-048 behobenen Tiefenverteidigungsänderungen.
-   Nicolás Economou von [Core Security Technologies](http://www.coresecurity.com/) für den Hinweis auf ein in MS10-048 beschriebenes Problem.
-   Marsh Ray und Steve Dispensa von [PhoneFactor](http://www.phonefactor.com/) für den Hinweis auf ein in MS10-049 beschriebenes Problem.
-   Dyon Balding von [Secunia](http://secunia.com/) für den Hinweis auf ein in MS10-050 beschriebenes Problem.
-   Skylined von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS10-051 beschriebenes Problem.
-   Moritz Jodeit von der n.runs AG, der mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) von [TippingPoint](http://www.tippingpoint.com/) zusammenarbeitet, für den Hinweis auf ein in MS10-052 beschriebenes Problem.
-   David Bloom von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS10-053 beschriebenes Problem.
-   Nicolas Joly vom [VUPEN Vulnerability Research Team](http://www.vupen.com) für den Hinweis auf vier in MS10-053 beschriebene Probleme.
-   Gambino ZaDarkSide für den Hinweis auf ein in MS10-053 beschriebenes Problem.
-   Laurent Gaffié von [stratsec](http://www.stratsec.net/) für den Hinweis auf ein in MS10-054 beschriebenes Problem.
-   Todd Wease und Richard Johnson von [Sourcefire VRT](http://www.sourcefire.com/services/sf_vrt.html) für den Hinweis auf ein in MS10-054 beschriebenes Problem.
-   Riku Hietamaki und Joshua Morin von [Codenomicon](http://www.codenomicon.com/) für den Hinweis auf ein in MS10-054 beschriebenes Problem.
-   Einer Person, die mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) von [TippingPoint](http://www.tippingpoint.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS10-055 beschriebenes Problem
-   L. W. Z von [team509](http://www.team509.com/), in Zusammenarbeit mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) von [TippingPoint](http://www.tippingpoint.com/), für den Hinweis auf ein in MS10-056 beschriebenes Problem.
-   Wushi von [team509](http://www.team509.com/) in Zusammenarbeit mit [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS10-056 beschriebenes Problem.
-   [team509](http://www.team509.com/) in Zusammenarbeit mit [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS10-056 beschriebenes Problem.
-   Rodrigo Rubira Branco vom [Check Point](http://www.checkpoint.com/) IPS Research Team für den Hinweis auf ein in MS10-056 beschriebenes Problem.
-   Einer Person, die mit [Zero Day Initiative](http://www.zerodayinitiative.com/) von [TippingPoint](http://www.tippingpoint.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS10-056 beschriebenes Problem.
-   Damián Frizza von [Core Security Technologies](http://www.coresecurity.com/) für den Hinweis auf ein in MS10-057 beschriebenes Problem.
-   Darren Willis vom [Fourteenforty Research Institute, Inc.](http://www.fourteenforty.jp/) für den Hinweis auf ein in MS10-058 beschriebenes Problem.
-   Matthieu Suiche von [MoonSols](http://moonsols.com/) für den Hinweis auf ein in MS10-058 beschriebenes Problem.
-   Cesar Cerrudo [des Argeniss](http://www.argeniss.com/) für die Zusammenarbeit mit uns an zwei in MS10-059 beschriebenen Problemen.
-   Carsten Book von der für den Hinweis auf ein in MS10-060 beschriebenes Problem.
-   [Eamon Nerbonne](http://eamon.nerbonne.org/) für den Hinweis auf ein in MS10-060 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](http://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (2. August 2010): Bulletin Summary veröffentlicht.
-   V2.0 (10. August 2010): Die Bulletins MS10-047 bis MS10-060 wurden hinzugefügt.
-   V2.1 (1. September 2010): MS10-056 wurde ein Hinweis hinzugefügt, um Benutzer von Word 2007 zu informieren, dass sie zusätzlich zum Sicherheitsupdatepaket KB2251419 auch das Sicherheitsupdatepaket KB2277947 installieren müssen.

*Built at 2014-04-18T01:50:00Z-07:00*
