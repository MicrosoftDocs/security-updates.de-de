---
TOCTitle: 'MS15-MAY'
Title: Microsoft Security Bulletin Summary für Mai 2015
ms:assetid: 'ms15-may'
ms:contentKeyID: 65633513
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms15-may(v=Security.10)'
---

Microsoft Security Bulletin Summary für Mai 2015
================================================

Veröffentlicht: 12. Mai 2015

**Version:** 1.0

In diesem Bulletin Summary sind die im Mai 2015 veröffentlichten Security Bulletins aufgeführt.

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://technet.microsoft.com/de-de/security/dd252948.aspx).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Security Bulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im nächsten Abschnitt **Betroffene Software**.

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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (3049563)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-044">MS15-044</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Microsoft-Schriftartentreiber können Remotecodeausführung ermöglichen (3057110)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows, Microsoft .NET Framework, Microsoft Office, Microsoft Lync und Microsoft Silverlight. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer ein speziell gestaltetes Dokument öffnet oder eine nicht vertrauenswürdige Website besucht, in das bzw. die TrueType-Schriftartdateien eingebettet sind.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3057110">3057110</a></td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework,<br />
Microsoft Office,<br />
Microsoft Lync,<br />
Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-045">MS15-045</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Journal kann Remotecodeausführung ermöglichen (3046002)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsrisiken können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Journaldatei öffnet. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-046">MS15-046</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (3057181)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-047">MS15-047</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft SharePoint Server können Remotecodeausführung ermöglichen (3058083)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office-Serversoftware. Diese Sicherheitsrisiken können Remotecodeausführung ermöglichen, wenn ein authentifizierter Angreifer speziell gestaltete Seiteninhalte an einen SharePoint-Zielserver sendet. Ein Angreifer, der diese Sicherheitsrisiken erfolgreich ausnutzt, kann beliebigen Code im Sicherheitskontext des W3WP-Dienstkontos auf der Ziel-SharePoint-Website ausführen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Server-Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-048">MS15-048</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in .NET Framework können Erhöhung von Berechtigungen ermöglichen (3057134)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft .NET Framework. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer eine speziell gestaltete, teilweise vertrauenswürdige Anwendung installiert.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-049">MS15-049</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Silverlight kann Erhöhung von Berechtigungen ermöglichen (3058985)</strong><br />
Dieses Sicherheitsupdate behebt ein Sicherheitsrisiko in Microsoft Silverlight. Das Sicherheitsrisiko kann Erhöhung von Berechtigungen ermöglichen, wenn eine speziell gestaltete Silverlight-Anwendung auf einem betroffenen System ausgeführt wird. Um diese Sicherheitsanfälligkeit auszunutzen, muss sich der Angreifer zunächst beim System anmelden oder einen angemeldeten Benutzer dazu verleiten, eine speziell gestaltete Anwendung auszuführen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Kein Neustart erforderlich.</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Silverlight</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-050">MS15-050</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Dienststeuerungs-Manager kann Erhöhung von Berechtigungen ermöglichen (3055642)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit im Windows Dienststeuerungs-Manager, die dadurch verursacht wird, dass der Dienststeuerungs-Manager Identitätswechselebenen nicht ordnungsgemäß überprüft. Die Sicherheitsanfälligkeit kann Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer zunächst beim System anmeldet und eine speziell gestaltete Anwendung ausführt, die auf Erhöhung von Berechtigungen ausgelegt ist.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-051">MS15-051</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Erhöhung von Berechtigungen ermöglichen (3057191)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Das schwerwiegendste dieser Sicherheitsrisiken kann Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem lokalen System anmeldet und beliebigen Code im Kernelmodus ausführt. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Ein Angreifer muss über gültige Anmeldeinformationen verfügen und sich lokal anmelden können, um dieses Sicherheitsrisiko ausnutzen zu können. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-052">MS15-052</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Kernel kann Umgehung von Sicherheitsfunktionen ermöglichen (3050514)</strong><br />
Dieses Sicherheitsupdate behebt ein Sicherheitsrisiko in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Umgehung von Sicherheitsfunktionen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Umgehung von Sicherheitsfunktionen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3050514">3050514</a></td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-053">MS15-053</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in JScript- und VBScript-Skriptmodulen können Umgehung von Sicherheitsfunktionen ermöglichen (3057263)<br />
</strong>Dieses Sicherheitsupdate behebt die Umgehung der ASLR-Sicherheitsfunktion in den JScript- und VBScript-Skriptmodulen in Microsoft Windows. Ein Angreifer kann eine dieser ASLR-Umgehungen in Verbindung mit einer anderen Sicherheitsanfälligkeit verwenden, etwa eine Sicherheitsanfälligkeit bezüglich Remotecodeausführung, um zuverlässiger beliebigen Code auf dem Zielsystem auszuführen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Umgehung von Sicherheitsfunktionen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-054">MS15-054</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Dateiformat von Microsoft Management Console (MMC) kann Denial-of-Service ermöglichen (3051768)</strong><br />
Dieses Sicherheitsupdate behebt ein Sicherheitsrisiko in Microsoft Windows. Die Sicherheitsanfälligkeit kann einen Denial-of-Service-Angriff ermöglichen, wenn ein nicht authentifizierter Remoteangreifer einen Benutzer dazu verleitet, eine Freigabe zu öffnen, die eine speziell gestaltete MSC-Datei enthält. Ein Angreifer kann den Benutzer jedoch nicht zum Besuch der Freigabe oder Anzeigen der Datei zwingen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-055">MS15-055</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Schannel kann Offenlegung von Informationen ermöglichen (3061518)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Offenlegung von Informationen ermöglichen, wenn Secure Channel (Schannel) in einer verschlüsselten TLS-Sitzung die Verwendung einer schwachen DHE-Schlüssellänge (Diffie-Hellman Ephemeral) von 512 Bits zulässt. Durch 512-Bit-DHE-Schlüssel wird der DHE-Schlüsselaustausch schwach und für verschiedene Angriffe anfällig. Damit ein Angriff erfolgreich sein kann, muss der Server die DHE-Schlüssellänge von 512 Bit unterstützen. In der Standardkonfiguration von Windows-Servern ist die kleinste zulässige DHE-Schlüssellänge 1024 Bit.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3061518">3061518</a></td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Im Ausnutzbarkeitsindex sind nur Sicherheitsanfälligkeiten enthalten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259).
  
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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1658">CVE-2015-1658</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">ASLR-Umgehung durch VBScript</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1684">CVE-2015-1684</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">ASLR-Umgehung durch Internet Explorer</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1685">CVE-2015-1685</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">ASLR-Umgehung durch VBScript und JScript</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1686">CVE-2015-1686</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1688">CVE-2015-1688</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1689">CVE-2015-1689</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1691">CVE-2015-1691</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer kann Offenlegung von Informationen der Zwischenablage ermöglichen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1692">CVE-2015-1692</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1694">CVE-2015-1694</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1703">CVE-2015-1703</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1704">CVE-2015-1704</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1705">CVE-2015-1705</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1706">CVE-2015-1706</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1708">CVE-2015-1708</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1709">CVE-2015-1709</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1710">CVE-2015-1710</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1711">CVE-2015-1711</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1712">CVE-2015-1712</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1713">CVE-2015-1713</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1714">CVE-2015-1714</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1717">CVE-2015-1717</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-043">MS15-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1718">CVE-2015-1718</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-044">MS15-044</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit beim Analysieren von OpenType-Schriftarten</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1670">CVE-2015-1670</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-044">MS15-044</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bei der Analyse von TrueType-Schriftarten</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1671">CVE-2015-1671</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-045">MS15-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1675">CVE-2015-1675</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-045">MS15-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1695">CVE-2015-1695</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-045">MS15-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1696">CVE-2015-1696</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-045">MS15-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1697">CVE-2015-1697</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-045">MS15-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1698">CVE-2015-1698</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-045">MS15-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Journal bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1699">CVE-2015-1699</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-046">MS15-046</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1682">CVE-2015-1682</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-046">MS15-046</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1683">CVE-2015-1683</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-047">MS15-047</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft SharePoint-Seiteninhalten</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1700">CVE-2015-1700</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-048">MS15-048</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in XML-Entschlüsselung in .NET bezüglich Denial-of-Service-Angriffen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1672">CVE-2015-1672</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-048">MS15-048</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Forms bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1673">CVE-2015-1673</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-049">MS15-049</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Silverlight bezüglich Anwendungen, die außerhalb des Browsers ausgeführt werden</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1715">CVE-2015-1715</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-050">MS15-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Dienststeuerungs-Manager bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1702">CVE-2015-1702</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-051">MS15-051</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Windows-Kernelspeicher bezüglich Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1676">CVE-2015-1676</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-051">MS15-051</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Windows-Kernelspeicher bezüglich Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1677">CVE-2015-1677</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-051">MS15-051</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Windows-Kernelspeicher bezüglich Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1678">CVE-2015-1678</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-051">MS15-051</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Windows-Kernelspeicher bezüglich Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1679">CVE-2015-1679</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-051">MS15-051</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Windows-Kernelspeicher bezüglich Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1680">CVE-2015-1680</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-051">MS15-051</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1701">CVE-2015-1701</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-052">MS15-052</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows-Kernel kann Umgehung von Sicherheitsfunktionen ermöglichen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1674">CVE-2015-1674</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-053">MS15-053</a></td>
<td style="border:1px solid black;">ASLR-Umgehung durch VBScript</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1684">CVE-2015-1684</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-053">MS15-053</a></td>
<td style="border:1px solid black;">ASLR-Umgehung durch VBScript und JScript</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1686">CVE-2015-1686</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-054">MS15-054</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Dateiformat von Microsoft Management Console (MMC) kann Denial-of-Service ermöglichen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1681">CVE-2015-1681</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-055">MS15-055</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Schannel kann Offenlegung von Informationen ermöglichen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1716">CVE-2015-1716</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
</tbody>
</table>
  
