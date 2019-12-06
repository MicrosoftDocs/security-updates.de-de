---
TOCTitle: 'MS14-FEB'
Title: Microsoft Security Bulletin Summary für Februar 2014
ms:assetid: 'ms14-feb'
ms:contentKeyID: 61597926
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms14-feb(v=Security.10)'
---

Microsoft Security Bulletin Summary für Februar 2014
====================================================

Microsoft Security Bulletin Summary für Februar 2014
----------------------------------------------------

Veröffentlicht: Veröffentlicht: 11. Februar 2014 | Aktualisiert: 13. Februar 2014

**Version:** 1.2

In diesem Bulletin Summary sind die im Februar 2014 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Februar 2014 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 10. Februar 2014 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, den 12. Februar 2014 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Februar](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032572879&culture=en-us).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt Weitere Informationen.

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Security Bulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im nächsten Abschnitt Betroffene Software.

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><strong>Titel des Bulletins und Kurzzusammenfassung</strong></td>
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads und Sicherheitsauswirkung</strong></td>
<td style="border:1px solid black;"><strong>Neustartanforderung</strong></td>
<td style="border:1px solid black;"><strong>Betroffene Software</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (2909921)<br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich und dreiundzwanzig vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der die schwerwiegendste dieser Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=391023">MS14-011</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Skriptmodul VBScript kann Remotecodeausführung ermöglichen (2928390)<br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Skriptmodul VBScript in Microsoft Windows. Wenn ein Benutzer eine speziell gestaltete Website besucht, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Ein Angreifer kann Benutzer nicht zum Besuch einer bestimmten Website zwingen. Er muss den Benutzer dazu verleiten, aktiv zu werden. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386447">MS14-007</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Direct2D kann Remotecodeausführung ermöglichen (2912390)<br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Ein Angreifer kann Benutzer jedoch nicht zwingen, die speziell gestalteten Inhalte anzuzeigen. Stattdessen muss ein Angreifer Benutzer zu Handlungen verleiten. Zu diesem Zweck werden Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder einer Instant Messenger-Nachricht zu klicken, wodurch die Benutzer zur Website eines Angreifers gelangen, oder eine Dateianlage zu öffnen, die per E-Mail gesendet wurde.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390218">MS14-008</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Forefront Protection für Exchange kann Remotecodeausführung ermöglichen (2927022)<br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Forefront. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn eine speziell gestaltete E-Mail gescannt wird.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Sicherheitssoftware</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386454">MS14-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in .NET Framework können Erhöhung von Berechtigungen ermöglichen (2916607)<br />
<br />
Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete Sicherheitsanfälligkeiten und eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft .NET Framework. Die schwerwiegendste Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer eine speziell gestaltete Website oder eine Website mit speziell gestalteten Webinhalten besucht. Ein Angreifer kann Endbenutzer jedoch nicht zum Besuch solcher Websites zwingen. Er muss den Benutzer zum Besuch der schädlichen Webseite verleiten. Zu diesem Zweck wird der Benutzer normalerweise dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=391022">MS14-005</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Microsoft XML Core Services kann Offenlegung von Informationen ermöglichen (2916036)<br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft XML Core Services, die in Microsoft Windows enthalten sind. Die öffentliche gemeldete Sicherheitsanfälligkeit kann zur Offenlegung von Informationen führen, wenn ein Benutzer eine speziell gestaltete Webseite unter Verwendung von Internet Explorer anzeigt. Ein Angreifer kann Benutzer jedoch nicht zwingen, die speziell gestalteten Inhalte anzuzeigen. Stattdessen muss ein Angreifer Benutzer zu Handlungen verleiten. Zu diesem Zweck werden Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder einer Instant Messenger-Nachricht zu klicken, wodurch die Benutzer zur Website eines Angreifers gelangen, oder eine Dateianlage zu öffnen, die per E-Mail gesendet wurde.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386450">MS14-006</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in IPv6 kann zu einem Denial-of-Service-Angriff führen (2904659)<br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer eine große Anzahl speziell gestalteter IPv6-Pakete an ein betroffenes System sendet. Um diese Sicherheitsanfälligkeit auszunutzen, muss das System eines Angreifers zu demselben Subnetz gehören wie das Zielsystem.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
 
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
Wie verwende ich diese Tabelle?
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
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
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><strong>Titel der Sicherheitsanfälligkeit</strong></td>
<td style="border:1px solid black;"><strong>CVE-ID</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für ältere Softwareversionen</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit durch Denial-of-Service</strong></td>
<td style="border:1px solid black;"><strong>Wichtige Hinweise</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=391022">MS14-005</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MSXML durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0266">CVE-2014-0266</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.<br />
<br />
Microsoft ist sich gezielter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386450">MS14-006</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Denial-of-Service in TCP/IP Version 6 (IPv6)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0254">CVE-2014-0254</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386447">MS14-007</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in der Microsoft Graphics-Komponente bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0263">CVE-2014-0263</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390218">MS14-008</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0294">CVE-2014-0294</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386454">MS14-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Denial-of-Service in POST-Anforderung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0253">CVE-2014-0253</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386454">MS14-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Typüberquerung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0257">CVE-2014-0257</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=386454">MS14-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in VSAVB7RT durch ASLR</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0295">CVE-2014-0295</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit aufgrund der Umgehung von Sicherheitsfunktionen.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.<br />
<br />
Microsoft ist sich begrenzter, gezielter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0267">CVE-2014-0267</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0268">CVE-2014-0268</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0269">CVE-2014-0269</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0270">CVE-2014-0270</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0271">CVE-2014-0271</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0272">CVE-2014-0272</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0273">CVE-2014-0273</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0274">CVE-2014-0274</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0275">CVE-2014-0275</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0276">CVE-2014-0276</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0277">CVE-2014-0277</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0278">CVE-2014-0278</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0279">CVE-2014-0279</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0280">CVE-2014-0280</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0281">CVE-2014-0281</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0283">CVE-2014-0283</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0284">CVE-2014-0284</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0285">CVE-2014-0285</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0286">CVE-2014-0286</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0287">CVE-2014-0287</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0288">CVE-2014-0288</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0289">CVE-2014-0289</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0290">CVE-2014-0290</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=390977">MS14-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch domänenübergreifende Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0293">CVE-2014-0293</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=391023">MS14-011</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in VBScript bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-0271">CVE-2014-0271</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
</tbody>
</table>
  
