---
TOCTitle: 'MS09-APR'
Title: Microsoft Security Bulletin Summary für April 2009
ms:assetid: 'ms09-apr'
ms:contentKeyID: 61225067
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für April 2009
==================================================

Veröffentlicht: Dienstag, 14. April 2009 | Aktualisiert: Donnerstag, 16. April 2009

**Version:** 1.1

In diesem Bulletin Summary sind die im April 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für April 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 9. April 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 15. April 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im April](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395126). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139849">MS09-010</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in WordPad- und Office-Textkonvertern können Remotecodeausführung ermöglichen (960477)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete und zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft WordPad- und Microsoft Office-Textkonvertern. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn eine speziell gestaltete Datei in WordPad oder Microsoft Office Word geöffnet wird. Öffnen Sie keine Microsoft Office-, RTF-, Write- oder WordPerfect-Dateien, die von nicht vertrauenswürdigen Quellen stammen, mit betroffenen Versionen von WordPad oder Microsoft Office Word.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139852">MS09-013</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in den Windows HTTP-Diensten können Remotecodeausführung ermöglichen (960803)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und zwei vertraulich gemeldete Sicherheitsanfälligkeiten in den Microsoft Windows HTTP-Diensten (WinHTTP). Die schwerste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139107">MS09-011</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft DirectShow kann Remotecodeausführung ermöglichen (961373)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft DirectX. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete MJPEG-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=146659">MS09-014</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (963027)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten und zwei öffentlich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite über Internet Explorer öffnet oder wenn ein Benutzer eine Verbindung zum Server eines Angreifers über das HTTP-Protokoll herstellt. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=143568">MS09-009</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (968557)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit und eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Office Excel. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132587">MS09-012</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows können Erhöhung von Berechtigungen ermöglichen (959454)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vier öffentlich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer beim System anmelden und anschließend eine speziell gestaltete Anwendung ausführen kann. Der Angreifer muss Code auf dem lokalen Computer ausführen können, um diese Sicherheitsanfälligkeit auszunutzen. Ein Angreifer, dem es gelingt, eine dieser Sicherheitsanfälligkeiten auszunutzen, kann vollständige Kontrolle über das betroffene System erlangen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141639">MS09-016</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft ISA Server und Forefront Threat Management Gateway (Medium Business Edition) können ein Denial-of-Service verursachen (961759)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit und eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Internet Security and Acceleration (ISA) Server und Microsoft Forefront Threat Management Gateway (TMG), Medium Business Edition (MBE). Diese Sicherheitsanfälligkeiten können zu einem Denial-of-Service führen, wenn ein Angreifer speziell gestaltete Netzwerkpakete an das betroffene System sendet, oder zur Offenlegung von Informationen, wenn ein Benutzer auf eine schädliche URL klickt oder eine Website besucht, die vom Angreifer kontrollierten Inhalt enthält.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Forefront Edge Security</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=146803">MS09-015</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit durch komplexe Bedrohung in SearchPath kann Erhöhung von Berechtigungen ermöglichen (959426)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in der Windows SearchPath-Funktion, die eine Erhöhung von Berechtigungen ermöglichen kann, wenn ein Benutzer eine speziell gestaltete Datei an einen bestimmten Ort heruntergeladen und anschließend eine Anwendung geöffnet hat, die die Datei unter bestimmten Umständen laden kann.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Mittel</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID geordnet.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Kennung des Bulletins                                     | Titel des Bulletins                                                                                                                                                   | CVE-ID                                                                               | Ausnutzbarkeitsindex – Bewertung                                                                                     | Wichtige Hinweise                                                                                                                                                                                                                                                                                                                    |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-009](http://go.microsoft.com/fwlink/?linkid=143568) | Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (968557)                                                                  | [CVE-2009-0100](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0100)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                              |  
| [MS09-009](http://go.microsoft.com/fwlink/?linkid=143568) | Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (968557)                                                                  | [CVE-2009-0238](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0238)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**                                                                                                                                                                                                                                                   |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Sicherheitsanfälligkeiten in WordPad- und Office-Textkonvertern können Remotecodeausführung ermöglichen (960477)                                                      | [CVE-2008-4841](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4841)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**                                                                                                                                                                                                                                                   |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Sicherheitsanfälligkeiten in WordPad- und Office-Textkonvertern können Remotecodeausführung ermöglichen (960477)                                                      | [CVE-2009-0087](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0087)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Dies ist eine komplexe Sicherheitsanfälligkeit aufgrund mehrerer Codepfade. Die meisten Angreifercodes führen zu inkonsistenten Ergebnissen. Standardmäßige schadensbegrenzende Faktoren schützen vor diesem Angriff.                                                                                                                |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Sicherheitsanfälligkeiten in WordPad- und Office-Textkonvertern können Remotecodeausführung ermöglichen (960477)                                                      | [CVE-2009-0088](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0088)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Diese Sicherheitsanfälligkeit kann ausgenutzt werden, betrifft aber nur ältere Versionen und ein älteres, nicht übliches Dateiformat. Neuere Versionen wie z. B. Microsoft Office System 2007 und Microsoft Office 2003 Service Pack 3 sind nicht betroffen.                                                                         |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Sicherheitsanfälligkeiten in WordPad- und Office-Textkonvertern können Remotecodeausführung ermöglichen (960477)                                                      | [CVE-2009-0235](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0235)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Diese Sicherheitsanfälligkeit bezüglich Speicherbeschädigung kann leicht ausgenutzt werden.                                                                                                                                                                                                                                          |  
| [MS09-011](http://go.microsoft.com/fwlink/?linkid=139107) | Sicherheitsanfälligkeit in Microsoft DirectShow kann Remotecodeausführung ermöglichen (961373)                                                                        | [CVE-2009-0084](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0084)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                              |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Sicherheitsanfälligkeiten in Windows können Erhöhung von Berechtigungen ermöglichen (959454)                                                                          | [CVE-2008-1436](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-1436)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**                                                                                                                                                                                                                                                   |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Sicherheitsanfälligkeiten in Windows können Erhöhung von Berechtigungen ermöglichen (959454)                                                                          | [CVE-2009-0078](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0078)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**                                                                                                                                                                                                                                                   |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Sicherheitsanfälligkeiten in Windows können Erhöhung von Berechtigungen ermöglichen (959454)                                                                          | [CVE-2009-0079](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0079)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**                                                                                                                                                                                                                                                   |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Sicherheitsanfälligkeiten in Windows können Erhöhung von Berechtigungen ermöglichen (959454)                                                                          | [CVE-2009-0080](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0080)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.**                                                                                                                                                                                                                                                   |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Sicherheitsanfälligkeiten in den Windows HTTP-Diensten können Remotecodeausführung ermöglichen (960803)                                                               | [CVE-2009-0086](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0086)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Diese Sicherheitsanfälligkeit im Speicher kann leicht gesteuert werden, durch mehrere Angriffsmethoden und die Möglichkeiten zur Ausnutzung aufgrund weit verbreiteter Verwendung dieser Technologie.                                                                                                                                |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Sicherheitsanfälligkeiten in den Windows HTTP-Diensten können Remotecodeausführung ermöglichen (960803)                                                               | [CVE-2009-0089](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0089)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                              |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Sicherheitsanfälligkeiten in den Windows HTTP-Diensten können Remotecodeausführung ermöglichen (960803)                                                               | [CVE-2009-0550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0550)\*\* | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Es wurde Angreifercode veröffentlicht.                                                                                                                                                                                                                                                                                               |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulatives Sicherheitsupdate für Internet Explorer (963027)                                                                                                          | [CVE-2008-2540](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2540)\*   | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Details zum Angriff wurden veröffentlicht, aber es liegen derzeit keine bekannten Angriffsmethoden für dieses Problem vor. Um diese Sicherheitsanfälligkeit erfolgreich auszunutzen, müssen ein Angreifer und der Benutzer eine Reihe komplizierter Schritte ausführen, einschließlich Speichern bestimmter Dateien auf dem Desktop. |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulatives Sicherheitsupdate für Internet Explorer (963027)                                                                                                          | [CVE-2009-0550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0550)\*\* | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | Es wurde Angreifercode veröffentlicht.                                                                                                                                                                                                                                                                                               |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulatives Sicherheitsupdate für Internet Explorer (963027)                                                                                                          | [CVE-2009-0551](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0551)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                                                                                                                                                                                                              |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulatives Sicherheitsupdate für Internet Explorer (963027)                                                                                                          | [CVE-2009-0552](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0552)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Schadensbegrenzende Faktoren für Internet Explorer 7 verhindern Codeausführung. Bei Internet Explorer 6 und früheren Versionen ist die Wahrscheinlichkeit der Ausnutzung höher, wenn diese Versionen nicht mit allen Sicherheitsupdates aktualisiert wurden.                                                                         |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulatives Sicherheitsupdate für Internet Explorer (963027)                                                                                                          | [CVE-2009-0553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0553)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | (Keine)                                                                                                                                                                                                                                                                                                                              |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulatives Sicherheitsupdate für Internet Explorer (963027)                                                                                                          | [CVE-2009-0554](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0554)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                                                                                                                                                                                                              |  
| [MS09-015](http://go.microsoft.com/fwlink/?linkid=146803) | Sicherheitsanfälligkeit durch komplexe Bedrohung in SearchPath kann Erhöhung von Berechtigungen ermöglichen (959426)                                                  | [CVE-2008-2540](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2540)\*   | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Details zum Angriff wurden veröffentlicht, aber es liegen derzeit keine bekannten Angriffsmethoden für dieses Problem vor. Um diese Sicherheitsanfälligkeit erfolgreich auszunutzen, müssen ein Angreifer und der Benutzer eine Reihe komplizierter Schritte ausführen, einschließlich Speichern bestimmter Dateien auf dem Desktop. |  
| [MS09-016](http://go.microsoft.com/fwlink/?linkid=141639) | Sicherheitsanfälligkeiten in Microsoft ISA Server und Forefront Threat Management Gateway (Medium Business Edition) können ein Denial-of-Service verursachen (961759) | [CVE-2009-0077](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0077)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dienstbasierter Denial-of-Service ist sehr wahrscheinlich. Codeausführung ist jedoch nicht möglich.                                                                                                                                                                                                                                  |  
| [MS09-016](http://go.microsoft.com/fwlink/?linkid=141639) | Sicherheitsanfälligkeiten in Microsoft ISA Server und Forefront Threat Management Gateway (Medium Business Edition) können ein Denial-of-Service verursachen (961759) | [CVE-2009-0237](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-0237)          | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Offenlegung von Information ist möglich. Codeausführung ist sehr unwahrscheinlich.                                                                                                                                                                                                                                                   |
  
\*Diese beiden Sicherheitsanfälligkeiten, denen die gleiche CVE-Nummer zugewiesen wurde, werden in zwei Sicherheitsupdates behandelt. Weitere Informationen finden Sie in den jeweiligen Bulletins.
  
\*\*Diese beiden Sicherheitsanfälligkeiten, denen die gleiche CVE-Nummer zugewiesen wurde, werden in zwei Sicherheitsupdates behandelt. Weitere Informationen finden Sie in den jeweiligen Bulletins.
  
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
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=552d322a-5282-42c7-9c1e-1d8c494a7318)  
(KB923561)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=39d5468e-5733-4c3e-9e75-3adac8ac8cb9)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 8.1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0ec5b7c7-13d3-467a-b24e-3cc6fb47adf6)  
(Kritisch)  
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8b98ed5c-a3ab-45a7-a61e-349eae304bc6)\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7799fd05-5b26-449f-8a14-50227c9164d1)  
(Kritisch)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=87f0c380-5c31-4099-a6a9-c12f9d69b03b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=52b756e7-636f-4d9e-8a17-dbf467bfbe4d)  
(KB952004)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c4e408d7-6716-4a12-ad3a-8029667f5c84)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=50a8519a-503e-43dd-a78a-c1bc764fd213)  
(KB923561)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=35af4151-1858-4c9a-85e4-9ff45feca1a4)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=feb5d821-f210-40e8-b1aa-2ca3170df8df)\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=052c29fc-e8df-402c-9ab1-1079bc738e1b)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=55d6729a-9f96-4da4-b564-676c0a0c9390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows XP Service Pack 2 und Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=90fe715e-8190-43e9-9c43-df5be564d923)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows XP Service Pack 2 und Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=73d2324f-be59-4b0c-b1ac-9876a13c2c03)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3de0684d-605c-489b-bdc7-08bce9b2d4f6)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=323f4211-5add-4e02-bce1-e5a1b489982c)  
(KB923561)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=49b16f0f-f6c3-4ca8-8041-392f4f7b5bbb)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=f1be8b7c-4874-4342-99b3-76ff725fbb9a)\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=84c62211-2e82-4ccc-9f9b-26462b026d86)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=191c2f20-89ae-4e1c-bdd4-24b4abfe6b6c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a794c32a-9a0c-47d9-9c57-ff5d4a8e4944)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b2f12ae5-0e46-47e1-ac5b-93550d030189)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b743a7fe-7bf4-420d-a72e-39471e5659fa)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2233a4d2-7c8a-4c89-b020-100d9afb43c8)  
(KB923561)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=42509f5a-d0f9-444a-9445-5eabdb555011)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c1b4cd76-1dd6-43fa-bb9a-20c428985bfd)\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f73a3669-c17f-4b18-8456-96cb7d52ed86)  
(Hoch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6a45dbd0-0520-4d9b-b76e-3f5109dd310d)  
(Hoch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=25adec10-db8c-4cac-bf74-2c784678150a)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=42aba890-8b76-4c5a-8fb6-609797d19831)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=992bb0cd-fbc7-4a7c-9088-f7f9d9a3ead0)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=323f4211-5add-4e02-bce1-e5a1b489982c)  
(KB923561)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7373ea32-bc2e-49f1-8b9f-4eeda5acc74c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f0e1e1db-94a5-451c-ab11-6b431fa065f1)\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=03a9d581-2bd5-4151-9826-17b96e16f606)  
(Hoch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=60ccc1d6-ea31-420c-b630-d7878a8dc527)  
(Hoch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=b014c399-f404-4cb2-8f9d-864df382efeb)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a0609f65-82d9-4d82-9f48-f3266e8de123)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f0a58e8c-7d63-4d7d-ba95-b3787cf408f0)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e840b9cb-f1f4-482a-aa07-eb6b42b477c4)  
(KB923561)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=05e33cc5-cff6-4c71-be71-285f66a95e01)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8f36c215-fa8a-40c2-b680-6b1fece03b8d)\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=53d13c07-80b0-4f05-b372-a2dac17e6157)  
(Hoch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0abaa2fb-7c4f-4149-993d-1575888bfc84)  
(Hoch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6ada372b-ba17-433e-b022-d2c57b35af8a)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=fda8837c-e5d2-4489-9b44-4c24a1102e77)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=00c6479d-f81f-445d-b8e4-7b71d77d540a)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista und Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f071d770-3b6b-4040-9911-d4de8cde4c68)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d743849d-f3b5-4114-adef-ade2716d55ac)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f111b99a-e555-4f29-8d1f-e9ec03d5cf1f)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d0ea1598-45cb-4c79-8945-caae98969675)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2b672d45-f33b-4edc-9f22-2f2c8c726a8b)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7ceef2d0-f316-48d1-aecc-d74f91cc5e1f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d191c8dc-a965-4a6a-b6d8-1470505eb55f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=fa153bdc-6b48-4df2-9e5e-abacd6da782c)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6dd82f4b-bb33-41ec-90a7-9ef91329b240)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7576e7d5-5bb1-4a53-b568-1ee0500ce721)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4c36548f-c8c9-4318-91e2-9e0501339548)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e2c6313c-3ba9-4f7c-b259-b4582a390146)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9e3c7b52-65a7-42fb-beb5-1b374934737f)\*  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d58702af-bbf8-4f1b-ae72-ced9ef23d581)\*  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6b73cf5e-66fe-4b7d-95fc-91a1c262c1e5)\*  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1c3f0997-a8a9-4340-ae0c-2c4d6792c65c)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ebbade9d-704c-440b-8796-6d64225ac01a)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eebb4d4d-29d2-4247-8cbb-63a3b17585ec)\*  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=20bf4e9b-909b-4bc3-ae43-322d74a4f1c3)\*  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7e60847c-b341-4c38-bc25-2e3cf2d4ae14)\*  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0885b3b0-b78e-4980-902d-dff3886bcaac)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1b04aa6f-b787-4122-bf82-0d150618fe7a)  
(Hoch)
</td>
<td style="border:1px solid black;">
Aktualisierung der MSDTC-Transaktionsfunktion:  
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=cc383c24-b0f6-47c1-9e89-6a378b09e82f)  
(KB952004)  
(Hoch)  
Aktualisierung der Windows-Dienstisolierung:  
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=bcc2b18f-67db-4109-a9f4-764f985423ee)  
(KB956572)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=de1c2b4b-af47-4b9a-8363-720e5527573c)  
(Mittel)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008**