Betroffene Software  
-------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.
  
**Hinweis** Für eine Sicherheitsanfälligkeit müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
### Windows-Betriebssystem und -Komponenten (Tabelle 1 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)                                             
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)                                          
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3049563)  
(Mittel)  
Internet Explorer 7  
(3049563)  
(Mittel)  
Internet Explorer 8  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3048073)  
(Kritisch)  
Microsoft .NET Framework 4  
(3048074)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1 Service Pack 1  
(3023211)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3023220)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035488)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(Kein Update; siehe Hinweise)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3049563)  
(Mittel)  
Internet Explorer 7  
(3049563)  
(Mittel)  
Internet Explorer 8  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3048073)  
(Kritisch)  
Microsoft .NET Framework 4  
(3048074)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3023220)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035488)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(Kein Update; siehe Hinweise)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3049563)  
(Mittel)  
Internet Explorer 7  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3045171)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3023220)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035488)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(Kein Update; siehe Hinweise)  
(Hoch)
</td>
</tr>
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3049563)  
(Kritisch)  
Internet Explorer 8  
(3049563)  
(Kritisch)  
Internet Explorer 9  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3048068)  
(Kritisch)  
Microsoft .NET Framework 4  
(3048074)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3048077)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3023213)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035485)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3049563)  
(Kritisch)  
Internet Explorer 8  
(3049563)  
(Kritisch)  
Internet Explorer 9  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3048068)  
(Kritisch)  
Microsoft .NET Framework 4  
(3048074)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3048077)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3023213)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035485)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3055642)  
(Hoch)
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3049563)  
(Mittel)  
Internet Explorer 8  
(3049563)  
(Mittel)  
Internet Explorer 9  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3048068)  
(Kritisch)  
Microsoft .NET Framework 4  
(3048074)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3048077)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3023213)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035485)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3049563)  
(Mittel)  
Internet Explorer 8  
(3049563)  
(Mittel)  
Internet Explorer 9  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3048068)  
(Kritisch)  
Microsoft .NET Framework 4  
(3048074)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3048077)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3023213)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035485)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3045171)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3023213)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3035485)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3055642)  
(Hoch)
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3049563)  
(Kritisch)  
Internet Explorer 9  
(3049563)  
(Kritisch)  
Internet Explorer 10  
(3049563)  
(Kritisch)  
Internet Explorer 11  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(3048070)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3023215)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3032655)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3049563)  
(Kritisch)  
Internet Explorer 9  
(3049563)  
(Kritisch)  
Internet Explorer 10  
(3049563)  
(Kritisch)  
Internet Explorer 11  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(3048070)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3023215)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3032655)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3055642)  
(Hoch)
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3049563)  
(Mittel)  
Internet Explorer 9  
(3049563)  
(Mittel)  
Internet Explorer 10  
(3049563)  
(Mittel)  
Internet Explorer 11  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(3048070)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3023215)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3032655)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3045171)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3023215)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3032655)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3055642)  
(Hoch)
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048071)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023217)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035486)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023223)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035489)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048071)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023217)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035486)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023223)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035489)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048072)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023219)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035487)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3023222)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3032663)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048072)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023219)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035487)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3023222)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3032663)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3055642)  
(Hoch)
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048071)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023217)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035486)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023223)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035489)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3049563)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048072)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023219)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035487)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3023222)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3032663)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3055642)  
(Hoch)
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3045171)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023223)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035489)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3055642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3049563)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3045171)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3046002)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.1/4.5.2  
(3023222)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3032663)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3055642)  
(Hoch)
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
[**MS15-043**](https://technet.microsoft.com/de-de/library/security/ms15-043)
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-045**](https://technet.microsoft.com/de-de/library/security/ms15-045)
</td>
<td style="border:1px solid black;">
[**MS15-048**](https://technet.microsoft.com/de-de/library/security/ms15-048)
</td>
<td style="border:1px solid black;">
[**MS15-050**](https://technet.microsoft.com/de-de/library/security/ms15-050)
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3045171)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3055642)  
(Hoch)
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3045171)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3055642)  
(Hoch)
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(3048070)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3023215)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3032655)  
(Hoch)  
Microsoft .NET Framework 4  
(3023221)  
(Hoch)  
Microsoft .NET Framework 4  
(3032662)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023224)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035490)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3055642)  
(Hoch)
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
Windows Server 2012 (Server Core-Installation)  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048071)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023217)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035486)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3023223)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3035489)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3055642)  
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
Windows Server 2012 R2 (Server Core-Installation)  
(3045171)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(3048072)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3023219)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3035487)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3023222)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3032663)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3055642)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise zu MS15-044**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt.