Betroffene Software  
-------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
Wie verwende ich diese Tabellen?
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.
  
Hinweis: Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows XP**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Internet Explorer 6   
(2909921)  
(Kritisch)  
Internet Explorer 7   
(2909921)  
(Kritisch)  
Internet Explorer 8   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Kritisch)  
VBScript 5.8   
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0 Service Pack 3  
(2904878)  
(Hoch)  
(nur Media Center Edition 2005 Service Pack 3 und Tablet PC Edition 2005 Service Pack 3)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2901111)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898856)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 3  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6   
(2909921)  
(Kritisch)  
Internet Explorer 7   
(2909921)  
(Kritisch)  
Internet Explorer 8   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.6  
(2909213)  
(Kritisch)  
VBScript 5.7   
(2909212)  
(Kritisch)  
VBScript 5.8   
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901111)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898856)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Mittel](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Niedrig](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Internet Explorer 6   
(2909921)  
(Mittel)  
Internet Explorer 7  
(2909921)  
(Mittel)  
Internet Explorer 8  
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.6  
(2909213)  
(Mittel)  
VBScript 5.7   
(2909212)  
(Mittel)  
VBScript 5.8   
(2909210)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1 Service Pack 1  
(2901115)  
(Hoch)  
Microsoft .NET Framework 1.1 Service Pack 1  
(2898860)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2901111)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898856)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6   
(2909921)  
(Mittel)  
Internet Explorer 7  
(2909921)  
(Mittel)  
Internet Explorer 8  
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.6  
(2909213)  
(Mittel)  
VBScript 5.7   
(2909212)  
(Mittel)  
VBScript 5.8   
(2909210)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901111)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898856)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2916036)  
(Niedrig)
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
Internet Explorer 6   
(2909921)  
(Mittel)  
Internet Explorer 7  
(2909921)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.6  
(2909213)  
(Mittel)  
VBScript 5.7   
(2909212)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901111)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898856)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2909921)  
(Kritisch)  
Internet Explorer 8  
(2909921)  
(Kritisch)  
Internet Explorer 9   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 9  
(2909921)<sup>[1]</sup>
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901113)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898858)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2911502)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2909921)  
(Kritisch)  
Internet Explorer 8  
(2909921)  
(Kritisch)  
Internet Explorer 9   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 9  
(2909921)<sup>[1]</sup>
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901113)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898858)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2911502)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Mittel](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Niedrig](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2909921)  
(Mittel)  
Internet Explorer 8  
(2909921)  
(Hoch)  
Internet Explorer 9   
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Mittel)  
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Mittel)  
VBScript 5.8 für Systeme mit Internet Explorer 9  
(2909921)<sup>[1]</sup>
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901113)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898858)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2911502)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2909921)  
(Mittel)  
Internet Explorer 8  
(2909921)  
(Hoch)  
Internet Explorer 9   
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Mittel)  
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Mittel)  
VBScript 5.8 für Systeme mit Internet Explorer 9  
(2909921)<sup>[1]</sup>
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901113)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898858)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2911502)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2909921)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2901113)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2898858)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2911502)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2909921)  
(Kritisch)  
Internet Explorer 9   
(2909921)  
(Kritisch)  
Internet Explorer 10   
(2909921)  
(Kritisch)  
Internet Explorer 11   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 9  
(2909921)<sup>[1]</sup>
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 10  
(2909210)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 11  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2901112)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2898857)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2911501)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2909921)  
(Kritisch)  
Internet Explorer 9   
(2909921)  
(Kritisch)  
Internet Explorer 10   
(2909921)  
(Kritisch)  
Internet Explorer 11   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 9  
(2909921)<sup>[1]</sup>
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 10  
(2909210)  
(Kritisch)  
VBScript 5.8 für Systeme mit Internet Explorer 11  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2901112)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2898857)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2911501)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Mittel](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Niedrig](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2909921)  
(Hoch)  
Internet Explorer 9   
(2909921)  
(Hoch)  
Internet Explorer 10   
(2909921)  
(Hoch)  
Internet Explorer 11   
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Mittel)  
VBScript 5.8 für Systeme mit Internet Explorer 9  
(2909921)<sup>[1]</sup>
(Mittel)  
VBScript 5.8 für Systeme mit Internet Explorer 10  
(2909210)  
(Mittel)  
VBScript 5.8 für Systeme mit Internet Explorer 11  
(2909210)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2901112)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2898857)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2911501)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 8  
(2909210)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2901112)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2898857)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2911501)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4  
(2898855)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 10  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901120)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898866)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901119)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898865)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901127)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898870)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2904659)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 10  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901120)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898866)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901119)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898865)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901127)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898870)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(2904659)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 11  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901125)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898868)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901128)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898871)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 11  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901125)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898868)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901128)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898871)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Mittel](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Niedrig](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10   
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 10  
(2909210)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901120)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898866)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901119)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898865)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901127)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898870)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2904659)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11   
(2909921)  
(Hoch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 11  
(2909210)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901125)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898868)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901128)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898871)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 10  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5  
(2901119)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898865)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901127)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898870)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(2904659)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11   
(2909921)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.8 für Systeme mit Internet Explorer 11  
(2909210)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(2912390)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.1  
(2901128)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898871)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(2916036)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-010](https://go.microsoft.com/fwlink/?linkid=390977)
</td>
<td style="border:1px solid black;">
[MS14-011](https://go.microsoft.com/fwlink/?linkid=391023)
</td>
<td style="border:1px solid black;">
[MS14-007](https://go.microsoft.com/fwlink/?linkid=386447)
</td>
<td style="border:1px solid black;">
[MS14-009](https://go.microsoft.com/fwlink/?linkid=386454)
</td>
<td style="border:1px solid black;">
[MS14-005](https://go.microsoft.com/fwlink/?linkid=391022)
</td>
<td style="border:1px solid black;">
[MS14-006](https://go.microsoft.com/fwlink/?linkid=386450)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
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
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Niedrig](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[Hoch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
VBScript 5.7   
(2909212)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
VBScript 5.8   
(2909210)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2901112)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2898857)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2911501)  
(Hoch)  
Microsoft .NET Framework 4  
(2901110)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901118)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898864)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901126)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
VBScript 5.8   
(2909210)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901120)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898866)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2901119)  
(Hoch)  
Microsoft .NET Framework 4.5  
(2898865)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901127)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898870)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(2904659)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
VBScript 5.8   
(2909210)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2901125)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2898868)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2901128)  
(Hoch)  
Microsoft .NET Framework 4.5.1  
(2898871)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(2916036)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
Hinweis für MS14-011

