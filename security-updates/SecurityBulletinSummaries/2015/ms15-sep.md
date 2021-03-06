---
TOCTitle: 'MS15-SEP'
Title: Microsoft Security Bulletin Summary für September 2015
ms:assetid: 'ms15-sep'
ms:contentKeyID: 69932941
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms15-sep(v=Security.10)'
---

Microsoft Security Bulletin Summary für September 2015
======================================================

Veröffentlicht: 8. September 2015 | Aktualisiert: 10. November 2015

**Version:** 4.0

In diesem Bulletin Summary sind die im September 2015 veröffentlichten Security Bulletins aufgeführt.

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Security Bulletins für diesen Monat nach Schweregrad geordnet.

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
und Auswirkung der Sicherheitsanfälligkeit</strong></td>
<td style="border:1px solid black;"><strong>Neustartanforderung</strong></td>
<td style="border:1px solid black;"><strong>Bekannte<br />
Probleme</strong></td>
<td style="border:1px solid black;"><strong>Betroffene Software</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (3089548)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-095">MS15-095</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Microsoft Edge (3089665) <br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Edge. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Microsoft Edge anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Microsoft Edge</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-096">MS15-096</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory-Dienst kann Denial-of-Service ermöglichen (3072595)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Active Directory. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein authentifizierter Angreifer mehrere Computerkonten erstellt. Um die Sicherheitsanfälligkeit ausnutzen zu können, muss ein Angreifer ein Konto mit Berechtigungen haben, die ihm das Hinzufügen von Computern zur Domäne gestatten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Graphics-Komponente können Remotecodeausführung ermöglichen (3089656)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows, Microsoft Office und Microsoft Lync. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer ein speziell gestaltetes Dokument öffnet oder eine nicht vertrauenswürdige Website besucht, in das bzw. die OpenType-Schriftartdateien eingebettet sind.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3086255">3086255</a><br />
<a href="https://support.microsoft.com/de-de/kb/3099414">3099414</a></td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Microsoft Office, <br />
Microsoft Lync</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-098">MS15-098</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Journal können Remotecodeausführung ermöglichen (3089669)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Das schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Journaldatei öffnet. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-099">MS15-099</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (3089664)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office, <br />
Microsoft SharePoint Foundation</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-100">MS15-100</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Media Center kann Remotecodeausführung ermöglichen (3087918) <br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn in Windows Media Center eine speziell gestaltete Media Center-Linkdatei (MCL) geöffnet wird, die auf schädlichen Code verweist. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-101">MS15-101</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in .NET Framework können Erhöhung von Berechtigungen ermöglichen (3089662) <br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft .NET Framework. Die schwerste dieser Sicherheitsanfälligkeiten kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer ein speziell gestaltete .NET-Anwendung ausführt. Ein Angreifer kann Benutzer jedoch keinesfalls zum Ausführen einer solchen Anwendung zwingen. Ein Angreifer muss Benutzer vielmehr dazu verleiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Kein Neustart erforderlich.</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-102">MS15-102</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Task Management kann Erhöhung von Berechtigungen ermöglichen (3089657)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-103">MS15-103</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Exchange Server können Offenlegung von Informationen ermöglichen (3089250)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Exchange Server. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann die Offenlegung von Information ermöglichen, wenn Outlook Web Access (OWA) Webanforderungen nicht ordnungsgemäß verarbeitet und Benutzereingaben und E-Mail-Inhalte nicht ordnungsgemäß bereinigt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Exchange Server</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-104">MS15-104</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Skype for Business Server und Lync Server können Erhöhung von Berechtigungen ermöglichen (3089952)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Skype for Business Server und Microsoft Lync Server. Die schwerste Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer auf eine speziell gestaltete URL klickt. Ein Angreifer muss die Benutzer dazu verleiten, auf einen Link in einer Instant Messenger oder E-Mail-Nachricht zu klicken, der die Benutzer über eine speziell gestaltete URL zu einer betroffenen Website führt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Kein Neustart erforderlich.</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3080353">3080353</a></td>
<td style="border:1px solid black;">Skype for Business Server, <br />
Microsoft Lync Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-105">MS15-105</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Hyper-V kann Umgehung von Sicherheitsfunktionen ermöglichen (3091287)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Umgehung von Sicherheitsfunktionen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anwendung ausführt, die bewirkt, dass Windows Hyper-V falsche Konfigurationseinstellungen für die Zugriffsteuerungsliste anwendet. Endbenutzer, die die Hyper-V-Rolle nicht aktiviert haben, sind nicht betroffen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Umgehung von Sicherheitsfunktionen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Im Ausnutzbarkeitsindex sind nur Sicherheitsanfälligkeiten enthalten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
In den nachfolgenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.
 
