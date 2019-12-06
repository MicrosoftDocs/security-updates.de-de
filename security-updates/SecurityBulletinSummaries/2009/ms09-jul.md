---
TOCTitle: 'MS09-JUL'
Title: Microsoft Security Bulletin Summary für Juli 2009
ms:assetid: 'ms09-jul'
ms:contentKeyID: 61225072
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-jul(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Juli 2009
=================================================

Veröffentlicht: Dienstag, 14. Juli 2009 | Aktualisiert: Dienstag, 9. März 2010

**Version:** 8.0

In diesem Bulletin Summary sind die im Juli 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Juli 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 9. Juli 2009 veröffentlicht wurde, und die außerplanmäßige Bulletin Advance Notification, die erstmalig am 24. Juli 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 15. Juli 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu den regulär geplanten Bulletins zu beantworten. Dieser Webcast ist jetzt auf Anfrage verfügbar. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://www.microsoft.com/germany/technet/sicherheit/bulletins/aktuell/default.mspx)

Für die außerplanmäßigen Security Bulletins, MS09-034 und MS09-035, die zur Version 2.0 dieses Bulletin Summary hinzugefügt wurden, stellt Microsoft zwei Webcasts bereit, um Kundenfragen zu diesen Bulletins zu beantworten: am 28. Juli 2009 um 13:00 Uhr pazifische Zeit (USA & Kanada) und um 16:00 Uhr pazifische Zeit (USA & Kanada). Registrieren Sie sich jetzt für den [Webcast am 28. Juli um 13:00 Uhr](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032422339&culture=en-us) und den [Webcast am 28. Juli um 16:00 Uhr](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032422341&culture=en-us). Später sind diese Webcasts auf Anfrage verfügbar. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://www.microsoft.com/germany/technet/sicherheit/bulletins/aktuell/default.mspx)

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139788">MS09-029</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Embedded OpenType-Schriftartmodul können Remotecodeausführung ermöglichen (961371)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in der Microsoft Windows-Komponente des Embedded OpenType (EOT)-Schriftartmoduls. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen. Ein Angreifer, dem es gelingt, eine dieser Sicherheitsanfälligkeiten auszunutzen, kann von einem Remotestandort aus vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=152887">MS09-028</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft DirectShow kann Remotecodeausführung ermöglichen (971633)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft DirectShow. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete QuickTime-Mediendatei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=157386">MS09-032</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate von ActiveX-Kill Bits (973346)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit, die derzeit ausgenutzt wird. Die Sicherheitsanfälligkeit in Microsoft Video-ActiveX-Steuerelement kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt und das ActiveX-Steuerelement instanziiert. Dieses Steuerelement sollte nie in Internet Explorer instanziiert werden. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=158199">MS09-034</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (972260)</strong><br />
<br />
Dieses Sicherheitsupdate wird außerplanmäßig und in Verbindung mit dem Microsoft Security Bulletin MS09-035 veröffentlicht, in dem Sicherheitsanfälligkeiten in Komponenten und Steuerelementen beschrieben werden, die unter Verwendung anfälliger Versionen der Microsoft Active Template Library (ATL) entwickelt wurden. Dieses Sicherheitsupdate für Internet Explorer ist eine Tiefenverteidigungsmaßnahme und hilft als solche, bekannte Angriffsmethoden in Internet Explorer im Zusammenhang mit denjenigen Komponenten und Steuerelementen abzuschwächen, die mit anfälligen Versionen von ATL entwickelt wurden, wie in der Microsoft-Sicherheitsempfehlung (973882) und im Microsoft Security Bulletin MS09-035 beschrieben.<br />
<br />
Dieses Sicherheitsupdate behebt auch drei vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, können diese Sicherheitsanfälligkeiten Remotecodeausführung ermöglichen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=153891">MS09-033</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Virtual PC und Virtual Server kann Erhöhung von Berechtigungen ermöglichen (969856)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Virtual PC und Microsoft Virtual Server. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code ausführen und vollständige Kontrolle über ein betroffenes Gastsystem erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Virtual PC, Virtual Server</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=154993">MS09-031</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft ISA Server 2006 kann Erhöhung von Berechtigungen verursachen (970953)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Internet Security and Acceleration (ISA) Server 2006. Die Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer erfolgreich ein Benutzerkonto mit Administratorberechtigungen für einen ISA Server nachahmt, das für Radius-Einmalkennwort-Authentifizierung und Authentifizierungsdelegierung mit eingeschränkter Kerberos-Delegierung konfiguriert ist.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft ISA Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147424">MS09-030</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office Publisher kann Remotecodeausführung ermöglichen (969516)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office Publisher, die Remotecodeausführung ermöglichen kann, wenn ein Benutzer eine speziell gestaltete Publisher-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=158131">MS09-035</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in der Visual Studio Active Template Library können Remotecodeausführung ermöglichen (969706)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in den öffentlichen Versionen der Microsoft Active Template Library (ATL), die in Visual Studio enthalten sind. Dieses Sicherheitsupdate ist speziell für Entwickler von Komponenten und Steuerelementen vorgesehen. Entwickler, die mit ATL Komponenten und Steuerelemente erstellen und weiterverteilen, sollten das in diesem Bulletin bereitgestellte Update installieren und der bereitgestellten Anleitung folgen, um Komponenten und Steuerelemente, die nicht anfällig für die in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten sind, zu erstellen und an ihre Kunden zu verteilen.<br />
<br />
Dieses Security Bulletin beschreibt Sicherheitsanfälligkeiten, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine Komponente oder ein Steuerelement heruntergeladen hat, die mit den anfälligen Versionen der ATL erstellt wurden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Mittel</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Visual Studio</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID geordnet.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259.aspx).
  