**\*Die Server Core-Installation von Windows Server 2008 ist betroffen.** Für unterstützte Editionen von Windows Server 2008 gilt dieses Update mit der gleichen Bewertung des Schweregrads. Dabei spielt es keine Rolle, ob Windows Server 2008 mit der Server Core-Installationsoption installiert wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**\*\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 nicht, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**Hinweis für MS09-010**

Im Abschnitt **Microsoft Office Suites und Software** finden Sie weitere Aktualisierungsdateien. Dieses Bulletin umfasst sowohl Windows-Betriebssystem als auch Komponenten und Microsoft Office Suites und Software.

**Hinweis für MS09-011**

\*\*\*Das Update für DirectX 9.0 gilt auch für DirectX 9.0a, DirectX 9.0b und DirectX 9.0c.

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
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=95876927-e612-414c-bdec-3632a3100415)  
(KB921606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3dc8b670-25a5-4f46-b7de-12bc693b628a)  
(KB959964)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e1db55c6-78fb-498d-89a5-9ad54d971546)  
(KB933399)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9a52bf4b-05f6-4b73-94b9-28ed7e20f86c)  
(KB959988)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d9dbfa63-c0cb-4c84-9b8a-6e52568045b0)  
(KB959995)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=50d8630b-1365-4007-81a0-18c0d6d4b86e)\*  
(KB959997)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=52271140-89be-4b9c-baa2-cea09097d703)  
(KB968695)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f6e407eb-11a5-433f-8006-4b822953ca98)  
(KB968694)  
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
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c72e6087-b48f-4d2d-8366-01d9f5ff6b6c)  
(KB959993)  
(Hoch)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=58b3929c-5373-47a4-aa97-66d179758792)  
(KB960000)  
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
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=05f7c517-e551-4dcd-b24a-5d548f2d09cf)  
(KB960003)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Converter Pack
</td>
<td style="border:1px solid black;">
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=d763fae3-b2af-47f9-a554-ec786766b3c3)  
(KB960476)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis für MS09-010**

