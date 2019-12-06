---
TOCTitle: 'MS16-SEP'
Title: Microsoft Security Bulletin Summary für September 2016
ms:assetid: 'ms16-sep'
ms:contentKeyID: 73895977
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms16-sep(v=Security.10)'
---

Microsoft Security Bulletin Summary für September 2016
======================================================

Veröffentlicht: 13. September 2016 | Aktualisiert: 11. Juli 2017

**Version:** 2.0

In diesem Bulletin Summary sind die im September 2016 veröffentlichten Sicherheitsbulletins aufgeführt.

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft-Sicherheitsbulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://go.microsoft.com/fwlink/?linkid=21163).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Sicherheitsbulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im Abschnitt **Betroffene Software**.

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=823624">MS16-104</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (3183038)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Wenn der aktuelle Benutzer mit Administratorrechten angemeldet ist, kann ein Angreifer die Kontrolle über ein betroffenes System übernehmen. Der Angreifer könnte dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit uneingeschränkten Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3185319">3185319</a></td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=823625">MS16-105</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Microsoft Edge (3183043)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Edge. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Microsoft Edge anzeigt. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für jene, die mit Administratorrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Edge</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=824814">MS16-106</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft-Grafikkomponente (3185848)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell entworfene Website besucht oder ein speziell entworfenes Dokument öffnet. Benutzer, deren Konten mit weniger Rechten auf dem System konfiguriert sind, können davon möglicherweise weniger betroffen sein als Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=824817">MS16-107</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Office (3185852)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell entworfene Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit Administratorrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Office-Dienste und Web Apps</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=824829">MS16-108</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Exchange Server (3185883)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Exchange Server. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung in einigen Oracle Outside In-Bibliotheken zulassen, die in Exchange Server integriert sind, wenn ein Angreifer eine E-Mail mit einer speziell entworfenen Anlage an einen anfälligen Exchange-Server sendet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Exchange</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=824768">MS16-109</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Silverlight (3182373)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Silverlight. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine manipulierte Website besucht, die eine speziell gestaltete Silverlight-Anwendung enthält. Ein Angreifer kann einen Benutzer nicht zum Besuch einer manipulierten Website zwingen. Stattdessen muss er den Benutzer zum Besuch dieser Webseite verleiten. Zu diesem Zweck wird der Benutzer normalerweise dazu gebracht, in einer E-Mail oder Sofortnachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Kein Neustart erforderlich.</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=821596">MS16-110</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows (3178467)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung zulassen, wenn ein Angreifer eine speziell gestaltete Anforderung erstellt und auf einem Zielsystem beliebigen Code mit den entsprechenden Berechtigungen ausführt.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3187754">3187754</a></td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=825142">MS16-111</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows Kernel (3186973)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Rechteerweiterungen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anwendung auf einem Zielsystem ausführt.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a><br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3175024">3175024</a></td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=821605">MS16-112</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows-Sperrbildschirm (3178469)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Diese Sicherheitsanfälligkeit kann Rechteerweiterungen ermöglichen, wenn Windows fälschlicherweise zulässt, dass Webinhalte vom Windows-Sperrbildschirm geladen werden.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a><br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=824825">MS16-113</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für sicheren Windows-Kernelmodus (3185876)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann zu einer Offenlegung von Informationen führen, wenn der sichere Windows-Kernelmodus Objekte im Arbeitsspeicher nicht ordnungsgemäß verarbeitet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=824826">MS16-114</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für SMBv1-Server (3185879)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Unter den Betriebssystemen Windows Vista, Windows Server 2008, Windows 7 und Windows Server 2008 R2 kann die Sicherheitsanfälligkeit Remotecodeausführung ermöglichen, wenn ein authentifizierter Angreifer speziell entworfene Pakete an einen betroffenen Microsoft Server Message Block 1.0 (SMBv1)-Server sendet. Die Sicherheitsanfälligkeit wirkt sich nicht auf andere SMB-Server-Versionen aus. Obwohl neuere Betriebssysteme betroffen sind, ist die potenzielle Auswirkung Denial-of-Service.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=825727">MS16-115</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek (3188733)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können die Offenlegung von Informationen ermöglichen, wenn ein Benutzer speziell gestalteten PDF-Inhalt online anzeigt oder ein speziell gestaltetes PDF-Dokument öffnet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=825725">MS16-116</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate in OLE-Automatisierung für VBScript-Skriptmodul (3188724)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer eines betroffenen Systems erfolgreich dazu verleitet, eine schädliche oder manipulierte Website zu besuchen. Beachten Sie, dass Sie zwei Updates installieren müssen, um vor der in diesem Bulletin beschriebenen Sicherheitsanfälligkeit geschützt zu sein: Das Update in diesem Bulletin (MS16-116) und das Update in <a href="https://go.microsoft.com/fwlink/?linkid=823624">MS16-104</a>.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows<br />
</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=825603">MS16-117</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Adobe Flash Player (3188128)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Adobe Flash Player bei der Installation unter allen unterstützten Editionen von Windows 8.1, Windows Server 2012, Windows Server 2012 R2, Windows RT 8.1 und Windows 10.</td>
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
[**MS16-104: Kumulatives Sicherheitsupdate für Internet Explorer (3183038)**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3247](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3247)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
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
[CVE-2016-3291](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3291)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser durch Offenlegung von Information
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
[CVE-2016-3292](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3292)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Browser bezüglich Rechteerweiterungen
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
[CVE-2016-3295](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3295)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
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
[CVE-2016-3297](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3297)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
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
[CVE-2016-3324](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3324)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
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
[CVE-2016-3325](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3325)
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
[CVE-2016-3351](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3351)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser durch Offenlegung von Information
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
[CVE-2016-3353](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3353)
</td>
<td style="border:1px solid black;">
Umgehung von Sicherheitsfunktionen in Internet Explorer
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
[CVE-2016-3375](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3375)
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
<td style="border:1px solid black;" colspan="5">
[**MS16-105: Kumulatives Sicherheitsupdate für Microsoft Edge (3183043)**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3247](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3247)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
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
[CVE-2016-3291](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3291)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser durch Offenlegung von Information
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
[CVE-2016-3294](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3294)
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
[CVE-2016-3295](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3295)
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
[CVE-2016-3297](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3297)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
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
[CVE-2016-3325](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3325)
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
[CVE-2016-3330](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3330)
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
[CVE-2016-3350](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3350)
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
[CVE-2016-3351](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3351)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser durch Offenlegung von Information
</td>
<td style="border:1px solid black;">
0 – Ausnutzung erkannt
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
[CVE-2016-3370](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3370)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in PDF-Bibliothek bezüglich der Offenlegung von Informationen
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
[CVE-2016-3374](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3374)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in PDF-Bibliothek bezüglich der Offenlegung von Informationen
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
[CVE-2016-3377](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3377)
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
[**MS16-106: Sicherheitsupdate für Microsoft-Grafikkomponente (3185848)**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3348](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3348)
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
[CVE-2016-3349](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3349)
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
[CVE-2016-3354](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3354)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in GDI bezüglich der Offenlegung von Informationen
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
[CVE-2016-3355](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3355)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in GDI bezüglich Rechteerweiterungen
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
[CVE-2016-3356](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3356)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in GDI bezüglich Remotecodeausführung
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
<td style="border:1px solid black;" colspan="5">
[**MS16-107: Sicherheitsupdate für Microsoft Office (3185852)**](https://go.microsoft.com/fwlink/?linkid=824817)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0137](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0137)
</td>
<td style="border:1px solid black;">
ASLR-Umgehung durch Microsoft APP-V
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
[CVE-2016-0141](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0141)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Software bezüglich der Offenlegung von Informationen
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
[CVE-2016-3357](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3357)
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
[CVE-2016-3358](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3358)
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
[CVE-2016-3359](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3359)
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
[CVE-2016-3360](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3360)
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
[CVE-2016-3361](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3361)
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
[CVE-2016-3362](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3362)
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
[CVE-2016-3363](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3363)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[CVE-2016-3364](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3364)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[CVE-2016-3365](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3365)
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
[CVE-2016-3366](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3366)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Spoofingangriffen
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
[CVE-2016-3381](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3381)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[**MS16-108: Sicherheitsupdate für Microsoft Exchange Server (3185883)**](https://go.microsoft.com/fwlink/?linkid=824829)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0138](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0138)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Exchange durch Offenlegung von Information
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
[CVE-2016-3378](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3378)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Exchange durch offene Umleitung
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
[CVE-2016-3379](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3379)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Exchange bezüglich Rechteerweiterungen
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
<td style="border:1px solid black;" colspan="5">
[**MS16-109: Sicherheitsupdate für Silverlight (3182373)**](https://go.microsoft.com/fwlink/?linkid=824768)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3367](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3367)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Silverlight bezüglich Speicherbeschädigung
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
[**MS16-110: Sicherheitsupdate für Windows (3178467)**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3346](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3346)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit beim Erzwingen von Berechtigungen in Windows bezüglich Rechteerweiterungen
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
[CVE-2016-3352](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3352)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Software bezüglich der Offenlegung von Informationen
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
[CVE-2016-3368](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3368)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows bezüglich Remotecodeausführung
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
[CVE-2016-3369](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3369)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows bezüglich Denial-of-Service
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS16-111: Sicherheitsupdate für Windows Kernel (3186973)**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3305](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3305)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Windows-Sitzungsobjekt bezüglich Rechteerweiterungen
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
[CVE-2016-3306](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3306)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Windows-Sitzungsobjekt bezüglich Rechteerweiterungen
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
[CVE-2016-3371](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3371)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bezüglich Rechteerweiterungen im Windows-Kernel
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
[CVE-2016-3372](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3372)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bezüglich Rechteerweiterungen im Windows-Kernel
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
[CVE-2016-3373](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3373)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bezüglich Rechteerweiterungen im Windows-Kernel
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
[**MS16-112: Sicherheitsupdate für Windows-Sperrbildschirm (3178469)**](https://go.microsoft.com/fwlink/?linkid=821605)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3302](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3302)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Windows-Sperrbildschirm bezüglich Rechteerweiterungen
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
[**MS16-113: Sicherheitsupdate für den sicheren Windows-Kernelmodus (3185876)**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3344](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3344)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im sicheren Windows-Kernelmodus bezüglich der Offenlegung von Informationen
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
<td style="border:1px solid black;" colspan="5">
[**MS16-114: Sicherheitsupdate für SMBv1-Server (3185879)**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3345](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3345)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows SMB bezüglich authentifizierter Remotecodeausführung
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
<td style="border:1px solid black;" colspan="5">
[**MS16-115: Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek (3188733)**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3370](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3370)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in PDF-Bibliothek bezüglich der Offenlegung von Informationen
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
[CVE-2016-3374](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3374)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in PDF-Bibliothek bezüglich der Offenlegung von Informationen
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
[**MS16-116: Sicherheitsupdate in OLE-Automatisierung für VBScript-Skriptmodul (3188724)**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-3375](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-3375)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Skriptmodul bezüglich Offenlegung von Informationen
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
[**MS16-117: Sicherheitsupdate für Adobe Flash Player (3188128)**](https://go.microsoft.com/fwlink/?linkid=825603)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[APSB16-29](https://helpx.adobe.com/de/security/products/flash-player/apsb16-29.html)
</td>
<td style="border:1px solid black;">
Die Bewertungen des Schweregrads und der Updatepriorität finden Sie unter [APSB16-29](https://helpx.adobe.com/de/security/products/flash-player/apsb16-29.html).
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
</table>
 

 Betroffene Software
--------------------

In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.

In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.

**Hinweis** Für ein Sicherheitsrisiko müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.

 

### Windows-Betriebssysteme und -Komponenten (Tabelle 1 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
Internet Explorer 9   
(3185319)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3175024)  
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
Internet Explorer 9   
(3185319)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9   
(3185319)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3175024)  
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
Internet Explorer 9   
(3185319)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3175024)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3175024)  
(Hoch)
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
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185319)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar                   
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3175024)  
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
Internet Explorer 11  
(3185319)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3175024)  
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
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185319)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3175024)  
(Hoch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185319)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3184471)  
(Hoch)  
Windows 8.1 für 32-Bit-Systeme  
(3187754)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3178539)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185319)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3184471)  
(Hoch)  
Windows 8.1 für x64-basierte Systeme  
(3187754)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3178539)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3185319)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185319)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3178539)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185319)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3184471)  
(Hoch)  
Windows RT 8.1  
(3187754)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3178539)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3185611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3185611)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3185611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185614)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3185614)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3185614)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3185614)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3189866)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3189866)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3189866)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(3189866)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(3189866)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3189866)  
(Hoch)
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
Windows 10 Version 1703 für 32-Bit-Systeme  
(4025342)  
(Hoch)
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
Windows 10 Version 1703 für x64-basierte Systeme  
(4025342)  
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
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-104**](https://go.microsoft.com/fwlink/?linkid=823624)
</td>
<td style="border:1px solid black;">
[**MS16-105**](https://go.microsoft.com/fwlink/?linkid=823625)
</td>
<td style="border:1px solid black;">
[**MS16-106**](https://go.microsoft.com/fwlink/?linkid=824814)
</td>
<td style="border:1px solid black;">
[**MS16-110**](https://go.microsoft.com/fwlink/?linkid=821596)
</td>
<td style="border:1px solid black;">
[**MS16-111**](https://go.microsoft.com/fwlink/?linkid=825142)
</td>
<td style="border:1px solid black;">
[**MS16-112**](https://go.microsoft.com/fwlink/?linkid=821605)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3175024)  
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
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3175024)  
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
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3185911)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3184471)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3175024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3178539)  
(Hoch)
</td>
</tr>
</table>
 
 

### Windows-Betriebssysteme und -Komponenten (Tabelle 2 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
<td style="border:1px solid black;">
**Keine**
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
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3184122)  
(Kritisch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3184122)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3184122)  
(Mittel)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3184122)  
(Mittel)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
<td style="border:1px solid black;">
**Keine**
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
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3184122)  
(Kritisch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3184122)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3184122)  
(Mittel)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3184943)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3184122)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3184943)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3184122)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
<td style="border:1px solid black;">
[**Hoch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3184943)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3188128)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3184943)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3188128)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3184943)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3184122)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
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
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3185611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3185611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3185614)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3185614)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3189866)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme  
(3188128)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(3185614)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(3189866)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(3189866)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme  
(3188128)  
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
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-113**](https://go.microsoft.com/fwlink/?linkid=824825)
</td>
<td style="border:1px solid black;">
[**MS16-114**](https://go.microsoft.com/fwlink/?linkid=824826)
</td>
<td style="border:1px solid black;">
[**MS16-115**](https://go.microsoft.com/fwlink/?linkid=825727)
</td>
<td style="border:1px solid black;">
[**MS16-116**](https://go.microsoft.com/fwlink/?linkid=825725)
</td>
<td style="border:1px solid black;">
[**MS16-117**](https://go.microsoft.com/fwlink/?linkid=825603)
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
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3184122)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3177186)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3184122)  
(Mittel)
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
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(3118300)  
(Kritisch)  
Microsoft Excel 2007 Service Pack 3  
(3115459)  
(Hoch)  
Microsoft Outlook 2007  
(3118303)  
(Hoch)  
Microsoft PowerPoint 2007 Service Pack 3  
(3114744)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(3118309)  
(Kritisch)  
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2553432)  
(Kritisch)  
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(3118316)  
(Hoch)  
Microsoft Outlook 2010 Service Pack 2 (32-Bit-Editionen)  
(3118313)  
(Hoch)  
Microsoft PowerPoint 2010 Service Pack 2 (32-Bit-Editionen)  
(3115467)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3118309)  
(Kritisch)  
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2553432)  
(Kritisch)  
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(3118316)  
(Hoch)  
Microsoft Outlook 2010 Service Pack 2 (64-Bit-Editionen)  
(3118313)  
(Hoch)  
Microsoft PowerPoint 2010 Service Pack 2 (64-Bit-Editionen)  
(3115467)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)  
(3118268)  
(Kritisch)  
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)<sup>[1]</sup>
(Hoch)  
Microsoft Excel 2013 Service Pack 1 (32-Bit-Editionen)  
(3118284)  
(Hoch)  
Microsoft Outlook 2013 Service Pack 1 (32-Bit-Editionen)  
(3118280)  
(Hoch)  
Microsoft PowerPoint 2013 Service Pack 1 (32-Bit-Editionen)  
(3115487)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)  
(3118268)  
(Kritisch)  
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)<sup>[1]</sup>
(Hoch)  
Microsoft Excel 2013 Service Pack 1 (64-Bit-Editionen)  
(3118284)  
(Hoch)  
Microsoft Outlook 2013 Service Pack 1 (64-Bit-Editionen)  
(3118280)  
(Hoch)  
Microsoft PowerPoint 2013 Service Pack 1 (64-Bit-Editionen)  
(3115487)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2013 RT**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office 2013 RT Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 RT Service Pack 1  
(3118268)  
(Kritisch)  
Microsoft Excel 2013 RT Service Pack 1  
(3118284)  
(Hoch)  
Microsoft Outlook 2013 RT Service Pack 1  
(3118280)  
(Hoch)  
Microsoft PowerPoint 2013 RT Service Pack 1  
(3115487)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office 2016 (32-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Office 2016 (32-Bit-Edition)<sup>[1]</sup>
Microsoft Office 2016 (32-Bit-Edition)  
(3118292)  
(Kritisch)  
Microsoft Excel 2016 (32-Bit-Edition)  
(3118290)  
(Hoch)  
Microsoft Outlook 2016 (32-Bit-Edition)  
(3118293)  
(Hoch)  
Microsoft Visio 2016 (32-Bit-Editionen)  
(Hoch)<sup>[1]</sup>
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Edition)<sup>[1]</sup>
Microsoft Office 2016 (64-Bit-Edition)  
(3118292)  
(Kritisch)  
Microsoft Excel 2016 (64-Bit-Edition)  
(3118290)  
(Hoch)  
Microsoft Outlook 2016 (64-Bit-Edition)  
(3118293)  
(Hoch)  
Microsoft Visio 2016 (64-Bit-Editionen)  
(Hoch)<sup>[1]</sup>
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office für Mac 2011**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Microsoft Word für Mac 2011  
(3186805)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2016 für Mac**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office 2016 für Mac
</td>
<td style="border:1px solid black;">
Microsoft Excel 2016 für Mac  
(3186807)  
(Hoch)  
Microsoft PowerPoint 2016 für Mac  
(3186807)  
(Hoch)  
Microsoft Word 2016 für Mac  
(3186807)  
(Kritisch)  
Microsoft Outlook 2016 für Mac  
(3186807)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Weitere Office-Software**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2597974)  
(Hoch)  
Microsoft Office Compatibility Pack Service Pack 3  
(3115462)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
Microsoft Excel Viewer  
(3115463)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Microsoft PowerPoint Viewer  
(3054969)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(3118297)  
(Kritisch)
</td>
</tr>
</table>
 