<p> </p>
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
<td style="border:1px solid black;"><strong>Titel der Sicherheitsanfälligkeit</strong></td>
<td style="border:1px solid black;"><strong>CVE-ID</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für<br />
aktuelle Softwareversion</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für<br />
ältere Softwareversionen</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit<br />
durch Denial-of-Service</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2483">CVE-2015-2483</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Manipulationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2484">CVE-2015-2484</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2485">CVE-2015-2485</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2486">CVE-2015-2486</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2487">CVE-2015-2487</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2489">CVE-2015-2489</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2490">CVE-2015-2490</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2491">CVE-2015-2491</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2492">CVE-2015-2492</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Skriptmodul bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2493">CVE-2015-2493</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2494">CVE-2015-2494</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2498">CVE-2015-2498</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2499">CVE-2015-2499</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2500">CVE-2015-2500</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2501">CVE-2015-2501</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2541">CVE-2015-2541</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-094">MS15-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2542">CVE-2015-2542</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-095">MS15-095</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2485">CVE-2015-2485</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-095">MS15-095</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2486">CVE-2015-2486</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-095">MS15-095</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2494">CVE-2015-2494</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-095">MS15-095</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2542">CVE-2015-2542</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-096">MS15-096</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Active Directory bezüglich Denial-of-Service</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2535">CVE-2015-2535</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit beim Analysieren von OpenType-Schriftarten</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2506">CVE-2015-2506</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Schriftartentreiber bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2507">CVE-2015-2507</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Schriftartentreiber bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2508">CVE-2015-2508</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Vorläufig</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Grafikkomponente bezüglich Pufferüberlaufs</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2510">CVE-2015-2510</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2511">CVE-2015-2511</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Schriftartentreiber bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2512">CVE-2015-2512</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2517">CVE-2015-2517</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2518">CVE-2015-2518</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2527">CVE-2015-2527</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Kernel durch Umgehung der ASLR-Sicherheitsfunktion</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2529">CVE-2015-2529</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-097">MS15-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2546">CVE-2015-2546</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">0 – Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-098">MS15-098</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2513">CVE-2015-2513</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-098">MS15-098</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Denial-of-Service</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2514">CVE-2015-2514</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-098">MS15-098</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Denial-of-Service</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2516">CVE-2015-2516</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-098">MS15-098</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung durch Ganzzahlüberlauf</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2519">CVE-2015-2519</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-098">MS15-098</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2530">CVE-2015-2530</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-099">MS15-099</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2520">CVE-2015-2520</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-099">MS15-099</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2521">CVE-2015-2521</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-099">MS15-099</a></td>
<td style="border:1px solid black;">Spoofing-Sicherheitsanfälligkeit in Microsoft SharePoint durch siteübergreifende Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2522">CVE-2015-2522</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-099">MS15-099</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2523">CVE-2015-2523</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-099">MS15-099</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich fehlerhafter EPS-Datei</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2545">CVE-2015-2545</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">0 – Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-100">MS15-100</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Media Player bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2509">CVE-2015-2509</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-101">MS15-101</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2504">CVE-2015-2504</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-101">MS15-101</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MVC durch Denial-of-Service</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2526">CVE-2015-2526</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-102">MS15-102</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Task Management bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2524">CVE-2015-2524</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-102">MS15-102</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bei Dateilöschung in Windows-Aufgabenplanung bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2525">CVE-2015-2525</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-102">MS15-102</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Task Management bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2528">CVE-2015-2528</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-103">MS15-103</a></td>
<td style="border:1px solid black;">Exchange-Sicherheitsanfälligkeit durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2505">CVE-2015-2505</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-103">MS15-103</a></td>
<td style="border:1px solid black;">Spoofing-Sicherheitsanfälligkeit in Exchange</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2543">CVE-2015-2543</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-103">MS15-103</a></td>
<td style="border:1px solid black;">Spoofing-Sicherheitsanfälligkeit in Exchange</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2544">CVE-2015-2544</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-104">MS15-104</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Skype for Business Server und Lync Server bezüglich Offenlegung von Informationen durch siteübergreifende Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2531">CVE-2015-2531</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-104">MS15-104</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Lync Server bezüglich Offenlegung von Informationen durch siteübergreifende Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2532">CVE-2015-2532</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-104">MS15-104</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Skype for Business Server und Lync Server bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2536">CVE-2015-2536</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-105">MS15-105</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Hyper-V durch Umgehung von Sicherheitsfunktionen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2534">CVE-2015-2534</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
</tbody>
</table>
  