Zudem sind Updates für Microsoft .NET Framework 4.6 RC verfügbar, allerdings nur über das [Microsoft Download Center](http://www.microsoft.com/de-de/download/search.aspx?q=security%20update).

**Hinweis zu MS15-043, MS15-044 und MS15-045**

Windows Technical Preview und Windows Server Technical Preview sind betroffen. Benutzern mit diesen Betriebssystemen wird empfohlen, die Updates über [Windows Update](http://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) zu installieren.

**Hinweis zu MS15-050**

Windows Server 2003 ist betroffen, aber es wird kein Update dafür veröffentlicht. Weitere Informationen finden Sie im Bulletin.

### Windows-Betriebssystem und -Komponenten (Tabelle 2 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="6">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)                                 
</td>
<td style="border:1px solid black;">
**Nicht bewertet**                                             
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)                                      
</td>
<td style="border:1px solid black;">
**Nicht bewertet**                                             
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)                                      
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.6 und VBScript 5.6  
(3050946)  
(Hoch)  
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.6 und VBScript 5.6  
(3050946)  
(Hoch)  
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.6 und VBScript 5.6  
(3050946)  
(Hoch)  
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3061518)  
(Hoch)
</td>
</tr>
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3061518)  
(Hoch)
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3061518)  
(Hoch)
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3061518)  
(Hoch)
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3061518)  
(Hoch)
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3061518)  
(Hoch)
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3061518)  
(Hoch)
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Windows RT  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3061518)  
(Hoch)
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
[**MS15-051**](https://technet.microsoft.com/de-de/library/security/ms15-051)
</td>
<td style="border:1px solid black;">
[**MS15-052**](https://technet.microsoft.com/de-de/library/security/ms15-052)
</td>
<td style="border:1px solid black;">
[**MS15-053**](https://technet.microsoft.com/de-de/library/security/ms15-053)
</td>
<td style="border:1px solid black;">
[**MS15-054**](https://technet.microsoft.com/de-de/library/security/ms15-054)
</td>
<td style="border:1px solid black;">
[**MS15-055**](https://technet.microsoft.com/de-de/library/security/ms15-055)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.7 und VBScript 5.7  
(3050945)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
JScript 5.8 und VBScript 5.8  
(3050941)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3061518)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3045171)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3050514)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3051768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3061518)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-053 und MS15-054:**

Windows Technical Preview und Windows Server Technical Preview sind betroffen. Benutzern mit diesen Betriebssystemen wird empfohlen, die Updates über [Windows Update](http://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) zu installieren.

 

### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft SharePoint Server 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
<td style="border:1px solid black;">
[**MS15-047**](https://technet.microsoft.com/de-de/library/security/ms15-047)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (32-Bit-Editionen)  
(2760412)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (64-Bit-Editionen)  
(2760412)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft SharePoint Server 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
<td style="border:1px solid black;">
[**MS15-047**](https://technet.microsoft.com/de-de/library/security/ms15-047)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 Service Pack 2  
(3017815)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 Service Pack 2  
(3017815)  
(Hoch)  
Microsoft SharePoint Server 2010 Service Pack 2  
(2956192)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft SharePoint Server 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
<td style="border:1px solid black;">
[**MS15-047**](https://technet.microsoft.com/de-de/library/security/ms15-047)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013 Service Pack 1  
(3039736)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2013 Service Pack 1  
(3054792)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-046**

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
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(2883029)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(2965282)  
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
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2881073)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2965311)  
(Hoch)  
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2999412)  
(Hoch)  
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2965242)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(2965240)  
(Hoch)  
Microsoft PowerPoint 2010 Service Pack 2 (32-Bit-Editionen)  
(2999420)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(2965237)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2881073)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2965311)  
(Hoch)  
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2999412)  
(Hoch)  
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2965242)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(2965240)  
(Hoch)  
Microsoft PowerPoint 2010 Service Pack 2 (64-Bit-Editionen)  
(2999420)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(2965237)  
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
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(2975808)  
(Hoch)  
Microsoft Excel 2013 Service Pack 1 (32-Bit-Editionen)  
(2986216)  
(Hoch)  
Microsoft PowerPoint 2013 Service Pack 1 (32-Bit-Editionen)  
(2975816)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (32-Bit-Editionen)  
(2965307)  
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
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)  
(2975808)  
(Hoch)  
Microsoft Excel 2013 Service Pack 1 (64-Bit-Editionen)  
(2986216)  
(Hoch)  
Microsoft PowerPoint 2013 Service Pack 1 (64-Bit-Editionen)  
(2975816)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (64-Bit-Editionen)  
(2965307)  
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
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Microsoft Office 2013 RT Service Pack 1  
(2975808)  
(Hoch)  
Microsoft Excel 2013 RT Service Pack 1  
(2986216)  
(Hoch)  
Microsoft PowerPoint 2013 RT Service Pack 1  
(2975816)  
(Hoch)  
Microsoft Word 2013 RT Service Pack 1  
(2965307)  
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
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Microsoft Office für Mac 2011  
(3048688)  
(Hoch)  
Microsoft Excel für Mac 2011  
(3048688)  
(Hoch)  
Microsoft PowerPoint für Mac 2011  
(3048688)  
(Hoch)  
Microsoft Word für Mac 2011  
(3048688)  
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
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft PowerPoint Viewer  
(2956195)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-044 und MS15-046**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

 

