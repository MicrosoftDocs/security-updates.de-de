---
TOCTitle: 'MS16-MAR'
Title: Microsoft Security Bulletin Summary für März 2016
ms:assetid: 'ms16-mar'
ms:contentKeyID: 72464092
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms16-mar(v=Security.10)'
---

Microsoft Security Bulletin Summary für März 2016
=================================================

Veröffentlicht: 8. März 2016 | Aktualisiert: 25. März 2016

**Version:** 3.1

In diesem Bulletin Summary sind die im März 2016 veröffentlichten Security Bulletins aufgeführt.

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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-023">MS16-023</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (3142015)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Wenn der aktuelle Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, Kontrolle über ein betroffenes System erlangen. Der Angreifer könnte dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Benutzerkonten mit Vollzugriffsrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-024">MS16-024</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Microsoft Edge (3142019) <br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Edge. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Microsoft Edge anzeigt. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Microsoft Edge</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-025">MS16-025</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für das Laden von Windows-Bibliotheken zum Unterbinden von Remotecodeausführung (3140709)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn Microsoft Windows Eingaben vor dem Laden bestimmter Bibliotheken nicht ordnungsgemäß überprüft. Ein Angreifer muss aber zunächst auf das lokale System zugreifen und eine schädliche Anwendung auf dem System ausführen können.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-026">MS16-026</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Grafikschriften zum Unterbinden von Remotecodeausführung (3143148)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, ein speziell gestaltetes Dokument zu öffnen oder eine Webseite zu besuchen, in das bzw. die OpenType-Schriftarten eingebettet sind.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-027">MS16-027</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows-Medien Unterbinden von Remotecodeausführung (3143146)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer speziell gestaltete Medieninhalte öffnet, die auf einer Website gehostet werden.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-028">MS16-028</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek zum Unterbinden von Remotecodeausführung (3143081)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete PDF-Datei öffnet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-029">MS16-029</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Office zum Unterbinden von Remotecodeausführung (3141806)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office, <br />
Microsoft Office Services und Web Apps,<br />
Microsoft Server-Software </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-030">MS16-030</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows OLE zum Unterbinden von Remotecodeausführung (3143136)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn Windows OLE Benutzereingaben nicht ordnungsgemäß überprüft. Angreifer können die Sicherheitsanfälligkeiten ausnutzen, um schädlichen Code auszuführen. Allerdings muss ein Angreifer einen Benutzer zunächst dazu verleiten, eine speziell gestaltete Datei oder ein speziell gestaltetes Programm auf einer Webseite oder in einer E-Mail-Nachricht zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-031">MS16-031</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows zum Unterbinden einer Erhöhung von Berechtigungen (3140410)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem Zielsystem anmelden und eine speziell gestaltete Anwendung ausführen kann.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-032">MS16-032</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für sekundären Anmeldedienst zum Unterbinden einer Erhöhung von Berechtigungen (3143141)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn der sekundäre Windows-Anmeldedienst Handles im Speicher nicht ordnungsgemäß verarbeitet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-033">MS16-033</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows USB-Massenspeichergerät-Klassentreiber zum Unterbinden einer Erhöhung von Berechtigungen (3143142)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer mit physischem Zugang zum System ein speziell gestaltetes USB-Gerät in das System einfügt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-034">MS16-034</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows-Kernelmodustreiber zum Unterbinden einer Erhöhung von Berechtigungen (3143145)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-035">MS16-035</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für .NET Framework zum Unterbinden einer Umgehung von Sicherheitsfunktionen (3141780)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft .NET Framework. Die Umgehung von Sicherheitsfunktionen wird durch eine .NET Framework-Komponente ermöglicht, welche bestimmte Elemente signierter XML-Dokumente nicht ordnungsgemäß überprüft.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Umgehung von Sicherheitsfunktionen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3135996">3135996</a><br />
<a href="https://support.microsoft.com/de-de/kb/3136000">3136000</a><br />
<a href="https://support.microsoft.com/de-de/kb/3149737">3149737</a><br />
<a href="https://support.microsoft.com/de-de/kb/3148821">3148821</a></td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Microsoft .NET Framework</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-036">MS16-036</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Adobe Flash Player (3144756)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Adobe Flash Player bei der Installation unter allen unterstützten Editionen von Windows 8.1, Windows Server 2012, Windows Server 2012 R2, Windows RT 8.1 und Windows 10.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Adobe Flash Player</td>
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
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;">
**CVE ID** 
</td>
<td style="border:1px solid black;">
**Titel der Sicherheitsanfälligkeit**
</td>
<td style="border:1px solid black;" colspan="2">
**Bewertung der Ausnutzbarkeit für  
aktuelle Softwareversion**
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
<td style="border:1px solid black;" colspan="6">
[**MS16-023: Kumulatives Sicherheitsupdate für Internet Explorer (3142015)**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0102](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0102)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0103](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0103)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0104](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0104)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0105](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0105)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0106](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0106)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0107](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0107)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0108](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0108)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0109](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0109)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0110](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0110)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0111](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0111)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0112](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0112)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0113](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0113)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0114](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0114)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
<td style="border:1px solid black;" colspan="6">
[**MS16-024: Kumulatives Sicherheitsupdate für Microsoft Edge (3142019)**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0102](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0102)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0105](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0105)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0109](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0109)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0110](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0110)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0111](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0111)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Browser bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0116](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0116)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0123](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0123)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0124](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0124)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0125](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0125)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich der Offenlegung von Informationen
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0129](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0129)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0130](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0130)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
<td style="border:1px solid black;" colspan="6">
[**MS16-025: Sicherheitsupdate für das Laden von Windows-Bibliotheken zum Unterbinden von Remotecodeausführung (3140709)**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0100](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0100)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bezüglich Remotecodeausführung beim Laden von Bibliotheken
</td>
<td style="border:1px solid black;" colspan="2">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-026: Sicherheitsupdate für Grafikschriften zum Unterbinden von Remotecodeausführung (3143148)**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0120](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0120)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit beim Analysieren von OpenType-Schriftarten
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0121](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0121)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit beim Analysieren von OpenType-Schriftarten
</td>
<td style="border:1px solid black;" colspan="2">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-027: Sicherheitsupdate für Windows-Medien Unterbinden von Remotecodeausführung (3143146)**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0098](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0098)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bezüglich Remotecodeausführung beim Analysieren von Windows-Medien
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0101](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0101)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bezüglich Remotecodeausführung beim Analysieren von Windows-Medien
</td>
<td style="border:1px solid black;" colspan="2">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-028: Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek zum Unterbinden von Remotecodeausführung (3143081)**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0117](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0117)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0118](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0118)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-029: Sicherheitsupdate für Microsoft Office zum Unterbinden von Remotecodeausführung (3141806)**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0021](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0021)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0057](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0057)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office durch Umgehung der Sicherheitsfunktionen
</td>
<td style="border:1px solid black;" colspan="2">
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
[CVE-2016-0134](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0134)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;" colspan="2">
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
<td style="border:1px solid black;" colspan="6">
[**MS16-030: Sicherheitsupdate für Windows OLE zum Unterbinden von Remotecodeausführung (3143136)**](https://technet.microsoft.com/de-de/library/security/ms16-030)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0091](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0091)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Windows-OLE-Speicher bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;" colspan="2">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0092](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0092)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Windows-OLE-Speicher bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;" colspan="2">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-031: Sicherheitsupdate für Microsoft Windows zum Unterbinden einer Erhöhung von Berechtigungen (3140410)**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0087](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0087)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-032: Sicherheitsupdate für sekundären Anmeldedienst zum Unterbinden einer Erhöhung von Berechtigungen (3143141)**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0099](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0099)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in sekundärem Anmeldedienst bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-033: Sicherheitsupdate für Windows USB-Massenspeichergerät-Klassentreiber zum Unterbinden einer Erhöhung von Berechtigungen (3143142)**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0133](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0133)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in USB-Massenspeicher bezüglich einer Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-034: Sicherheitsupdate für Windows-Kernelmodustreiber zum Unterbinden der Erhöhung von Berechtigungen (3143145)**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0093](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0093)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0094](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0094)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
2 – Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0095](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0095)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0096](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0096)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
1 – Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="6">
[**MS16-035: Sicherheitsupdate für .NET Framework zum Unterbinden einer Umgehung von Sicherheitsfunktionen (3141780)**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0132](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0132)
</td>
<td style="border:1px solid black;">
.NET-Sicherheitsanfälligkeit bei XML-Überprüfung durch Umgehung von Sicherheitsfunktionen
</td>
<td style="border:1px solid black;" colspan="2">
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
<td style="border:1px solid black;" colspan="6">
[**MS16-036: Sicherheitsupdate für Adobe Flash Player (3144756)**](https://technet.microsoft.com/de-de/library/security/ms16-036)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[APSB16-08](https://helpx.adobe.com/de/security/products/flash-player/apsb16-08.html)
</td>
<td style="border:1px solid black;">
Die Bewertungen des Schweregrads und der Updatepriorität finden Sie unter [Adobe Security Bulletin APSB16-08](https://helpx.adobe.com/de/security/products/flash-player/apsb16-08.html).
</td>
<td style="border:1px solid black;" colspan="2">
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
-------------------

In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.

In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.

**Hinweis** Für eine Sicherheitsanfälligkeit müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.

 

### Windows-Betriebssysteme und Komponenten (Tabelle 1 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9  
(3139929)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3140709)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3140735)  
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
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9  
(3139929)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3140709)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3140735)  
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
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
**Keine**
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9  
(3139929)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3140709)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9  
(3139929)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3140709)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3139940)  
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
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3140709)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3139929)  
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
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3138910)  
(Kritisch)  
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3138962)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3139929)  
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
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3138910)  
(Kritisch)  
Windows 7 für x64-basierte Systeme Service Pack 1  
(3138962)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
**Keine**
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3139929)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3138910)  
(Kritisch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3138962)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3139940)  
(Hoch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3139929)  
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
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3138910)  
(Kritisch)  
Windows 8.1 für 32-Bit-Systeme  
(3138962)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3137513)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3139929)  
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
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3138910)  
(Kritisch)  
Windows 8.1 für x64-basierte Systeme  
(3138962)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3137513)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Internet Explorer 10  
(3139929)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3138910)  
(Kritisch)  
Windows Server 2012  
(3138962)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3137513)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3139929)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3138910)  
(Kritisch)  
Windows Server 2012 R2  
(3138962)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3137513)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3139929)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3138910)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3137513)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3139940)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Internet Explorer 11  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3140745)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3140745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3140745)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3140768)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3140768)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3140768)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="8">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-023**](https://technet.microsoft.com/de-de/library/security/ms16-023)
</td>
<td style="border:1px solid black;">
[**MS16-024**](https://technet.microsoft.com/de-de/library/security/ms16-024)
</td>
<td style="border:1px solid black;">
[**MS16-025**](https://technet.microsoft.com/de-de/library/security/ms16-025)
</td>
<td style="border:1px solid black;">
[**MS16-026**](https://technet.microsoft.com/de-de/library/security/ms16-026)
</td>
<td style="border:1px solid black;">
[**MS16-027**](https://technet.microsoft.com/de-de/library/security/ms16-027)
</td>
<td style="border:1px solid black;">
[**MS16-028**](https://technet.microsoft.com/de-de/library/security/ms16-028)
</td>
<td style="border:1px solid black;">
[**MS16-030**](https://technet.microsoft.com/de-de/library/security/ms16-030)
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
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3140709)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3139940)  
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
(3140709)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3139940)  
(Hoch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3139940)  
(Hoch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3139940)  
(Hoch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3140735)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3137513)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3139940)  
(Hoch)
</td>
</tr>
</table>
 
 

### Windows-Betriebssysteme und Komponenten (Tabelle 2 von 2)

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
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
Windows Vista Service Pack 2  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3135982)  
(Hoch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3135987)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3136000)  
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
Windows Vista x64 Edition Service Pack 2  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3135982)  
(Hoch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3135987)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3136000)  
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
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3135982)  
(Hoch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3135987)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3136000)  
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
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3135982)  
(Hoch)  
Microsoft .NET Framework 3.0 Service Pack 2  
(3135987)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3136000)  
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
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3135982)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3135983)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3135988)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3136000)  
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
Windows 7 für x64-basierte Systeme Service Pack 1  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3135983)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3135988)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3136000)  
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
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3135983)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3135988)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3136000)  
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
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3135983)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135985)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3135991)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135994)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3135998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135985)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3135991)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135994)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3135998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Kritisch)
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
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2012  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135984)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3135989)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135995)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3135997)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
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
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135985)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3135991)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135994)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3135998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.2  
(3135994)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3135998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3140745)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Kritisch)
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
Windows 10 für x64-basierte Systeme  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3140745)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3140745)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3140768)  
(Hoch)  
Microsoft .NET Framework 4.6.1  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3140768)  
(Hoch)  
Microsoft .NET Framework 4.6.1  
(3140768)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3144756)  
(Kritisch)
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
[**MS16-031**](https://technet.microsoft.com/de-de/library/security/ms16-031)
</td>
<td style="border:1px solid black;">
[**MS16-032**](https://technet.microsoft.com/de-de/library/security/ms16-032)
</td>
<td style="border:1px solid black;">
[**MS16-033**](https://technet.microsoft.com/de-de/library/security/ms16-033)
</td>
<td style="border:1px solid black;">
[**MS16-034**](https://technet.microsoft.com/de-de/library/security/ms16-034)
</td>
<td style="border:1px solid black;">
[**MS16-035**](https://technet.microsoft.com/de-de/library/security/ms16-035)
</td>
<td style="border:1px solid black;">
[**MS16-036**](https://technet.microsoft.com/de-de/library/security/ms16-036)
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
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3139852)  
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
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3139852)  
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
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3140410)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3135983)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3135988)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135996)  
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
Windows Server 2012  
(Server Core-Installation)  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135984)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3135989)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135995)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3135997)  
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
Windows Server 2012 R2  
(Server Core-Installation)  
(3139914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3139398)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3139852)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135985)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3135991)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3135994)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3135998)  
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
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(2956110)  
(Hoch)  
Microsoft InfoPath 2007 Service Pack 3  
(3114426)  
(Hoch)  
Microsoft Outlook 2007 Service Pack 3  
(2880510)  
(Hoch)  
Microsoft Word 2007 Service Pack 3  
(3114901)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2956063)  
(Hoch)  
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(3114873)  
(Hoch)  
Microsoft InfoPath 2010 Service Pack 2 (32-Bit-Editionen)  
(3114414)  
(Hoch)  
Microsoft Outlook 2010 Service Pack 2 (32-Bit-Editionen)  
(3114883)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(3114878)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3114873)  
(Hoch)  
Microsoft InfoPath 2010 Service Pack 2 (64-Bit-Editionen)  
(3114414)  
(Hoch)  
Microsoft Outlook 2010 Service Pack 2 (64-Bit-Editionen)  
(3114883)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(3114878)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)  
(3039746)  
(Hoch)  
Microsoft InfoPath 2013 Service Pack 1 (32-Bit-Editionen)  
(3114833)  
(Hoch)  
Microsoft Outlook 2013 Service Pack 1 (32-Bit-Editionen)  
(3114829)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (32-Bit-Editionen)  
(3114824)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft InfoPath 2013 Service Pack 1 (64-Bit-Editionen)  
(3114833)  
(Hoch)  
Microsoft Outlook 2013 Service Pack 1 (64-Bit-Editionen)  
(3114829)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (64-Bit-Editionen)  
(3114824)  
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
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 RT Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Outlook 2013 RT Service Pack 1  
(3114829)  
(Hoch)  
Microsoft Word 2013 RT Service Pack 1  
(3114824)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (32-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Office 2016 (32-Bit-Edition)  
(3114690)  
(Hoch)  
Microsoft Outlook 2016 (32-Bit-Edition)  
(3114861)  
(Hoch)  
Microsoft Word 2016 (32-Bit-Edition)  
(3114855)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Outlook 2016 (64-Bit-Edition)  
(3114861)  
(Hoch)  
Microsoft Word 2016 (64-Bit-Edition)  
(3114855)  
(Hoch)
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
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Word für Mac 2011  
(3138328)<sup>[1]</sup>
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2016 für Mac**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 für Mac
</td>
<td style="border:1px solid black;">
Microsoft Word 2016 für Mac  
(3138327)<sup>[1]</sup>
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
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Office Compatibility Pack Service Pack 3  
(3114900)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(3114812)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise zu MS16-029**

<sup>[1]</sup>Gemäß dem Stand vom 16. März 2016 sind das Update 3138327 für Microsoft Office 2016 für Mac und das Update 3138328 für Microsoft Office für Mac 2011 verfügbar. Beachten Sie, dass das Update 3138327 für Microsoft Outlook 2016 für Mac am 16. März 2016 noch nicht veröffentlicht worden war. Das Update wird veröffentlicht, sobald es verfügbar ist, und die Benutzer werden durch eine Überarbeitung des Bulletins benachrichtigt. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 3138327](https://support.microsoft.com/de-de/kb/3138327) und im [Microsoft Knowledge Base-Artikel 3138328](https://support.microsoft.com/de-de/kb/3138328).

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
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Word-Automatisierungsdienste  
(3114866)  
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
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Word-Automatisierungsdienste  
(3114814)  
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
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2  
(3114880)  
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
[**MS16-029**](https://technet.microsoft.com/de-de/library/security/ms16-029)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2013 Service Pack 1  
(3114821)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise zu MS16-029**

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

Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/de-de/lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.

Sicherheitslösungen für IT-Profis: [TechNet Security – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)

Hilfe beim Schützen des Computers, auf dem Windows ausgeführt wird, vor Viren und Schadsoftware: [Safety and Security Center](https://www.microsoft.com/de-de/security/default.aspx)

Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx?ln=de)

### Haftungsausschluss

Die Informationen in der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (8. März 2016): Bulletin Summary veröffentlicht.
-   V2.0 (10. März 2016): Das Bulletin Summary wurde zur Dokumentation der außerplanmäßigen Veröffentlichung von MS16-036 überarbeitet.
-   V2.1 (10. März 2016): Der Tabelle in der Kurzzusammenfassung für MS16-035 wurde ein Verweis auf ein bekanntes Problem hinzugefügt. Weitere Informationen finden Sie in [Microsoft Knowledge Base-Artikel 3148821](https://support.microsoft.com/de-de/kb/3148821).
-   V2.2 (15. März 2016): Der Tabelle in der Kurzzusammenfassung für MS16-035 wurden Verweise auf bekannte Probleme hinzugefügt. Weitere Informationen finden Sie in [Microsoft Knowledge Base-Artikel 3135996](https://support.microsoft.com/de-de/kb/3135996), [Microsoft Knowledge Base-Artikel 3136000](https://support.microsoft.com/de-de/kb/3136000) und [Microsoft Knowledge Base-Artikel 3149737](https://support.microsoft.com/de-de/kb/3149737).
-   V3.0 (16. März 2016): In MS16-029 wurden das Update 3138327 für Microsoft Office 2016 für Mac und das Update 3138328 für Microsoft Office für Mac 2011 hinzugefügt, die ab dem 16. März 2016 verfügbar sind. Beachten Sie, dass das Update 3138327 für Microsoft Outlook 2016 für Mac am 16. März 2016 noch nicht veröffentlicht worden war. Das Update wird veröffentlicht, sobald es verfügbar ist, und die Benutzer werden durch eine Überarbeitung des Bulletins benachrichtigt. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 3138327](https://support.microsoft.com/de-de/kb/3138327) und im [Microsoft Knowledge Base-Artikel 3138328](https://support.microsoft.com/de-de/kb/3138328).
-   V3.1 (25. März 2016): Für MS16-028 wurde Windows Server 2012 (Server Core-Installation) aus den Windows-Betriebssystemen und Komponenten (Tabelle 1 von 2) entfernt, da es nicht betroffen ist. Diese Änderung dient lediglich zur Information.

*Seite generiert am 2016-03-25 um 11:32-07:00.*