| Kennung des Bulletins                                     | Titel des Bulletins                                                                                                     | CVE-ID                                                                           | Ausnutzbarkeitsindex - Bewertung                                                                                     | Wichtige Hinweise                                                                   |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|  
| [MS09-028](http://go.microsoft.com/fwlink/?linkid=152887) | Sicherheitsanfälligkeit in Microsoft DirectShow kann Remotecodeausführung ermöglichen (971633)                          | [CVE-2009-1537](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1537) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**  |  
| [MS09-028](http://go.microsoft.com/fwlink/?linkid=152887) | Sicherheitsanfälligkeit in Microsoft DirectShow kann Remotecodeausführung ermöglichen (971633)                          | [CVE-2009-1538](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1538) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                             |  
| [MS09-028](http://go.microsoft.com/fwlink/?linkid=152887) | Sicherheitsanfälligkeit in Microsoft DirectShow kann Remotecodeausführung ermöglichen (971633)                          | [CVE-2009-1539](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1539) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                             |  
| [MS09-029](http://go.microsoft.com/fwlink/?linkid=139788) | Sicherheitsanfälligkeiten im Embedded OpenType-Schriftartmodul können Remotecodeausführung ermöglichen (961371)         | [CVE-2009-0231](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0231) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                             |  
| [MS09-029](http://go.microsoft.com/fwlink/?linkid=139788) | Sicherheitsanfälligkeiten im Embedded OpenType-Schriftartmodul können Remotecodeausführung ermöglichen (961371)         | [CVE-2009-0232](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0232) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                             |  
| [MS09-030](http://go.microsoft.com/fwlink/?linkid=147424) | Sicherheitsanfälligkeit in Microsoft Office Publisher kann Remotecodeausführung ermöglichen (969516)                    | [CVE-2009-0566](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0566) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                             |  
| [MS09-031](http://go.microsoft.com/fwlink/?linkid=154993) | Sicherheitsanfälligkeit in Microsoft ISA Server 2006 kann Erhöhung von Berechtigungen verursachen (970953)              | [CVE-2009-1135](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1135) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                             |  
| [MS09-032](http://go.microsoft.com/fwlink/?linkid=157386) | Kumulatives Sicherheitsupdate von ActiveX-Kill Bits (973346)                                                            | [CVE-2008-0015](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-0015) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**  |  
| [MS09-033](http://go.microsoft.com/fwlink/?linkid=153891) | Sicherheitsanfälligkeit in Virtual PC und Virtual Server kann Erhöhung von Berechtigungen ermöglichen (969856)          | [CVE-2009-1542](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1542) | [**2**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Inkonsistenter Angreifercode wahrscheinlich     | Funktionale Codeausführung ist mit inkonsistenten Ausnutzungsergebnissen möglich.   |  
| [MS09-034](http://go.microsoft.com/fwlink/?linkid=158199) | Kumulatives Sicherheitsupdate für Internet Explorer (972260)                                                            | [CVE-2009-1917](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1917) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | Funktionale Codeausführung ist einfach und zuverlässig.                             |  
| [MS09-034](http://go.microsoft.com/fwlink/?linkid=158199) | Kumulatives Sicherheitsupdate für Internet Explorer (972260)                                                            | [CVE-2009-1918](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1918) | [**2**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Inkonsistenter Angreifercode wahrscheinlich     | Funktionale Codeausführung ist mit inkonsistenten Ausnutzungsergebnissen möglich.   |  
| [MS09-034](http://go.microsoft.com/fwlink/?linkid=158199) | Kumulatives Sicherheitsupdate für Internet Explorer (972260)                                                            | [CVE-2009-1919](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1919) | [**2**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Inkonsistenter Angreifercode wahrscheinlich     | Funktionale Codeausführung ist mit inkonsistenten Ausnutzungsergebnissen möglich.   |  
| [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) | Sicherheitsanfälligkeiten in der Visual Studio Active Template Library können Remotecodeausführung ermöglichen (969706) | [CVE-2009-0901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0901) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | Funktionale Codeausführung ist einfach und zuverlässig.                             |  
| [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) | Sicherheitsanfälligkeiten in der Visual Studio Active Template Library können Remotecodeausführung ermöglichen (969706) | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | [**1**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | Funktionale Codeausführung ist einfach und zuverlässig.                             |  
| [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) | Sicherheitsanfälligkeiten in der Visual Studio Active Template Library können Remotecodeausführung ermöglichen (969706) | [CVE-2009-2495](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2495) | [**3**](http://technet.microsoft.com/de-de/security/cc998259.aspx) - Funktionierender Angreifercode unwahrscheinlich | Fehler durch Offenlegung von Informationen nur ohne Bedrohung durch Codeausführung. |
  
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
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-029**](http://go.microsoft.com/fwlink/?linkid=139788)
</td>
<td style="border:1px solid black;">
[**MS09-028**](http://go.microsoft.com/fwlink/?linkid=152887)
</td>
<td style="border:1px solid black;">
[**MS09-032**](http://go.microsoft.com/fwlink/?linkid=157386)
</td>
<td style="border:1px solid black;">
[**MS09-034**](http://go.microsoft.com/fwlink/?linkid=158199)
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
Keine
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1efbbd95-cd72-43df-b1ce-7e2b0c0cb9e2)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 7.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e3e54348-6548-4162-b4c0-9910ec6e18b3)  
(Kritisch)  
[DirectX 8.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ce297c3e-8122-4276-a9c2-d1a404f8028d)\*\*\*  
(Kritisch)  
[DirectX 9.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=862db2ad-3c1f-4a26-af70-d8c4f5a69dda)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=89d941f0-3f71-46e3-8096-716561396b72)  
(Keine Bewertung des Schweregrads\*\*)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=50ffc8f4-7ab7-4e64-9965-5767db5f53cd)  
(Kritisch)  
[Microsoft Internet Explorer 6 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=93bd1baa-e2fb-4e8c-9dd7-738efef32282)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-029**](http://go.microsoft.com/fwlink/?linkid=139788)
</td>
<td style="border:1px solid black;">
[**MS09-028**](http://go.microsoft.com/fwlink/?linkid=152887)
</td>
<td style="border:1px solid black;">
[**MS09-032**](http://go.microsoft.com/fwlink/?linkid=157386)
</td>
<td style="border:1px solid black;">
[**MS09-034**](http://go.microsoft.com/fwlink/?linkid=158199)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6914167b-6961-480c-a4d4-808cd58a035b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=09d585cb-481d-4767-875e-9c6ebe456b80)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24701af8-b87e-4e85-9463-f50755a1b6ad)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=22bed634-5227-4a22-8df5-801f3e2e232a)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c874c8f8-0449-42b1-8d8b-901040069568)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0acc8aaa-0ae1-412a-9f2b-dc7c707cae00)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3b8b019e-e6d8-4ce2-8f1f-3a6399b252d1)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](https://www.microsoft.com/download/details.aspx?familyid=f8cd4803-82da-467c-8cb1-520f5a6021d4)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2cbf3699-7f79-4006-99e9-0a4c0d394c48)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=35ab0c5e-df3d-4873-8139-d1d98b3ac350)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=113cc76a-c434-42ff-b594-4834989ad5ba)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=29c8d9e6-2cb8-42b6-b0a6-2510fdb49eab)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-029**](http://go.microsoft.com/fwlink/?linkid=139788)
</td>
<td style="border:1px solid black;">
[**MS09-028**](http://go.microsoft.com/fwlink/?linkid=152887)
</td>
<td style="border:1px solid black;">
[**MS09-032**](http://go.microsoft.com/fwlink/?linkid=157386)
</td>
<td style="border:1px solid black;">
[**MS09-034**](http://go.microsoft.com/fwlink/?linkid=158199)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=018ef53d-f78e-4084-940d-7c86bf59d83c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=571d57c5-1ef8-4dc4-a1e5-2211a805f0cc)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b0a458d6-c34c-41c7-964a-c130cfcb0d01)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=44852619-58ad-48f2-bc55-e8e1c72b1ba9)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f4112c25-9e6f-473a-bdbc-3df6dd66e6af)  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f4ae65a7-142f-4953-a542-315dac2ac606)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7f5fc902-f5d8-4a87-a73f-68632f9a0935)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1779cbc0-0c29-4fac-a3a6-8b335ffcb98e)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8b7a7bb0-80ef-4f25-bc70-3d0ac06007c5)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bd7f36c6-c5c5-4f19-ab59-39f1aaba7fe2)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a594ee0d-ec8f-47df-9125-89d0bbf2115d)  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3bc0e17b-898b-4f29-aa29-607527e1c1cd)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7df0fce2-543c-4e82-85e6-012bfc8bf130)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=48282a89-f849-405a-a31e-2676f45b5042)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7be36edf-02af-402f-983a-f9ca8128b6b5)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=cdb70acf-77c3-40a4-b6a3-0fbc0fc0d7fc)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=adb6bad2-9931-4ede-856e-bb43bb0f6071)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-029**](http://go.microsoft.com/fwlink/?linkid=139788)
</td>
<td style="border:1px solid black;">
[**MS09-028**](http://go.microsoft.com/fwlink/?linkid=152887)
</td>
<td style="border:1px solid black;">
[**MS09-032**](http://go.microsoft.com/fwlink/?linkid=157386)
</td>
<td style="border:1px solid black;">
[**MS09-034**](http://go.microsoft.com/fwlink/?linkid=158199)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c67d85c4-25c5-4821-8db9-91764888f893)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6c90240e-c201-4dad-9835-ea71e3527b45)  
(Keine Bewertung des Schweregrads\*\*)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d3be9a13-1a5b-4b74-9649-449df923f573)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b05a19f7-7412-4c2b-ad11-34396e54ca43)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3f8ae651-59f7-48e1-9e8c-8e07c6806964)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d2084e8d-212b-4c39-9163-a71ec6d1b1c7)  
(Keine Bewertung des Schweregrads\*\*)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2b23cd74-6cf1-413b-82a7-b602347e3ce6)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=900e9a05-2f71-42de-b603-47e4ac061bcb)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-029**](http://go.microsoft.com/fwlink/?linkid=139788)
</td>
<td style="border:1px solid black;">
[**MS09-028**](http://go.microsoft.com/fwlink/?linkid=152887)
</td>
<td style="border:1px solid black;">
[**MS09-032**](http://go.microsoft.com/fwlink/?linkid=157386)
</td>
<td style="border:1px solid black;">
[**MS09-034**](http://go.microsoft.com/fwlink/?linkid=158199)
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
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=91f6ee68-0e39-4ec3-b4cd-45f05404e2fb)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0194f994-5821-4fb9-b9e1-ed6af248c995)\*  
(Keine Bewertung des Schweregrads\*\*)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=92e3af41-71b0-4a28-afc7-123733180ead)\*  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=30f99bda-9107-4969-90af-2a30e12acdae)\*  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5cdc3014-97b3-47b5-a6b7-cd0e12ec60e4)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4127b125-fdaa-489a-a80c-14b5647ac7e0)\*  
(Keine Bewertung des Schweregrads\*\*)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1958ec40-3b7b-43a9-9fdc-742735dcf516)\*  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=acd3667b-6676-4010-b23b-e8372dd55f93)\*  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=03330a14-9cfa-4146-a3d3-4b7a76975d2d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4082c776-318c-4e0c-83fc-2f3f472c039a)  
(Keine Bewertung des Schweregrads\*\*)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=470387ac-6d75-4b7e-8ca5-376b67a8bd4d)  
(Mittel)
</td>
</tr>
</table>
 
**Hinweis für Windows Server 2008**

**\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 nicht, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS09-032**

\**Bewertungen des Schweregrads treffen nicht auf dieses Update zu, da diese Software nicht von der Sicherheitsanfälligkeit betroffen ist, die in diesem Bulletin erörtert wird. Als Tiefenverteidigungsmaßnahme zum Schutz vor möglicherweise in der Zukunft entdeckten Sicherheitsanfälligkeiten empfiehlt Microsoft jedoch den Benutzern dieser Software, dieses Sicherheitsupdate zu installieren.

**Hinweise für MS09-028**

\***Das Update für DirectX 8.1 gilt auch für DirectX 8.1b.

\****Das Update für DirectX 9.0 gilt auch für DirectX 9.0a, DirectX 9.0b und DirectX 9.0c.

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
Microsoft Office Suites, Systeme und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-030**](http://go.microsoft.com/fwlink/?linkid=147424)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2007 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d4b0665d-5744-49c7-a3c0-f231fd08d3b8)  
(KB969693)  
(Hoch)
</td>
</tr>
</table>
 

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
Microsoft Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-035**](http://go.microsoft.com/fwlink/?linkid=158131)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=63ce454e-f69c-44e3-89fb-eb23c2e2154e)  
(KB971089)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2005
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=7c8729dc-06a2-4538-a90d-ff9464dc0197)  
(KB971090)  
(Mittel)  
[Microsoft Visual Studio 2005 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9d7ee45b-9892-41b5-ac08-5fde9cde1b42)\*  
(KB973673)  
(Mittel)  
[Microsoft Visual Studio 2005 Service Pack 1 64-bit Hosted Visual C++ Tools](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=43f96f2a-69c6-4c5e-b72c-0edfa35f4fc2)  
(KB973830)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Embedded CE 6.0
</td>
<td style="border:1px solid black;">
[Windows Embedded CE 6.0](https://www.microsoft.com/download/details.aspx?familyid=99d114f8-4d95-4075-a0f1-45f498f0ade8)\*\*  
(KB974616)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8f9da646-94dd-469d-baea-a4306270462c)  
(KB971091)  
(Mittel)  
[Microsoft Visual Studio 2008](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e3bb6602-b7f4-4614-9999-77f5c6f66ccd)\*  
(KB973674)  
(Mittel)  
[Microsoft Visual Studio 2008 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=294de390-3c94-49fb-a014-9a38580e64cb)  
(KB971092)  
(Mittel)  
[Microsoft Visual Studio 2008 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=75fbf397-5140-4961-92a9-78a88ba7228f)\*  
(KB973675)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual C++ 2005
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2005 Service Pack 1 Redistributable Package](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=766a6af7-ec73-40ff-b072-9112bab119c2)  
(KB973544)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual C++ 2008
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2008 Redistributable Package](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8b29655e-9da4-4b6b-9ac5-687ca0770f93)  
(KB973551)  
(Mittel)  
[Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2051a0c1-c9b5-4b0a-a8f5-770a549fd78c)  
(KB973552)  
(Mittel)
</td>
</tr>
</table>
 
**Hinweise für MS09-035**

\*Für mobile Anwendungen, die „ATL für intelligente Geräte“ verwenden

\*\*Installiert Windows Embedded CE 6.0 im Rahmen der monatlichen Veröffentlichung (Dezember 2009). Dieses Updatepaket ist nur im Microsoft Download Center verfügbar.

#### Microsoft Server und Sicherheitssoftware

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
Microsoft Internet Security and Acceleration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-031**](http://go.microsoft.com/fwlink/?linkid=154993)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Security and Acceleration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2006](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c4e9b1dd-526d-407b-bc23-ebc2738b1b19)  
(KB970811)  
(Hoch)  
[Microsoft Internet Security and Acceleration Server 2006-Unterstützungsupdate](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e8ccd770-a925-411c-b994-78e4cf5c3476)  
(KB970811)  
(Hoch)  
[Microsoft Internet Security and Acceleration Server 2006 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e536cfed-c1af-4868-b2ac-79178d6355a5)  
(KB971143)  
(Hoch)
</td>
</tr>
</table>
 

#### Microsoft-Virtualisierungssoftware

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
Microsoft Virtual PC
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-033**](http://go.microsoft.com/fwlink/?linkid=153891)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Virtual PC 2004
</td>
<td style="border:1px solid black;">
[Microsoft Virtual PC 2004 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=56a160e1-59b5-45bc-aecf-dfe614a7efad)  
(KB969856)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Virtual PC 2007
</td>
<td style="border:1px solid black;">
[Microsoft Virtual PC 2007](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5318c1fa-daf1-4028-832b-eaec9906a46a)  
(KB969856)  
(Hoch)  
[Microsoft Virtual PC 2007 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=88de1513-8d35-410f-8896-fe668f885ca0)  
(KB969856)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Virtual PC 2007 x64 Edition
</td>
<td style="border:1px solid black;">
[Microsoft Virtual PC 2007 x64 Edition](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5318c1fa-daf1-4028-832b-eaec9906a46a)  
(KB969856)  
(Hoch)  
[Microsoft Virtual PC 2007 x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=88de1513-8d35-410f-8896-fe668f885ca0)  
(KB969856)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Virtual Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-033**](http://go.microsoft.com/fwlink/?linkid=153891)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Virtual Server 2005
</td>
<td style="border:1px solid black;">
[Microsoft Virtual Server 2005](https://www.microsoft.com/download/details.aspx?familyid=092a389a-2296-4c3b-a160-2523154ec764)  
(KB969856)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Virtual Server 2005 R2
</td>
<td style="border:1px solid black;">
[Microsoft Virtual Server 2005 R2 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1481024d-b430-4d0e-be16-2f141c6a7e57)  
(KB969856)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Virtual Server 2005 R2 x64 Edition
</td>
<td style="border:1px solid black;">
[Microsoft Virtual Server 2005 R2 x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1481024d-b430-4d0e-be16-2f141c6a7e57)  
(KB969856)  
(Hoch)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) und [Windows-Update](http://go.microsoft.com/fwlink/?linkid=21130) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Hinweis:** Am 1. August 2009 stellt Microsoft den Support für Office Update und das Inventurprogramm für Office-Update ein. Verwenden Sie [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), um weiterhin die aktuellen Updates für Microsoft Office-Produkte zu erhalten. Weitere Informationen finden Sie in [Informationen zum Microsoft Office Update: Häufig gestellte Fragen (FAQs)](http://office.microsoft.com/de-de/downloads/fx010402221031.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung. Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) und das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 für Windows 2000 und neuere Betriebssysteme schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](http://technet.microsoft.com/de-de/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](http://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection-Tool für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/download/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) und im [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Microsoft Application Compatibility Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Microsoft Application Compatibility Toolkit 5.0](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Thomas Garnier von [SkyRecon](http://www.skyrecon.com/) und Zheng Wenbin, Liu Qi und Song Shenlei von [Qihoo 360 Security Center](http://www.360.cn/) für den Hinweis auf ein in MS09-028 beschriebenes Problem.
-   Yamata Li von [Palo Alto Networks](http://www.paloaltonetworks.com/) für den Hinweis auf ein in MS09-028 beschriebenes Problem.
-   Aaron Portnoy von [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) und einer Person, die mit [Zero Day Initiative](http://www.zerodayinitiative.com/) von TippingPoint zusammenarbeitet, aber anonym bleiben möchte, Thomas Garnier von [SkyRecon](http://www.skyrecon.com/) und Yamata Li von [Palo Alto Networks](http://www.paloaltonetworks.com/) für den Hinweis auf ein in MS09-028 beschriebenes Problem.
-   [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS09-029 beschriebenes Problem.
-   Tavis Ormandy von [Google Inc.](http://www.google.com) für den Hinweis auf ein in MS09-029 beschriebenes Problem.
-   Thomas Garnier für den Hinweis auf ein in MS09-029 beschriebenes Problem.
-   Lionel d'Hauenens von [Labo Skopia](http://www.laboskopia.com/), der mit [VeriSign iDefense Labs](http://www.idefense.com/) zusammenarbeitet, für den Hinweis auf ein in MS09-030 beschriebenes Problem.
-   Ryan Smith und Alex Wheeler von [IBM ISS X-Force](http://www.iss.net/) für den ersten Hinweis auf ein in MS09-032 beschriebenes Problem.
-   Julien Tinnes und Tavis Ormandy von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS09-033 beschriebenes Problem.
-   Peter Vreugdenhil von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS09-034 beschriebenes Problem.
-   Wushi und Ling von [team509](http://www.team509.com/) in Zusammenarbeit mit [TippingPoint](http://www.tippingpoint.com/) und [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-034 beschriebenes Problem.
-   Peter Vreugdenhil in Zusammenarbeit mit [TippingPoint](http://www.tippingpoint.com/) und [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-034 beschriebenes Problem.
-   David Dewey von [IBM ISS X-Force](http://www.iss.net/) für den Hinweis auf ein in MS09-035 beschriebenes Problem.
-   Ryan Smith von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf zwei in MS09-035 beschriebene Probleme.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](http://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (14. Juli 2009): Bulletin Summary veröffentlicht.
-   V1.1 (15. Juli 2009): Die Kurzzusammenfassung für MS09-032 wurde aktualisiert, die Neustartanforderungen für MS09-029 korrigiert und verschiedene Bearbeitungen wurden durchgeführt.
-   V2.0 (28. Juli 2009): Es wurden die Microsoft Security Bulletins MS09-034, Kumulatives Sicherheitsupdate für Internet Explorer (972260), und MS09-035, Sicherheitsanfälligkeiten in der Visual Studio Active Template Library können Remotecodeausführung ermöglichen (969706), hinzugefügt. Außerdem wurden die Bulletin-Webcast-Links für diese außerplanmäßigen Security Bulletins hinzugefügt.
-   V3.0 (4. August 2009): Das Bulletin Summary wurde überarbeitet, um die Aktualisierung des Updates für Microsoft Internet Explorer 6 Service Pack 1 unter Microsoft Windows 2000 Service Pack 4 anzukündigen. Alle Benutzer, die das ursprüngliche Update für Internet Explorer 6 Service Pack 1 unter Microsoft Windows 2000 Service Pack 4 bereits installiert haben, sind bereits geschützt. Benutzer jedoch, die über die koreanische Version von Internet Explorer 6 Service Pack 1 verfügen, müssen das Update für Internet Explorer 6 Service Pack 1 erneut auf ihren Windows 2000-Systemen installieren, um den gleichen Schutz zu erhalten und ein Druckausgabeproblem zu beheben. Siehe Microsoft Security Bulletin MS09-034.
-   V4.0 (11. August 2009): Das Bulletin Summary wurde überarbeitet, um die erneute Veröffentlichung von MS09-035 anzukündigen. MS09-035 wurde erneut veröffentlicht, um neue Updates für Microsoft Visual Studio 2005 Service Pack 1 (KB973673), Microsoft Visual Studio 2008 (KB973674) und Microsoft Visual Studio 2008 Service Pack 1 (KB973675) für Entwickler anzubieten, die Visual Studio verwenden, um mit „ATL für intelligente Geräte“ Komponenten und Steuerelemente für mobile Anwendungen zu erstellen.
-   V4.1 (13. August 2009): Die Neustartanforderung für MS09-035 wurde korrigiert.
-   V5.0 (19. August 2009): Es wurde eine Fußnote für Bulletin MS09-028 hinzugefügt, um die betroffene Software für DirectX 8.1 zu verdeutlichen.
-   V6.0 (25. August 2009): Das Bulletin Summary wurde überarbeitet, um die erneute Veröffentlichung des japanischen Updates für Windows XP Service Pack 2, Windows XP Service Pack 3 und Windows XP Professional x64 Edition Service Pack 2 anzukündigen. Alle Benutzer, die das ursprüngliche Update bereits installiert haben, sind bereits geschützt. Benutzer jedoch, die die japanische Version von Windows XP Service Pack 2, Windows XP Service Pack 3 oder Windows XP Professional x64 Edition Service Pack 2 haben, sollten das Update erneut installieren, um den gleichen Schutz zu erhalten und außerdem ein Druckausgabeproblem zu beheben. Siehe Microsoft Security Bulletin MS09-029.
-   V7.0 (12. Januar 2010): Das Bulletin wurde überarbeitet, um Windows Embedded CE 6.0 der betroffenen Software für MS09-035 hinzuzufügen. Das Update für Windows Embedded CE 6.0 (KB974616) ist ein kumulatives Update, das nur im Microsoft Download Center verfügbar ist. Benutzer, die die Windows Embedded CE 6.0-Plattform verwenden, sollten die Installation des kumulativen Updates erwägen.
-   V8.0 (9. März 2010): Das Bulletin wurde überarbeitet, um Microsoft Virtual Server 2005 als betroffene Software für MS09-033 hinzuzufügen.

*Built at 2014-04-18T01:50:00Z-07:00*
