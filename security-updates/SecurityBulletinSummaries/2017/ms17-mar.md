---
TOCTitle: 'MS17-MAR'
Title: Microsoft Security Bulletin Summary für März 2017
ms:assetid: 'ms17-mar'
ms:contentKeyID: 74430763
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms17-mar(v=Security.10)'
---

Microsoft Security Bulletin Summary für März 2017
=================================================

Veröffentlicht: 14. März 2017 | Aktualisiert: 8. August 2017

**Version:** 4.0

In diesem Bulletin Summary sind die im März 2017 veröffentlichten Sicherheitsbulletins aufgeführt.

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft-Sicherheitsbulletins finden Sie unter [Technische Sicherheitsbenachrichtigungen von Microsoft](https://go.microsoft.com/fwlink/?linkid=21163).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

Zur Erinnerung: Sicherheitsbulletins werden durch den [Leitfaden für Sicherheitsupdates](https://portal.msrc.microsoft.com/de-de/security-guidance) ersetzt. Details finden Sie in unserem Blogbeitrag [Furthering our commitment to security updates](https://blogs.technet.microsoft.com/msrc/2016/11/08/furthering-our-commitment-to-security-updates/).

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Sicherheitsbulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im nächsten Abschnitt **Betroffene Software**.

<p></p>
<table style="width:100%;">
<colgroup>
<col width="16%" />
<col width="16%" />
<col width="16%" />
<col width="16%" />
<col width="16%" />
<col width="16%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><strong>Titel des Bulletins und Kurzzusammenfassung</strong></td>
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads<br />
und Sicherheitsauswirkung</strong></td>
<td style="border:1px solid black;"><strong>Neustartanforderung</strong></td>
<td style="border:1px solid black;"><strong>Bekannte<br />
Probleme</strong></td>
<td style="border:1px solid black;"><strong>Betroffene Software</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842208">MS17-006</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (4013073)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Wenn der aktuelle Benutzer mit Administratorrechten angemeldet ist, kann ein Angreifer, der dieses Sicherheitsrisiko erfolgreich ausnutzt, Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842207">MS17-007</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Microsoft Edge (4013071)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Edge. Die Sicherheitsrisiken können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Microsoft Edge anzeigt. Ein Angreifer, der die Sicherheitsrisiken erfolgreich ausnutzt, könnte die Kontrolle über ein betroffenes System übernehmen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Edge</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842215">MS17-008</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows Hyper-V (4013082)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein authentifizierter Angreifer auf einem Gastbetriebssystem eine speziell gestaltete Anwendung ausführt, die bewirkt, dass das Betriebssystem des Hyper-V-Hosts beliebigen Code ausführt. Endbenutzer, die die Hyper-V-Rolle nicht aktiviert haben, sind nicht betroffen.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=839436">MS17-009</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek (4010319)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer speziell gestalteten PDF-Inhalt online anzeigt oder ein speziell gestaltetes PDF-Dokument öffnet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=843149">MS17-010</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows SMB-Server (4013389)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine Reihe speziell gestalteter Nachrichten an einen betroffenen Microsoft Server Message Block 1.0-Server (SMBv1) sendet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842211">MS17-011</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Uniscribe (4013076)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Windows Uniscribe. Die schwerwiegendsten dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Website besucht oder ein speziell gestaltetes Dokument öffnet. Für Benutzer mit Konten, die über weniger Systemrechte verfügen, kann dies geringere Auswirkungen haben als für Benutzer, die mit Administratorrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842212">MS17-012</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows (4013078)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete Anwendung ausführt, die sich mit einem iSNS-Server verbindet und anschließend bösartige Anforderungen an den Server sendet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842210">MS17-013</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft-Grafikkomponente (4013075)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows, Microsoft Office, Skype for Business, Microsoft Lync und Microsoft Silverlight. Die schwerwiegendsten dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Website besucht oder ein speziell gestaltetes Dokument öffnet. Für Benutzer mit Konten, die über weniger Systemrechte verfügen, kann dies geringere Auswirkungen haben als für Benutzer, die mit Administratorrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows<br />
Microsoft Office,<br />
Skype for Business,<br />
Microsoft Lync,<br />
Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842278">MS17-014</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Office (4013241)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Für Kunden, deren Konten mit weniger Benutzerrechten im System konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit Administratorrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Office-Dienste und Web Apps,<br />
Microsoft Server-Software,<br />
Microsoft Communications-Plattformen und -Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842279">MS17-015</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Exchange Server (4013242)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Exchange Outlook Web Access (OWA). Die Sicherheitsanfälligkeit kann Remotecodeausführung in Exchange Server ermöglichen, wenn ein Angreifer eine E-Mail mit einer speziell gestalteten Anlage an einen anfälligen Exchange-Server sendet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Exchange</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842209">MS17-016</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows IIS (4013074)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft-Internetinformationsdienste (IIS). Die Sicherheitsanfälligkeit kann Rechteerweiterungen ermöglichen, wenn ein Benutzer eine speziell gestaltete URL anklickt, die auf einem betroffenen Microsoft IIS-Server gehostet wird. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, könnte Skripte im Browser des Benutzers ausführen, um Informationen aus Websitzungen zu erhalten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842216">MS17-017</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows Kernel (4013081)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Rechteerweiterungen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anwendung ausführt.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=842217">MS17-018</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows-Kernelmodustreiber (4013083)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Rechteerweiterungen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt, die die Sicherheitsanfälligkeiten ausnutzen und die Kontrolle über ein betroffenes System übernehmen kann.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=839438">MS17-019</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Active Directory-Verbunddienste (4010320)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Active Directory-Verbunddienste (AD FS). Die Sicherheitsanfälligkeit kann die Offenlegung von Informationen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anforderung an einen AD FS-Server sendet, wodurch der Angreifer vertrauliche Informationen über das Zielsystem lesen kann.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=836272">MS17-020</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows DVD Maker (3208223)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit bezüglich der Offenlegung von Informationen in Windows DVD Maker. Aufgrund der Sicherheitsanfälligkeit kann ein Angreifer ggf. an Informationen gelangen, mit denen ein Zielsystem weiter geschädigt werden kann.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=839434">MS17-021</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows DirectShow (4010318)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Offenlegung von Informationen ermöglichen, wenn Windows DirectShow speziell gestaltete Medieninhalte öffnet, die auf einer schädlichen Website gehostet werden. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann in den Besitz von Informationen gelangen, mit denen ein Zielsystem weiter geschädigt werden kann.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=839435">MS17-022</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft XML Core Services (4010321)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Offenlegung von Informationen ermöglichen, wenn ein Benutzer eine schädliche Website besucht. Ein Angreifer kann einen Benutzer jedoch keinesfalls zum Klicken auf einen speziell gestalteten Link zwingen. Vielmehr muss ein Angreifer den Benutzer dazu verleiten, auf den Link zu klicken. Zu diesem Zweck wird der Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder einer Instant Messenger-Nachricht zu klicken.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=844066">MS17-023</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Adobe Flash Player (</strong>4014329)<br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Adobe Flash Player unter allen unterstützten Editionen von Windows 8.1, Windows Server 2012, Windows Server 2012 R2, Windows RT 8.1, Windows 10 und Windows Server 2016.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Adobe Flash Player</td>
</tr>
</tbody>
</table>
 

Ausnutzbarkeitsindex
--------------------

In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben wurden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID aufgeführt. Nur Sicherheitsanfälligkeiten mit einem Schweregrad von Kritisch oder Hoch in den Bulletins sind enthalten.

**Wie verwende ich diese Tabelle?**  

Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen nach der Veröffentlichung des Sicherheitsbulletins Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).

In den nachfolgenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;">
**CVE-ID**                    
</td>
<td style="border:1px solid black;">
**Titel der Sicherheitsanfälligkeit**
</td>
<td style="border:1px solid black;">
**Bewertung der Ausnutzbarkeit für  
aktuelle Softwareversionen**
</td>
<td style="border:1px solid black;">
**Bewertung der Ausnutzbarkeit für  
ältere Softwareversionen**
</td>
<td style="border:1px solid black;">
**Bewertung der Ausnutzbarkeit  
durch Denial-of-Service**
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-006: Kumulatives Sicherheitsupdate für Internet Explorer (4013073)**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0008](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0008)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0009](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0009)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser durch Offenlegung von Information
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0012](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0012)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Browser bezüglich Spoofingangriffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0018](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0018)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0033](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0033)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Browser bezüglich Spoofingangriffen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0037](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0037)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0040](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0040)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0049](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0049)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Skriptmodul bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0059](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0059)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0130](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0130)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0149](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0149)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
0 – Ausnutzung erkannt
</td>
<td style="border:1px solid black;">
0 – Ausnutzung erkannt
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0154](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0154)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-007: Kumulatives Sicherheitsupdate für Microsoft Edge (4013071)**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0009](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0009)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser durch Offenlegung von Information
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0010](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0010)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0011](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0011)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0012](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0012)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Browser bezüglich Spoofingangriffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0015](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0015)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0017](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0017)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0023](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0023)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft PDF bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0032](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0032)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0033](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0033)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Browser bezüglich Spoofingangriffen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0034](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0034)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0035](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0035)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0037](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0037)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0065](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser durch Offenlegung von Information
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0066](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0066)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Umgehung von Sicherheitsfunktionen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0067](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0067)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0068](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0068)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0069](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0069)
</td>
<td style="border:1px solid black;">
Spoofing-Sicherheitsanfälligkeit in Microsoft Edge
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0070](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0070)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0071](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0071)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0094](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0094)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0131](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0131)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0132](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0132)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0133](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0133)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0134](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0134)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0135](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0135)
</td>
<td style="border:1px solid black;">
Umgehung von Sicherheitsfunktionen in Microsoft Edge
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0136](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0136)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0137](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0137)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0138](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0138)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0140](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0140)
</td>
<td style="border:1px solid black;">
Umgehung von Sicherheitsfunktionen in Microsoft Edge
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0141](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0141)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0150](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0150)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0151](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0151)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Skriptmodul bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-008: Sicherheitsupdate für Windows Hyper-V (4013082)**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0021](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0021)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V vSMB bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0051](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0051)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Hyper-V-Netzwerkswitch bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0074](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0074)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0075](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0075)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0076](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0076)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0095](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0095)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V vSMB bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0096](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0096)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0097](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0097)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0098](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0098)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0099](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0099)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0109](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0109)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Hyper-V bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-009: Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek (4010319)**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0023](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0023)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft PDF bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-010: Sicherheitsupdate für Microsoft Windows SMB-Server (4013389)**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0143](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0143)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows SMB bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0144](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0144)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows SMB bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0145](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0145)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows SMB bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0146](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0146)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows SMB bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0147](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0147)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows SMB bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0148](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0148)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows SMB bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-011: Sicherheitsupdate für Microsoft Uniscribe (4013076)**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0072](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0072)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0083](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0083)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0084](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0084)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0085](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0085)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0086](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0086)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0087](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0087)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0088](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0088)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0089](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0089)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0090](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0090)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0091](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0091)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0092](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0092)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0111](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0111)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0112](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0112)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0113](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0113)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0114](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0114)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0115](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0115)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0116](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0116)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0117](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0117)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0118](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0118)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0119](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0119)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0120](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0120)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0121](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0121)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0122](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0122)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0123](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0123)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0124](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0124)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0125](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0125)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0126](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0125)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0127](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0127)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0128](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0128)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Uniscribe bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-012: Sicherheitsupdate für Microsoft Windows (4013078)**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0007](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0007)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Device Guard durch Umgehung von Sicherheitsfunktionen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0016](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0016)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in SMBv2/SMBv3 für Denial-of-Service-Angriffe (NULL-Dereferenzierung)
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0039](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0039)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows beim Laden von DLL-Dateien bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0057](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0057)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows DNS-Abfrage bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0100](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0100)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows HelpPane bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0104](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0104)
</td>
<td style="border:1px solid black;">
Sicherheitsrisiko im iSNS-Server bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-013: Sicherheitsupdate für Microsoft-Grafikkomponente (4013075)**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0001](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0001)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bei der Windows-GDI bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0005](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0005)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bei der Windows-GDI bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
0 – Ausnutzung erkannt
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0014](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0014)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in GDI+ bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0025](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0025)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bei der Windows-GDI bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0038](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0038)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows-Grafikkomponente bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0047](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0047)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bei der Windows-GDI bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0060](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0060)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in GDI+ bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0061](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0061)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in der Microsoft-Farbverwaltung bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0062](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0062)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in GDI+ bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0063](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0063)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in der Microsoft-Farbverwaltung bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0073](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0073)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows-GDI+ bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0108](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0108)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows-Grafikkomponente bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-014: Sicherheitsupdate für Microsoft Office (4013241)**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0006](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0006)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0019](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0019)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0020](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0020)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0027](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0027)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit durch Offenlegung von Informationen in Microsoft Office
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0029](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0029)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0030](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0030)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0031](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0031)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0052](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0052)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0053](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0053)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0105](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0105)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit durch Offenlegung von Informationen in Microsoft Office
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0107](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0107)
</td>
<td style="border:1px solid black;">
Microsoft SharePoint-Sicherheitsanfälligkeit bezüglich XSS
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0129](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0129)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Lync für Mac bezüglich Zertifikatüberprüfung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-015: Sicherheitsupdate für Microsoft Exchange Server (4013242)**](https://go.microsoft.com/fwlink/?linkid=842279)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0110](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0110)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Exchange Server bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-016: Sicherheitsupdate für Windows IIS (4013074)**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0055](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0055)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft IIS Server XSS bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-017: Sicherheitsupdate für Windows Kernel (4013081)**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0050](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0050)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bezüglich Rechteerweiterungen im Windows-Kernel
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0101](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0101)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0102](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0102)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0103](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0103)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows-Registrierung bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-018: Sicherheitsupdate für Windows-Kernelmodustreiber (4013083)**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0024](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0024)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0026](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0026)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0056](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0056)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0078](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0078)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0079](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0079)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0080](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0080)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0081](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0081)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0082](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0082)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-019: Sicherheitsupdate für Active Directory-Verbunddienste (4010320)**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0043](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0043)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Active Directory-Verbunddiensten bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Vorläufig
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-020: Sicherheitsupdate für Windows DVD Maker (3208223)**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0045](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0045)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows DVD Maker durch Fälschung siteübergreifender Anforderungen
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-021: Sicherheitsupdate für Windows DirectShow (4010318)**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0042](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0042)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows DirectShow bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-022: Sicherheitsupdate für Microsoft XML Core Services (4010321)**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0022](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0022)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft XML Core Services bezüglich Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
0 – Ausnutzung erkannt
</td>
<td style="border:1px solid black;">
0 – Ausnutzung erkannt
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-023: Sicherheitsupdate für Adobe Flash Player (4014329)**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[APSB17-07](https://helpx.adobe.com/de/security/products/flash-player/apsb17-07.html)
</td>
<td style="border:1px solid black;">
Die Bewertung des Schweregrads und der Updatepriorität finden Sie im Adobe-Sicherheitsbulletin [APSB17-07](https://helpx.adobe.com/de/security/products/flash-player/apsb17-07.html).
</td>
<td style="border:1px solid black;">
---------
</td>
<td style="border:1px solid black;">
---------
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 

Betroffene Software
-------------------

In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.

In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.

**Hinweis** Für ein Sicherheitsrisiko müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.

### Windows-Betriebssysteme und Komponenten (Tabelle 1 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9   
(4012204)  
(Kritisch)  
Microsoft Internet Messaging API  
(3218362)  
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
Windows Vista Service Pack 2  
(4012598)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(4012583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3217587)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(4017018)  
(Kritisch)  
Windows Vista Service Pack 2  
(4012584)  
(Hoch)  
Windows Vista Service Pack 2  
(4012497)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9   
(4012204)  
(Kritisch)  
Microsoft Internet Messaging API  
(3218362)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3211306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(4012598)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(4012583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3217587)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(4017018)  
(Kritisch)  
Windows Vista x64 Edition Service Pack 2  
(4012584)  
(Hoch)  
Windows Vista x64 Edition Service Pack 2  
(4012497)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9   
(4012204)  
(Mittel)  
Microsoft Internet Messaging API  
(3218362)  
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4012598)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4012583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3217587)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4012021)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4017018)  
(Kritisch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4012584)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4012497)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9   
(4012204)  
(Mittel)  
Microsoft Internet Messaging API  
(3218362)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3211306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4012598)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4012583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3217587)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4012021)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4017018)  
(Kritisch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4012584)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4012497)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
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
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4012598)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4012583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3217587)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4017018)  
(Kritisch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4012584)  
(Hoch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4012497)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012204)  
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
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012215)  
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
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012204)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012204)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012215)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
Nur Sicherheit
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
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
Monatlicher Rollup
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
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012204)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012204)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(4012204)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows-Server 2012  
(4012214)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(4012217)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows-Server 2012  
(4012217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012204)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012216)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025338)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4012606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025338)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4013198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025344)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4013198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025344)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1703 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025342)  
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
Windows 10 Version 1703 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4025342)  
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
<td style="border:1px solid black;" colspan="9">
**Windows Server 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(4013429)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(4013429)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-006**](https://go.microsoft.com/fwlink/?linkid=842208)
</td>
<td style="border:1px solid black;">
[**MS17-007**](https://go.microsoft.com/fwlink/?linkid=842207)
</td>
<td style="border:1px solid black;">
[**MS17-008**](https://go.microsoft.com/fwlink/?linkid=842215)
</td>
<td style="border:1px solid black;">
[**MS17-009**](https://go.microsoft.com/fwlink/?linkid=839436)
</td>
<td style="border:1px solid black;">
[**MS17-010**](https://go.microsoft.com/fwlink/?linkid=843149)
</td>
<td style="border:1px solid black;">
[**MS17-011**](https://go.microsoft.com/fwlink/?linkid=842211)
</td>
<td style="border:1px solid black;">
[**MS17-012**](https://go.microsoft.com/fwlink/?linkid=842212)
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4012598)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4012583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3217587)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4017018)  
(Kritisch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4012584)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4012497)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3211306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4012598)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4012583)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3217587)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4017018)  
(Kritisch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4012584)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4012497)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweis zu MS17-013**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Informationen zu zusätzlich betroffener Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Windows-Betriebssysteme und -Komponenten (Tabelle 2 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(4012373)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(4011981)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(4012497)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3205715)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3214051)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(3216916)  
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
Windows Vista x64 Edition Service Pack 2  
(4012373)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(4011981)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(4012497)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3205715)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3214051)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(3216916)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4012373)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4011981)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(4012497)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3217882)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3214051)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(3216916)  
(Hoch)
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4012373)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4011981)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(4012497)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3217882)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3214051)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(3216916)  
(Hoch)
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
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4012373)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4011981)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(4012497)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3217882)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3214051)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(3216916)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4015548)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(4015551)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012606)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4013198)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1703 für 32-Bit-Systeme
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
Windows 10 Version 1703 für x64-basierte Systeme
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
<td style="border:1px solid black;" colspan="9">
**Windows Server 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(4014329)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-016**](https://go.microsoft.com/fwlink/?linkid=842209)
</td>
<td style="border:1px solid black;">
[**MS17-017**](https://go.microsoft.com/fwlink/?linkid=842216)
</td>
<td style="border:1px solid black;">
[**MS17-018**](https://go.microsoft.com/fwlink/?linkid=842217)
</td>
<td style="border:1px solid black;">
[**MS17-019**](https://go.microsoft.com/fwlink/?linkid=839438)
</td>
<td style="border:1px solid black;">
[**MS17-020**](https://go.microsoft.com/fwlink/?linkid=836272)
</td>
<td style="border:1px solid black;">
[**MS17-021**](https://go.microsoft.com/fwlink/?linkid=839434)
</td>
<td style="border:1px solid black;">
[**MS17-022**](https://go.microsoft.com/fwlink/?linkid=839435)
</td>
<td style="border:1px solid black;">
[**MS17-023**](https://go.microsoft.com/fwlink/?linkid=844066)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4012373)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4011981)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(4012497)  
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
Microsoft XML Core Services 3.0  
(3216916)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4012373)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4011981)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(4012497)  
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
Microsoft XML Core Services 3.0  
(3216916)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012212)  
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
Microsoft XML Core Services 3.0  
(4012212)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(4012215)  
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
Microsoft XML Core Services 3.0  
(4012215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
)(4012217)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012213)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4012216)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2016 für x64-basierte Systeme  
(Server Core-Installation)  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0  
(4013429)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
 

### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(3127945)  
(Kritisch)  
Microsoft Office 2007 Service Pack 3  
(3141535)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2007 Service Pack 3  
(3178676)  
(Hoch)  
Microsoft Word 2007 Service Pack 3  
(3178683)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(3127958)  
(Kritisch)  
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(3178688)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(3178686)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(3178690)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(3178687)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3127958)  
(Kritisch)  
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3178688)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3178686)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(3178690)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(3178687)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 Service Pack 1 (32-Bit-Editionen)  
(3172542)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (32-Bit-Editionen)  
(3172464)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 Service Pack 1 (64-Bit-Editionen)  
(3172542)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (64-Bit-Editionen)  
(3172464)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2013 RT**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 RT Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 RT Service Pack 1  
(3172542)  
(Hoch)  
Microsoft Word 2013 RT Service Pack 1  
(3172464)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (32-Bit-Edition)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2016 (32-Bit-Edition)  
(3178673)  
(Hoch)  
Microsoft Word 2016 (32-Bit-Edition)  
(3178674)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Edition)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2016 (64-Bit-Edition)  
(3178673)  
(Hoch)  
Microsoft Word 2016 (64-Bit-Edition)  
(3178674)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office für Mac 2011**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel für Mac 2011  
(3198809)  
(Hoch)  
Microsoft Excel für Mac 2011  
(3212218)  
(Hoch)  
Microsoft Word für Mac 2011  
(3198809)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2016 für Mac**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Office 2016 für Mac  
(Hoch)  
Microsoft Excel 2016 für Mac  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Weitere Office-Software**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(3178677)  
(Hoch)  
Microsoft Office Compatibility Pack Service Pack 3  
(3178682)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel Viewer  
(3178680)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(3178693)  
(Kritisch)  
Microsoft Word Viewer  
(3178653)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(3178694)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS17-013 und MS17-014**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Informationen zu zusätzlich betroffener Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Microsoft Office-Dienste und Web Apps

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft SharePoint Server 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Excel Services (32-Bit-Edition)  
(3178678)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Excel Services (64-Bit-Edition)  
(3178678)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft SharePoint Server 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Excel Services  
(3178685)  
(Hoch)  
Word Automation Services  
(3178684)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft SharePoint Server 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Excel Services  
(3172431)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office Web Apps 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2  
(3178689)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office Web Apps 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2013 Service Pack 1  
(3172457)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS17-014**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Informationen zu zusätzlich betroffener Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft SharePoint Foundation 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
<td style="border:1px solid black;">
[**MS17-015**](https://go.microsoft.com/fwlink/?linkid=842279)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2013 Service Pack 1  
(3172540)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Exchange Server 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
<td style="border:1px solid black;">
[**MS17-015**](https://go.microsoft.com/fwlink/?linkid=842279)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Service Pack 1  
(4012178)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 14
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 14  
(4012178)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Exchange Server 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
<td style="border:1px solid black;">
[**MS17-015**](https://go.microsoft.com/fwlink/?linkid=842279)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2016 Kumulatives Update 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2016 Kumulatives Update 3  
(4012178)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS17-014 und MS17-015**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Informationen zu zusätzlich betroffener Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Microsoft Communications-Plattformen und -Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="3">
**Skype for Business 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Skype for Business 2016 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Skype for Business 2016 (32-Bit-Editionen)  
(3178656)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Skype for Business Basic 2016 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Skype for Business Basic 2016 (32-Bit-Editionen)  
(3178656)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Skype for Business 2016 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Skype for Business 2016 (64-Bit-Editionen)  
(3178656)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Skype for Business Basic 2016 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Skype for Business Basic 2016 (64-Bit-Editionen)  
(3178656)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Lync 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (32-Bit)  
(Skype for Business)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (32-Bit)  
(Skype for Business)  
(3172539)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (32-Bit)  
(Skype for Business Basic)
</td>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (32-Bit)  
(Skype for Business Basic)  
(3172539)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (64-Bit)  
(Skype for Business)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (64-Bit)  
(Skype for Business)  
(3172539)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (64-Bit)  
(Skype for Business Basic)
</td>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (64-Bit)  
(Skype for Business Basic)  
(3172539)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Lync 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 (32 Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 (32-Bit)  
(4010299)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64-Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64-Bit)  
(4010299)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Benutzerebene)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Benutzerebene)  
(4010300)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Administratorebene)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Administratorebene)  
(4010301)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Live Meeting 2007-Konsole**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Live Meeting 2007-Konsole
</td>
<td style="border:1px solid black;">
Microsoft Live Meeting 2007-Konsole  
(4010303)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Live Meeting 2007-Add-In**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Live Meeting 2007-Add-In
</td>
<td style="border:1px solid black;">
Microsoft Live Meeting 2007-Add-In  
(4010304)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Lync für Mac**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
<td style="border:1px solid black;">
[**MS17-014**](https://go.microsoft.com/fwlink/?linkid=842278)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync für Mac 2011
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Lync für Mac 2011  
(4012487)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS17-013 und MS17-014**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Informationen zu zusätzlich betroffener Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Silverlight**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-013**](https://go.microsoft.com/fwlink/?linkid=842210)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients
</td>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(4013867)  
**(**Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients
</td>
<td style="border:1px solid black;">
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(4013867)  
**(**Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern
</td>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(4013867)  
**(**Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern
</td>
<td style="border:1px solid black;">
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(4013867)  
**(**Kritisch)
</td>
</tr>
</table>
 
**Hinweis zu MS17-013**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Informationen zu zusätzlich betroffener Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter.

Windows Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager erleichtern Administratoren die Verteilung von Sicherheitsupdates.

Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](https://technet.microsoft.com/de-de/security/cc297183). 

Danksagungen
------------

Microsoft würdigt die Bemühungen derjenigen Benutzer der Sicherheitscommunity, die uns dabei helfen, Kunden durch eine verantwortungsbewusste Offenlegung von Sicherheitslücken zu schützen. Weitere Informationen finden Sie unter [Danksagung](https://technet.microsoft.com/de-de/library/security/mt745121.aspx).

Weitere Informationen
---------------------

### Microsoft Windows-Tool zum Entfernen bösartiger Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen von Sicherheitsbulletins ist keine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software erhältlich.

### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/de-de/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/wsus/bb456965). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Anbietern von Sicherheitssoftware vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsrisiken dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

### Sicherheitsstrategien und Community

**Updateverwaltungsstrategien**

Auf der Seite [Update Management](https://go.microsoft.com/fwlink/?linkid=21168) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsanfälligkeiten sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=21129) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/de-de/kb/913086).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie in der [IT-Pro Security Community](https://go.microsoft.com/fwlink/?linkid=21164) mit anderen IT-Profis über das Thema Sicherheit.

### Support

Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://go.microsoft.com/fwlink/?linkid=21742), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.

Sicherheitslösungen für IT-Experten: [TechNet Security – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)

So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Safety and Security Center](https://support.microsoft.com/de-de/contactus/cu_sc_virsec_master)

Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/de-de/common/international.aspx)

### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleichgültig, ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann die Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (14. März 2017): Bulletin Summary veröffentlicht.
-   V2.0 (11. April 2017): Bulletin Summary wurde überarbeitet, um die folgenden Updates anzukündigen:
    -   Für MS17-013 die Veröffentlichung des Updates 4017018 für Windows Vista und Windows Server 2008. Dieses Update ersetzt Update 4012583 nur für CVE-2017-0038, um die Sicherheitsanfälligkeit umfassend zu beheben. Microsoft empfiehlt Kunden, die die betroffene Software verwenden, das Sicherheitsupdate zu installieren, um vollständig vor der in diesem Bulletin beschriebenen Sicherheitsanfälligkeit geschützt zu sein. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 4017018](https://support.microsoft.com/de-de/kb/4017018).
    -   Für MS17-014 veröffentlicht Microsoft für eine umfassende Behebung von CVE-2017-0027 nur für Office für Mac 2011 das Sicherheitsupdate 3212218. Microsoft empfiehlt Kunden, die Office für Mac 2011 verwenden, das Update 3212218 zu installieren, um vor dieser Sicherheitsanfälligkeit vollständig geschützt zu sein. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 3212218](https://support.microsoft.com/de-de/kb/3212218).
    -   Für MS17-021 sind Sicherheitsupdates im Zusammenhang mit CVE-2017-0042 für Windows Server 2012 nun verfügbar. Kunden mit Windows Server 2012 sollten das Update 4015548 (Nur Sicherheit) oder 4015551 (Monatlicher Rollup) installieren, um vor dieser Sicherheitsanfälligkeit vollständig geschützt zu sein. Für Kunden mit anderen Microsoft Windows-Versionen besteht kein Handlungsbedarf.
-   V2.1 (14. April 2017) CVE-2017-0022 wurde überarbeitet, um den Ausnutzbarkeitsindex auf „0 – Ausnutzung erkannt“ zu aktualisieren. Diese Änderung dient lediglich zur Information.
-   V3.0 (9. Mai 2017): Für MS17-013 hat Microsoft das Sicherheitsupdate 4017018 für betroffene Editionen von Windows Server 2008 erneut veröffentlicht. In diesem Zusammenhang wurde es als Sicherheitsupdate neu klassifiziert. Microsoft empfiehlt Kunden, das Update 4017018 zu installieren, um vor CVE-2017-0038 vollständig geschützt zu sein. Kunden, die das Update bereits installiert haben, müssen keine weiteren Maßnahmen ergreifen.
-   V4.0 (8. August 2017): Damit MS17-007 die Sicherheitsanfälligkeit CVE-2017-0071 umfassend behebt, hat Microsoft die Sicherheitsupdates vom Juli für alle Versionen von Windows 10 veröffentlicht. Beachten Sie, dass Windows 10 für 32-Bit-Systeme, Windows 10 für x64-basierte Systeme, Windows 10 Version 1703 für 32-Bit-Systeme und Windows 10 Version 1703 für x64-basierte Systeme zur Tabelle „Betroffene Produkte“ hinzugefügt wurden, da sie ebenfalls von dieser Sicherheitsanfälligkeit betroffen sind. Microsoft empfiehlt Kunden, soweit noch nicht geschehen, die Sicherheitsupdates vom Juli 2017 zu installieren, um vor dieser Sicherheitsanfälligkeit vollständig geschützt zu sein.

*Seite generiert am 02.08.2017 um 12:34-07:00.*