### Microsoft Office-Dienste und Web Apps

<p> </p>
<table style="border:1px solid black;">
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
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Word-Automatisierungsdienste  
(2965233)  
(Hoch)  
Excel Services  
(2956194)  
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
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Word-Automatisierungsdienste  
(3023055)  
(Hoch)  
Excel Services  
(3039725)  
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
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2  
(2956140)  
(Hoch)  
Microsoft Excel Web Apps 2010 Service Pack 2  
(2956193)  
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
[**MS15-046**](https://technet.microsoft.com/de-de/library/security/ms15-046)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2013 Service Pack 1  
(3039748)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-046**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Microsoft Communications-Plattformen und -Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Live Meeting 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Live Meeting 2007-Konsole
</td>
<td style="border:1px solid black;">
Microsoft Live Meeting 2007-Konsole  
(3051467)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Lync 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 (32 Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 (32 Bit)  
(3051464)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64 Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64 Bit)  
(3051464)  
(Kritisch)
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
(3051465)  
(Kritisch)
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
(3051466)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Lync 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (32-Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (32-Bit)  
(Skype for Business)  
(3039779)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (32-Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (32-Bit)  
(Skype for Business Basic)  
(3039779)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (64-Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync 2013 Service Pack 1 (64-Bit)  
(Skype for Business)  
(3039779)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (64-Bit)
</td>
<td style="border:1px solid black;">
Microsoft Lync Basic 2013 Service Pack 1 (64-Bit)  
(Skype for Business Basic)  
(3039779)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-044**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Silverlight**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-044**](https://technet.microsoft.com/de-de/library/security/ms15-044)
</td>
<td style="border:1px solid black;">
[**MS15-049**](https://technet.microsoft.com/de-de/library/security/ms15-049)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 5
</td>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation auf dem Mac  
(3056819)  
(Kritisch)  
Microsoft Silverlight 5 Developer Runtime bei Installation auf dem Mac  
(3056819)  
(Kritisch)  
Microsoft Silverlight 5 bei Installation unter allen Versionen von Microsoft Windows-Clients  
(3056819)  
(Kritisch)  
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(3056819)  
(Kritisch)  
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(3056819)  
(Kritisch)  
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(3056819)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation auf dem Mac  
(3056819)  
(Hoch)  
Microsoft Silverlight 5 Developer Runtime bei Installation auf dem Mac  
(3056819)  
(Hoch)  
Microsoft Silverlight 5 bei Installation unter allen Versionen von Microsoft Windows-Clients  
(3056819)  
(Hoch)  
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(3056819)  
(Hoch)  
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(3056819)  
(Hoch)  
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(3056819)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-044**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

Tools und Hinweise zur Erkennung und Bereitstellung von Sicherheitsupdates
--------------------------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter.

Windows Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager erleichtern Administratoren die Verteilung von Sicherheitsupdates.

Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](http://technet.microsoft.com/de-de/security/cc297183).

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
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](http://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://technet.microsoft.com/de-de/security/dn467918) aufgeführt sind.

### Sicherheitsstrategien und Community

**Updateverwaltungsstrategien**

Auf der Seite [Patchmanagement](http://technet.microsoft.com/de-de/library/bb466251.aspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsanfälligkeiten sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/de-de/kb/913086).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

### Support

Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.

Sicherheitslösungen für IT-Profis: [TechNet Security – Problembehandlung und Support](http://technet.microsoft.com/de-de/security/bb980617)

Hilfe beim Schützen des Computers, auf dem Windows ausgeführt wird, vor Viren und Schadsoftware: [Safety and Security Center](http://www.microsoft.com/de-de/security/default.aspx)

Lokaler Support entsprechend Ihrem Land: [Internationaler Support](http://support.microsoft.com/common/international.aspx?ln=de)

### Haftungsausschluss

Die Informationen in der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (12. Mai 2015): Bulletin Summary veröffentlicht.

*Seite generiert am 19.05.2015 um 13:28Z-07:00.*