<sup>[1]</sup>Auf Systemen mit Internet Explorer 9 wird die Sicherheitsanfälligkeit durch das kumulative Update 2909921 für Internet Explorer 9 in [MS14-010](https://go.microsoft.com/fwlink/?linkid=390977) behoben.

 

### Microsoft Sicherheitssoftware

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Forefront Protection 2010 für Exchange Server**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Kennung des Bulletins
</td>
<td style="border:1px solid black;">
[MS14-008](https://go.microsoft.com/fwlink/?linkid=390218)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bewertung des Gesamtschweregrads
</td>
<td style="border:1px solid black;">
[Kritisch](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Forefront Protection 2010 für Exchange Server
</td>
<td style="border:1px solid black;">
Microsoft Forefront Protection 2010 für Exchange Server  
(2927022)  
(Kritisch)
</td>
</tr>
</table>
 
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

-   Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter.
-   Windows-Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager helfen Administratoren beim Verteilen von Sicherheitsupdates.
-   Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](https://technet.microsoft.com/de-de/security/cc297183). 

Danksagungen
------------

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

MS14-005

-   [FireEye, Inc.](https://www2.fireeye.com/) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in MSXML durch Offenlegung von Informationen (CVE-2014-0266).

MS14-007

-   [Omair](https://krash.in/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in der Microsoft Graphics-Komponente bezüglich Speicherbeschädigung (CVE-2014-0263).

MS14-009

-   James Forshaw von [Context Information Security](https://www.contextis.com/) für den Hinweis auf die Sicherheitsanfälligkeit durch Typüberquerung (CVE-2014-0257).

MS14-010

-   Liang Chen von [KeenTeam](https://www.k33nteam.org/) (@K33nTeam) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0267).
-   Code Audit Labs von [VulnHunt](https://www.vulnhunt.com/) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0267).
-   James Forshaw von [Context Information Security](https://www.contextis.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen (CVE-2014-0268).
-   Simon Zuckerbraun in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0269).
-   Jose A. Vazquez von Yenteasy -Security Research in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0270).
-   Jose A. Vazquez von Yenteasy –Security Research in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0270).
-   Bo Qu von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0272).
-   Bo Qu von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0273).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0274).
-   lokihardt@ASRT in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0274).
-   Simon Zuckerbraun in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0275).
-   Scott Bell von [Security-Assessment.com](https://www.security-assessment.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0276).
-   Scott Bell von [Security-Assessment.com](https://www.security-assessment.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0277).
-   Bo Qu von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0278).
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0278).
-   Scott Bell von [Security-Assessment.com](https://www.security-assessment.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0279).
-   Bo Qu von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0279).
-   Scott Bell von [Security-Assessment.com](https://www.security-assessment.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0280).
-   cons0ul und suto, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeiten, aber anonym bleiben möchten, für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0281).
-   Sachin Shinde für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0283).
-   Sachin Shinde für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0284).
-   Simon Zuckerbraun in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0285).
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0285).
-   Simon Zuckerbraun in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0286).
-   Peter ‘corelanc0d3 r‘ Van Eeckhoutte von [Corelan](https://www.corelangcv.com/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0287).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0288).
-   lokihardt@ASRT in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0289).
-   Bo Qu von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0290).
-   Zhibin Hu von [Qihoo](https://www.360.cn/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0290).
-   Yuki Chen von [Trend Micro](https://www.trendmicro.com/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-0290).
-   [Dieyu dieu deus deva divine dio theos dievas dewa ilu Diyin Ayóo Átʼéii atua tiānzhŭ Yahweh Zeus Odin El](https://dieyu.org/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer durch domänenübergreifende Offenlegung von Informationen (CVE-2014-0293).

Weitere Informationen:
----------------------

### Windows-Tool zum Entfernen schädlicher Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

### Sicherheitsstrategien und Community

Strategien für die Verwaltung von Sicherheitspatches:

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

Weitere Sicherheitsupdates

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086).

IT Pro Security Community:

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (11. Februar 2014): Bulletin Summary veröffentlicht.
-   V1.1 (12. Februar 2014): Für MS14-008 wurde die Bewertung der Ausnutzbarkeit für ältere Softwareversionen im **Ausnutzbarkeitsindex** für CVE-2014-0294 überarbeitet.
-   V1.2 (13. Februar 2014): Für MS14-011 wurde die Bewertung der Ausnutzbarkeit für ältere Softwareversionen im Ausnutzbarkeitsindex für CVE-2014-0271 überarbeitet.

*Seite am 23.04.2014 um 12:19Z-07:00 generiert.*