<sup>[1]</sup>Dieser Eintrag bezieht sich nur auf die Klick-und-Los (C2R)-Version.

 

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
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Excel Services  
(3115112)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Excel Services  
(3115112)  
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
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Excel Services  
(3115119)  
(Hoch)  
Word Automation Services  
(3115466)  
(Kritisch)
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
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft SharePoint Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013 Service Pack 1  
(3054862)  
(Kritisch)  
Excel Automation Services  
(3115169)  
(Kritisch)  
Word Automation Services  
(3115443)  
(Kritisch)
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
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office Web Apps 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2  
(3115472)  
(Kritisch)
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
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Microsoft Office Web Apps Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2013 Service Pack 1  
(3118270)  
(Kritisch)
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
[**MS16-107**](https://go.microsoft.com/fwlink/?linkid=824817)
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
Office Online Server
</td>
<td style="border:1px solid black;">
Office Online Server  
(3118299)  
(Hoch)
</td>
</tr>
</table>
 
 

### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Exchange Server 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-108**](https://go.microsoft.com/fwlink/?linkid=824829)
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
Microsoft Exchange Server 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007 Service Pack 3  
(3184711)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Exchange Server 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-108**](https://go.microsoft.com/fwlink/?linkid=824829)
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
Microsoft Exchange Server 2010 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2010 Service Pack 3  
(3184728)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Exchange Server 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-108**](https://go.microsoft.com/fwlink/?linkid=824829)
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
Microsoft Exchange Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Service Pack 1  
(3184736)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 12
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 12  
(3184736)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 13
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 13  
(3184736)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Exchange Server 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-108**](https://go.microsoft.com/fwlink/?linkid=824829)
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
Microsoft Exchange Server 2016 Kumulatives Update 1
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2016 Kumulatives Update 1  
(3184736)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2016 Kumulatives Update 2
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2016 Kumulatives Update 2  
(3184736)  
(Hoch)
</td>
</tr>
</table>
 
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
[**MS16-109**](https://go.microsoft.com/fwlink/?linkid=824768)
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
Microsoft Silverlight 5
</td>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation auf dem Mac  
(3182373)  
(Hoch)  
Microsoft Silverlight 5 Developer Runtime bei Installation auf dem Mac  
(3182373)  
(Hoch)  
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(3182373)  
(Hoch)  
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(3182373)  
(Hoch)  
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(3182373)  
(Hoch)
</td>
</tr>
</table>
 
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter.

Windows Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager erleichtern Administratoren die Verteilung von Sicherheitsupdates.

Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](https://technet.microsoft.com/de-de/security/cc297183). 

Danksagung
----------

Microsoft erkennt die Bemühungen der Mitglieder der Sicherheitscommunity an, die uns durch die verantwortungsvolle Offenlegung.von Sicherheitsanfälligkeiten helfen, unsere Kunden zu schützen. Weitere Informationen finden Sie unter [Danksagung](https://technet.microsoft.com/de-de/library/security/mt674627.aspx).

Weitere Informationen
---------------------

### Microsoft Windows-Tool zum Entfernen bösartiger Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen von Sicherheitsbulletins ist keine aktualisierte Version des Microsoft Windows-Tools zum Entfernen schädlicher Software erhältlich.

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

Die Informationen in der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleichgültig, ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann die Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 ([13. September 2016](https://technet.microsoft.com/de-DE/library/bulletin+summary_publisheddate(v=Security.10))): Bulletin Summary veröffentlicht.
-   V2.0 (11. Juli 2017): Für MS16-111 wurden Windows 10 Version 1703 für 32-Bit-Systeme und Windows 10 Version 1703 für x64-basierte Systeme zur Tabelle „Betroffene Software“ hinzugefügt, da diese Versionen von CVE-2016-3305 betroffen sind. Microsoft empfiehlt Kunden, die Windows 10 Version 1703 verwenden, das Update 4025342 zu installieren, um vor dieser Sicherheitsanfälligkeit geschützt zu sein.

*Seite generiert am 03.07.2017 um 16:05-07:00.*