Betroffene Software  
-------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.
  
**Hinweis** Für eine Sicherheitsanfälligkeit müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
### Windows-Betriebssysteme und Komponenten (Tabelle 1 von 2)

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
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
</td>
</tr>
<tr>
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3087038)  
(Kritisch)  
Internet Explorer 8  
(3087038)  
(Kritisch)  
Internet Explorer 9  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3087039)  
(Hoch)  
Windows Vista Service Pack 2  
(3087135)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3087038)  
(Kritisch)  
Internet Explorer 8  
(3087038)  
(Kritisch)  
Internet Explorer 9  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3087039)  
(Hoch)  
Windows Vista x64 Edition Service Pack 2  
(3087135)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3069114)  
(Kritisch)
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
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3087038)  
(Mittel)  
Internet Explorer 8  
(3087038)  
(Mittel)  
Internet Explorer 9  
(3087038)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3087039)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3087135)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3087038)  
(Mittel)  
Internet Explorer 8  
(3087038)  
(Mittel)  
Internet Explorer 9  
(3087038)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3087039)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3087135)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3087038)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3087039)  
(Hoch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3087135)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
</td>
</tr>
<tr>
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3087038)  
(Kritisch)  
Internet Explorer 9  
(3087038)  
(Kritisch)  
Internet Explorer 10  
(3087038)  
(Kritisch)  
Internet Explorer 11  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3087038)  
(Kritisch)  
Internet Explorer 9  
(3087038)  
(Kritisch)  
Internet Explorer 10  
(3087038)  
(Kritisch)  
Internet Explorer 11  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3087038)  
(Mittel)  
Internet Explorer 9  
(3087038)  
(Mittel)  
Internet Explorer 10  
(3087038)  
(Mittel)  
Internet Explorer 11  
(3087038)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3087038)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
</td>
</tr>
<tr>
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3087038)  
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
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3069114)  
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
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3087038)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3087038)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
</td>
</tr>
<tr>
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3087038)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3087038)  
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
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3069114)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
</td>
</tr>
<tr>
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3081455)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3081455)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3081455)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3081455)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3081455)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3081455)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3081455)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3081455)  
(Kritisch)
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
[**MS15-094**](https://technet.microsoft.com/de-de/library/security/ms15-094)
</td>
<td style="border:1px solid black;">
[**MS15-095**](https://technet.microsoft.com/de-de/library/security/ms15-095)
</td>
<td style="border:1px solid black;">
[**MS15-096**](https://technet.microsoft.com/de-de/library/security/ms15-096)
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-098**](https://technet.microsoft.com/de-de/library/security/ms15-098)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3087039)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3087135)  
(Kritisch)
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3087039)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3087135)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3087039)  
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
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3072595)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3087039)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis zu MS15-097**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