Weitere Updatedateien finden Sie auch in dem Abschnitt **Windows-Betriebssystem und Komponenten**. Dieses Bulletin umfasst sowohl Windows-Betriebssystem als auch Komponenten und Microsoft Server-Software.

**Hinweis für MS09-009**

\*Für Microsoft Office Excel 2007 Service Pack 1 müssen Benutzer auch das Sicherheitsupdate für Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1 installieren, um vor den in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten geschützt zu sein.

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
Microsoft Forefront
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-016**](http://go.microsoft.com/fwlink/?linkid=141639)
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
Microsoft Forefront Threat Management Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Threat Management Gateway, Medium Business Edition](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6abf9fb4-42d0-4c67-935f-8dc67850148b)\*  
(KB968075)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Internet Security and Acceleration Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-016**](http://go.microsoft.com/fwlink/?linkid=141639)
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
Microsoft Internet Security and Acceleration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2004 Standard Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=adf623fa-2d74-4f2a-9835-4b8debdb0e1b)\*\*  
(KB960995)  
(Hoch)  
[Microsoft Internet Security and Acceleration Server 2004 Enterprise Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d1d55ab6-3de5-4811-9693-8d43f49f5fe8)  
(KB960995)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Security and Acceleration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2006](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Hoch)  
[Microsoft Internet Security and Acceleration Server 2006-Unterstützungsupdate](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Hoch)  
[Microsoft Internet Security and Acceleration Server 2006 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS09-016**

\*Microsoft Forefront Threat Management Gateway, Medium Business Edition, wird sowohl als eigenständiges Produkt als auch als Komponente von Windows Essential Business Server 2008 angeboten.

\*\*Microsoft ISA Server 2004 Standard Edition wird als eigenständiges Produkt angeboten. Microsoft ISA Server 2004 Standard Edition wird auch als Komponente von Windows Small Business Server 2003 Enterprise Edition Service Pack 1 und Windows Small Business Server 2003 R2 Enterprise Edition angeboten.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Security Center](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch über [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](http://office.microsoft.com/de-de/downloads/default.aspx) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) und das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 für Windows 2000 und neuere Betriebssysteme schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](http://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection-Tool für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), die im [Anwendungskompatibilitäts-Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Anwendungskompatibilitäts-Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Haifei Li von Fortinets [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) für den Hinweis auf ein in MS09-009 beschriebenes Problem.
-   Sean Larsson und Jun Mao von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS09-010 beschriebenes Problem.
-   Einem Forscher des [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) von Fortinet für den Hinweis auf ein in MS09-010 beschriebenes Problem.
-   Einem Forscher der [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS09-010 beschriebenes Problem.
-   Piotr Bania von [Kryptos Logic](http://www.kryptoslogic.com/) für den Hinweis auf ein in MS09-011 beschriebenes Problem.
-   Cesar Cerrudo von [Argeniss](http://www.argeniss.com/) für den Hinweis auf mehrere in MS09-012 beschriebene Probleme.
-   Greg MacManus von [iSIGHT Partners Labs](http://www.isightpartners.com/) für den Hinweis auf ein in MS09-013 beschriebenes Problem.
-   WanTeh Chang und Cem Paya von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS09-013 beschriebenes Problem.
-   [Aviv Raff](http://aviv.raffon.net/) für den Hinweis auf ein in MS09-014 beschriebenes Problem.
-   Michal Zalewski von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS09-014 beschriebenes Problem.
-   Ivan Fratric von [iSIGHT Partners Labs](http://www.isightpartners.com/) für den Hinweis auf ein in MS09-014 beschriebenes Problem.
-   Skylined von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS09-014 beschriebenes Problem.
-   ADLab von [VenusTech](http://www.venustech.com.cn/) für den Hinweis auf ein in MS09-014 beschriebenes Problem.
-   [Aviv Raff](http://aviv.raffon.net/) für den Hinweis auf ein in MS09-015 beschriebenes Problem.
-   New York State Chief Information Officer/Office for Technology für den Hinweis auf ein in MS09-016 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](http://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (14. April 2009): Bulletin Summary veröffentlicht.
-   V1.1 (16. April 2009): Der Ausnutzbarkeitsindex wurde aktualisiert: Wichtige Hinweise für CVE-2009-0089 wurden entfernt und wichtige Hinweise für CVE-2008-2540 in MS09-014 und MS09-015 wurden geändert.

*Built at 2014-04-18T01:50:00Z-07:00*