### Windows-Betriebssysteme und Komponenten (Tabelle 2 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3074541)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3084135)  
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
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3074541)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3074541)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3084135)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3074541)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3084135)  
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
Microsoft .NET Framework 2,0 Service Pack 2  
(3074541)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3074543)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3084135)  
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
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3074543)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3074543)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3084135)  
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
Microsoft .NET Framework 3.5.1  
(3074543)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074544)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074229)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074549)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074552)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3082089)  
(Hoch)  
Windows 8 für 32-Bit-Systeme  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074544)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074229)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074549)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074552)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3082089)  
(Hoch)  
Windows 8 für x64-basierte Systeme  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074545)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074548)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074228)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074553)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074232)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3082089)  
(Hoch)  
Windows 8.1 für 32-Bit-Systeme  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows Media Center  
(3087918)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074545)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074548)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074228)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074553)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074232)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3082089)  
(Hoch)  
Windows 8.1 für x64-basierte Systeme  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3087088)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074544)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074229)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074549)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074552)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3082089)  
(Hoch)  
Windows Server 2012  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074545)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074548)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074228)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074553)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074232)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3082089)  
(Hoch)  
Windows Server 2012 R2  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3087088)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows RT
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074229)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074549)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074231)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074552)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3082089)  
(Hoch)  
Windows RT  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.1/4.5.2  
(3074548)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074228)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074232)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074553)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3082089)  
(Hoch)  
Windows RT 8.1  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
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
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3081455)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3081455)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3081455)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3081455)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3081455)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3081455)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3081455)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="5">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-100**](https://technet.microsoft.com/de-de/library/security/ms15-100)
</td>
<td style="border:1px solid black;">
[**MS15-101**](https://technet.microsoft.com/de-de/library/security/ms15-101)
</td>
<td style="border:1px solid black;">
[**MS15-102**](https://technet.microsoft.com/de-de/library/security/ms15-102)
</td>
<td style="border:1px solid black;">
[**MS15-105**](https://technet.microsoft.com/de-de/library/security/ms15-105)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3084135)  
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3084135)  
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
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3074543)  
(Hoch)  
Microsoft .NET Framework 4  
(3074547)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074550)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074230)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074554)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3084135)  
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
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074544)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074229)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3074549)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074552)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
(3082089)  
(Hoch)  
Windows Server 2012  
(Server Core-Installation)  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3074545)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074548)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3074228)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074553)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3074232)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3082089)  
(Hoch)  
Windows Server 2012 R2  
(Server Core-Installation)  
(3084135)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3087088)  
(Hoch)
</td>
</tr>
</table>
 
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
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
</td>
<td style="border:1px solid black;">
[**MS15-103**](https://technet.microsoft.com/de-de/library/security/ms15-103)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft SharePoint Foundation 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2013 Service Pack 1  
(3085501)  
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
Microsoft Exchange Server 2013
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 8  
(3089250)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 9  
(3089250)  
(Hoch)
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
Microsoft Exchange Server 2013 Service Pack 1  
(3089250)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-099**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

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
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(3085546)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(3085620)  
(Kritisch)  
Microsoft Excel 2007 Service Pack 3  
(3085543)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(3085529)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(3085560)  
(Kritisch)  
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(3085526)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3085529)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3085560)  
(Kritisch)  
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(3085526)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)  
(3085572)  
(Kritisch)  
Microsoft Excel 2013 Service Pack 1 (32-Bit-Editionen)  
(3085502)  
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
Microsoft Office Service Pack 1 (64-Bit-Editionen)  
(3085572)  
(Kritisch)  
Microsoft Excel 2013 Service Pack 1 (64-Bit-Editionen)  
(3085502)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2013 RT**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Microsoft Office 2013 RT Service Pack 1 (32-Bit-Editionen)  
(3085572)  
(Kritisch)  
Microsoft Excel 2013 RT Service Pack 1  
(3085502)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Office 2016 (32-Bit-Editionen)  
(3085635)  
(Kritisch)  
Microsoft Excel 2016 (32-Bit-Editionen)  
(2920693)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Editionen)  
(3085635)  
(Kritisch)  
Microsoft Excel 2016 (64-Bit-Editionen)  
(2920693)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office für Mac**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Microsoft Excel für Mac 2011  
(3088501)  
(Hoch)
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
Microsoft Excel 2016 für Mac  
(3088502)  
Hoch 
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
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-099**](https://technet.microsoft.com/de-de/library/security/ms15-099)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3054993)  
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
(3054995)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-097 und MS15-099**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

### Microsoft Communications-Plattformen und -Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Live Meeting 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-104**](https://technet.microsoft.com/de-de/library/security/ms15-104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3081090)  
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
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-104**](https://technet.microsoft.com/de-de/library/security/ms15-104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Microsoft Lync 2010 (32 Bit)  
(3081087)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64 Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64 Bit)  
(3081087)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Benutzerebene)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Benutzerebene)  
(3081088)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Administratorebene)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee  
(Installation auf Administratorebene)  
(3081089)  
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
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-104**](https://technet.microsoft.com/de-de/library/security/ms15-104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3085500)  
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
(3085500)  
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
(3085500)  
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
(3085500)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
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
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-104**](https://technet.microsoft.com/de-de/library/security/ms15-104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Skype for Business 2016 (32 Bit)
</td>
<td style="border:1px solid black;">
Skype for Business 2016 (32 Bit)  
(2910994)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Skype for Business 2016 (64 Bit)
</td>
<td style="border:1px solid black;">
Skype for Business 2016 (64 Bit)  
(2910994)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Lync Server 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-104**](https://technet.microsoft.com/de-de/library/security/ms15-104)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync Server 2013  
(Webkomponentenserver)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Lync Server 2013  
(Webkomponentenserver)  
(3080353)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Skype for Business Server 2015**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-097**](https://technet.microsoft.com/de-de/library/security/ms15-097)
</td>
<td style="border:1px solid black;">
[**MS15-104**](https://technet.microsoft.com/de-de/library/security/ms15-104)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Skype for Business Server 2015
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Skype for Business Server 2015  
(3061064)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-097**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

Tools und Hinweise zur Erkennung und Bereitstellung von Sicherheitsupdates
--------------------------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter.

Windows Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager erleichtern Administratoren die Verteilung von Sicherheitsupdates.

Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](https://technet.microsoft.com/de-de/security/cc297183).

Danksagung
----------

Microsoft würdigt die Bemühungen derjenigen Benutzer der Sicherheitscommunity, die uns dabei helfen, Kunden durch eine verantwortliche Offenlegung von Sicherheitsanfälligkeiten zu schützen. Weitere Informationen finden Sie unter [Danksagung](https://technet.microsoft.com/de-de/library/security/dn903755.aspx). 

Weitere Informationen
---------------------

### Microsoft Windows-Tool zum Entfernen bösartiger Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/de-de/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://technet.microsoft.com/de-de/security/dn467918) aufgeführt sind.

### Sicherheitsstrategien und Community

**Updateverwaltungsstrategien**

Auf der Seite [Patchmanagement](https://technet.microsoft.com/de-de/library/bb466251.aspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsanfälligkeiten sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/de-de/kb/913086).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

### Support

Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/lifecycle/?ln=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.

Sicherheitslösungen für IT-Experten: [TechNet Security – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)

Hilfe beim Schützen des Computers, auf dem Windows ausgeführt wird, vor Viren und Schadsoftware: [Safety and Security Center](https://www.microsoft.com/de-de/security/default.aspx)

Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx?ln=de)

### Haftungsausschluss

Die Informationen in der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (8. September 2015): Bulletin Summary veröffentlicht.
-   V1.1 (8. September 2015): In MS15-097 wurde die Bewertung der Ausnutzbarkeit im Ausnutzbarkeitsindex für CVE-2015-2506 überarbeitet. Dies ist lediglich eine Informationsänderung.
-   V1.2 (9. September 2015): In MS15-097 wurde die Bewertung der Ausnutzbarkeit im Ausnutzbarkeitsindex für CVE-2015-2546 überarbeitet, und in MS15-099 wurde die Bewertung der Ausnutzbarkeit im Ausnutzbarkeitsindex für CVE-2015-2545 überarbeitet. Dies sind lediglich Informationsänderungen.
-   V1.3 (23. September 2015): Das Bulletin Summary wurde überarbeitet, um den Titel von CVE-2015-2514 im Ausnutzbarkeitsindex zu korrigieren. Dies ist lediglich eine Informationsänderung. Kunden, die das Update, das die Sicherheitsanfälligkeit behebt, bereits erfolgreich installiert haben, müssen nichts weiter unternehmen.
-   V1.4 (25. September 2015): In MS15-099 wurde das Update 3088502 für Microsoft Office 2016 für Mac hinzugefügt, das ab dem 15. September 2015 verfügbar ist. Weitere Informationen finden Sie in [Microsoft Knowledge Base-Artikel 3088502](https://support.microsoft.com/de-de/kb/3088502).
-   V2.0 (30. September 2015): Bulletin Summary überarbeitet, um die Verfügbarkeit der Updatepakete für Microsoft Office 2016 in MS15-097 und Skype for Business 2016 in MS15-099 bekannt zu geben. Kunden, die Microsoft Office 2016 oder Skype for Business 2016 ausführen, sollten die betreffenden Updates installieren, um vor den in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten geschützt zu sein. Die meisten Kunden haben automatische Updates aktiviert und müssen nichts weiter tun, weil die betreffenden Updates automatisch heruntergeladen und installiert werden.
-   V3.0 (13. Oktober 2015): Für MS15-099 wurde das Bulletin Summary überarbeitet, um die Verfügbarkeit der Updatepakete für Microsoft Excel 2016 bekannt zu geben. Kunden, die Microsoft Excel 2016 ausführen, sollten das Update 2920693 installieren, um vor den in MS15-099 beschriebenen Sicherheitsanfälligkeiten geschützt zu sein. Die meisten Kunden haben automatische Updates aktiviert und müssen nichts weiter tun, weil das Update automatisch heruntergeladen und installiert wird.
-   V4.0 (10. November 2015): Damit MS15-099 die Sicherheitsanfälligkeit CVE-2015-2545 umfassend behebt, hat Microsoft die Sicherheitsupdates für die betroffene Microsoft Office-Software erneut veröffentlicht. Benutzer, die die betroffene Microsoft Office-Software ausführen, sollten die mit diesem überarbeiteten Bulletin veröffentlichten Sicherheitsupdates installieren, um vor dieser Sicherheitsanfälligkeit geschützt zu sein. Für Benutzer, die andere Microsoft Office-Software ausführen, besteht kein Handlungsbedarf. Downloadlinks finden Sie in [MS15-099](https://technet.microsoft.com/de-de/library/security/ms15-099) und weitere Informationen im [Microsoft Knowledge Base-Artikel 3089664](https://support.microsoft.com/de-de/kb/3089664).

*Seite generiert am 02.11.2015 um 16:26-08:00.*