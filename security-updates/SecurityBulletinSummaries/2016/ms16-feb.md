---
TOCTitle: 'MS16-FEB'
Title: Microsoft Security Bulletin Summary für Februar 2016
ms:assetid: 'ms16-feb'
ms:contentKeyID: 72238929
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms16-feb(v=Security.10)'
---

Microsoft Security Bulletin Summary für Februar 2016
====================================================

Veröffentlicht: 9. Februar 2016 | Aktualisiert: 24. Februar 2016

**Version:** 3.1

In diesem Bulletin Summary sind die im Februar 2016 veröffentlichten Security Bulletins aufgeführt.

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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-009">MS16-009</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (3134220)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Wenn der aktuelle Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, Kontrolle über ein betroffenes System erlangen. Der Angreifer könnte dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Benutzerkonten mit Vollzugriffsrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3134814">3134814</a></td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-011">MS16-011</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Microsoft Edge (3134225) <br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Edge. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Microsoft Edge anzeigt. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Microsoft Edge</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-012">MS16-012</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek zum Unterbinden von Remotecodeausführung (3138938)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn die Microsoft Windows-PDF-Bibliothek API-Aufrufe nicht ordnungsgemäß verarbeitet und es einem Angreifer dadurch ermöglicht, beliebigen Code auf dem System des Benutzers auszuführen. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Allerdings hat der Angreifer keine Möglichkeit, Benutzer zum Herunterladen oder Öffnen eines schädlichen PDF-Dokuments zu zwingen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-013">MS16-013</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows Journal zum Unterbinden von Remotecodeausführung (3134811)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Journaldatei öffnet. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-014">MS16-014</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Windows zum Unterbinden von Remotecodeausführung (3134228)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn sich ein Angreifer bei einem Zielsystem anmelden und eine speziell gestaltete Anwendung ausführen kann.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3126041">3126041</a><br />
<a href="https://support.microsoft.com/de-de/kb/3126587">3126587</a><br />
<a href="https://support.microsoft.com/de-de/kb/3126593">3126593</a></td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-015">MS16-015</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Office zum Unterbinden von Remotecodeausführung (3134226)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office, <br />
Microsoft Office Services und Web Apps,<br />
Microsoft Server-Software </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-016">MS16-016</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Winsock zum Unterbinden einer Erhöhung von Berechtigungen (3136041)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer den Microsoft WebDAV-Client (Web Distributed Authoring and Versioning) nutzt, um speziell gestaltete Eingaben an einen Server zu senden.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-017">MS16-017</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für RDP-Bildschirmtreiber zum Unterbinden einer Erhöhung von Berechtigungen (3134700)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer über RDP bei einem Zielsystem anmeldet und speziell gestaltete Daten über die Verbindung sendet. Standardmäßig ist RDP in keinem Windows-Betriebssystem aktiviert. Systeme, auf denen RDP nicht aktiviert ist, sind nicht gefährdet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3134700">3134700</a><br />
<a href="https://support.microsoft.com/de-de/kb/3126446">3126446</a></td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de//library/security/ms16-018">MS16-018</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Windows-Kernelmodustreiber zum Unterbinden einer Erhöhung von Berechtigungen (3136082)</strong> <br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-019">MS16-019</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für .NET Framework zum Unterbinden von Denial-of-Service-Angriffen (3137893)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft .NET Framework. Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können einen Denial-of-Service-Angriff ermöglichen, wenn ein Angreifer speziell gestaltetes XSLT in ein clientseitiges XML-Webpart einfügt, das bewirkt, dass der Server XSLT-Transformationen rekursiv kompiliert.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows, <br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-020">MS16-020</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Active Directory-Verbunddienste zum Unterbinden von Denial-of-Service-Angriffen (3134222)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Active Directory-Verbunddienste (AD FS). Die Sicherheitsanfälligkeit kann einen Denial-of-Service-Angriff ermöglichen, wenn ein Angreifer während der formularbasierten Authentifizierung bestimmte Eingabedaten an einen AD FS-Server sendet und dadurch bewirkt, dass der Server nicht mehr reagiert.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-021">MS16-021</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für NPS-RADIUS-Server zum Unterbinden von Denial-of-Service-Angriffen (3133043)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann einen Denial-of-Service-Angriff auf einen Netzwerkrichtlinienserver (NPS: Network Policy Server) ermöglichen, wenn ein Angreifer speziell gestaltete Benutzernamenszeichenfolgen an den NPS sendet, die eine RADIUS-Authentifizierung auf dem NPS verhindern.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms16-022">MS16-022</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Adobe Flash Player (3135782) <br />
</strong>Diese Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Adobe Flash Player bei der Installation in allen unterstützten Editionen von Windows Server 2012, Windows 8.1, Windows Server 2012 R2, Windows RT 8.1 und Windows 10.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows<br />
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
[**MS16-009: Kumulatives Sicherheitsupdate für Internet Explorer (3134220)**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0041](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0041)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit beim Laden von DLL-Dateien bezüglich Remotecodeausführung
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
[CVE-2016-0059](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0059)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen
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
[CVE-2016-0060](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0060)
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
[CVE-2016-0061](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0061)
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
[CVE-2016-0062](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0062)
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
[CVE-2016-0063](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0063)
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
[CVE-2016-0064](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0064)
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
[CVE-2016-0067](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0067)
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
[CVE-2016-0068](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0068)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen
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
[CVE-2016-0069](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0069)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen
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
[CVE-2016-0071](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0071)
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
[CVE-2016-0072](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0072)
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
[CVE-2016-0077](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0077)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Browser bezüglich Spoofingangriffen
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
[**MS16-011: Kumulatives Sicherheitsupdate für Microsoft Edge (3134225)**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0060](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0060)
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
[CVE-2016-0061](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0061)
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
[CVE-2016-0062](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0062)
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
[CVE-2016-0077](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0077)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft-Browser bezüglich Spoofingangriffen
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
[CVE-2016-0080](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0080)
</td>
<td style="border:1px solid black;">
ASLR-Umgehung in Microsoft Edge
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
[CVE-2016-0084](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0084)
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
[**MS16-012: Sicherheitsupdate für Microsoft Windows-PDF-Bibliothek zum Unterbinden von Remotecodeausführung (3138938)**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0046](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0046)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Windows Reader
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
<td style="border:1px solid black;">
[CVE-2016-0058](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0058)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit durch Pufferüberlauf in Microsoft-PDF-Bibliothek
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
<td style="border:1px solid black;" colspan="6">
[**MS16-013: Sicherheitsupdate für Windows Journal zum Unterbinden von Remotecodeausführung (3134811)**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0038](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0038)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows Journal durch Speicherbeschädigung
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
[**MS16-014: Sicherheitsupdate für Microsoft Windows zum Unterbinden von Remotecodeausführung (3134228)**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0040](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0040)
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
<td style="border:1px solid black;">
[CVE-2016-0041](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0041)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit beim Laden von DLL-Dateien bezüglich Remotecodeausführung
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
[CVE-2016-0042](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0042)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows beim Laden von DLL-Dateien bezüglich Remotecodeausführung
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
[CVE-2016-0044](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0044)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows beim Laden von Bibliothek bezüglich Denial-of-Service-Angriffen
</td>
<td style="border:1px solid black;" colspan="2">
4 – Nicht betroffen
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
[CVE-2016-0049](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0049)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows Kerberos durch Umgehung von Sicherheitsfunktionen
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
[**MS16-015: Sicherheitsupdate für Microsoft Office zum Unterbinden von Remotecodeausführung (3134226)**](https://technet.microsoft.com/de-de/library/security/ms16-015)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0022](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0022)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[CVE-2016-0039](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0039)
</td>
<td style="border:1px solid black;">
Microsoft SharePoint-Sicherheitsanfälligkeit bezüglich XSS
</td>
<td style="border:1px solid black;">
3 – Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
4 – Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0052](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0052)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[CVE-2016-0053](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0053)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[CVE-2016-0054](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0054)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[CVE-2016-0055](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0055)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
4 – Nicht betroffen
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
[CVE-2016-0056](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0056)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung
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
[**MS16-016: Sicherheitsupdate für Winsock zum Unterbinden einer Erhöhung von Berechtigungen (3136041)**](https://technet.microsoft.com/de-de/library/security/ms16-016)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0051](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0051)
</td>
<td style="border:1px solid black;">
WebDAV-Sicherheitsanfälligkeit bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;" colspan="2">
3 – Ausnutzung unwahrscheinlich
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
[**MS16-017: Sicherheitsupdate für RDP-Bildschirmtreiber zum Unterbinden einer Erhöhung von Berechtigungen (3134700)**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0036](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0036)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Remotedesktopprotokoll (RDP) bezüglich der Erhöhung von Berechtigungen
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
[**MS16-018: Sicherheitsupdate für Windows-Kernelmodustreiber zum Unterbinden der Erhöhung von Berechtigungen (3136082)**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0048](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0048)
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
[**MS16-019: Sicherheitsupdate für .NET Framework zum Unterbinden von Denial-of-Service-Angriffen (3137893)**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0033](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0033)
</td>
<td style="border:1px solid black;">
.NET Framework-Sicherheitsanfälligkeit bezüglich Denial-of-Service durch Stapelüberlauf
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
[CVE-2016-0047](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0047)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows Forms bezüglich der Offenlegung von Informationen
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
[**MS16-020: Sicherheitsupdate für Active Directory-Verbunddienste zum Unterbinden von Denial-of-Service-Angriffen (3134222)**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0037](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0037)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Active Directory-Verbunddiensten bezüglich Denial-of-Service-Angriffen
</td>
<td style="border:1px solid black;" colspan="2">
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
<td style="border:1px solid black;" colspan="6">
[**MS16-021: Sicherheitsupdate für NPS-RADIUS-Server zum Unterbinden von Denial-of-Service-Angriffen (3133043)**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2016-0050](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2016-0050)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in RADIUS-Implementierung von Netzwerkrichtlinienserver bezüglich Denial-of-Service-Angriffen
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
<td style="border:1px solid black;" colspan="6">
[**MS16-022: Sicherheitsupdate für Adobe Flash Player (3135782)**](https://technet.microsoft.com/de-de/library/security/ms16-022)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[APSB16-04](https://helpx.adobe.com/de/security/products/flash-player/apsb16-04.html)
</td>
<td style="border:1px solid black;">
Die Bewertungen des Schweregrads und der Updatepriorität finden Sie unter [Adobe Security Bulletin APSB16-04](https://helpx.adobe.com/de/security/products/flash-player/apsb16-04.html).
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
<td style="border:1px solid black;" colspan="7">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3134814)  
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
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3126587)  
(Hoch)  
Windows Vista Service Pack 2  
(3126593)  
(Hoch)  
Windows Vista Service Pack 2  
(3126041)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3124280)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9  
(3134814)  
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
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3126587)  
(Hoch)  
Windows Vista x64 Edition Service Pack 2  
(3126593)  
(Hoch)  
Windows Vista x64 Edition Service Pack 2  
(3126041)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3124280)  
(Hoch)
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
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3134814)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3126587)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3126593)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3126041)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3124280)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9  
(3134814)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3126587)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3126593)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3126041)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3124280)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 9  
(3134814)  
(Mittel)
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
(3126587)  
(Hoch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3126593)  
(Hoch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3126041)  
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
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3134814)  
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
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3126587)  
(Hoch)  
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3126593)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3124280)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3134814)  
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
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3126587)  
(Hoch)  
Windows 7 für x64-basierte Systeme Service Pack 1  
(3126593)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3124280)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3134814)  
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
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3126587)  
(Hoch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3126593)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3124280)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3134814)  
(Mittel)
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
(3126587)  
(Hoch)  
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3126593)  
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
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3134814)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3123294)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3126587)  
(Hoch)  
Windows 8.1 für 32-Bit-Systeme  
(3126593)  
(Hoch)  
Windows 8.1 für 32-Bit-Systeme  
(3126041)  
(Hoch)  
Windows 8.1 für 32-Bit-Systeme  
(3126434)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3124280)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3134814)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3123294)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3126587)  
(Hoch)  
Windows 8.1 für x64-basierte Systeme  
(3126593)  
(Hoch)  
Windows 8.1 für x64-basierte Systeme  
(3126041)  
(Hoch)  
Windows 8.1 für x64-basierte Systeme  
(3126434)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3124280)  
(Mittel)
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
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Internet Explorer 10  
(3134814)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3123294)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3126587)  
(Hoch)  
Windows Server 2012  
(3126593)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3124280)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3134814)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3123294)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3115858)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3126587)  
(Hoch)  
Windows Server 2012 R2  
(3126593)  
(Hoch)  
Windows Server 2012 R2  
(3126041)  
(Hoch)  
Windows Server 2012 R2  
(3126434)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3124280)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
**Keine**
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
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3134814)  
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
Windows RT 8.1  
(3126587)  
(Hoch)  
Windows RT 8.1  
(3126593)  
(Hoch)  
Windows RT 8.1  
(3126434)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3124280)  
(Mittel)
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
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3135174)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3135174)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3135174)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3135173)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3135173)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3135173)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3135173)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme  
(3135173)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3135173)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3135173)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3135173)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3135173)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme  
(3135173)  
(Mittel)
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
[**MS16-009**](https://technet.microsoft.com/de-de/library/security/ms16-009)
</td>
<td style="border:1px solid black;">
[**MS16-011**](https://technet.microsoft.com/de-de/library/security/ms16-011)
</td>
<td style="border:1px solid black;">
[**MS16-012**](https://technet.microsoft.com/de-de/library/security/ms16-012)
</td>
<td style="border:1px solid black;">
[**MS16-013**](https://technet.microsoft.com/de-de/library/security/ms16-013)
</td>
<td style="border:1px solid black;">
[**MS16-014**](https://technet.microsoft.com/de-de/library/security/ms16-014)
</td>
<td style="border:1px solid black;">
[**MS16-016**](https://technet.microsoft.com/de-de/library/security/ms16-016)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3126587)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3126593)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3126041)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3126587)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3126593)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3126041)  
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
(3126587)  
(Hoch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3126593)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3126587)  
(Hoch)  
Windows Server 2012 (Server Core-Installation)  
(3126593)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3123294)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3126587)  
(Hoch)  
Windows Server 2012 R2 (Server Core-Installation)  
(3126593)  
(Hoch)  
Windows Server 2012 R2 (Server Core-Installation)  
(3126041)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
<td style="border:1px solid black;">
**Keine**
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
Windows Vista Service Pack 2  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3122646)  
(Hoch)  
Microsoft .NET Framework 2,0 Service Pack 2  
(3127219)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3122661)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3127233)  
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
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3122646)  
(Hoch)  
Microsoft .NET Framework 2,0 Service Pack 2  
(3127219)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3122661)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3127233)  
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
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3122646)  
(Hoch)  
Microsoft .NET Framework 2,0 Service Pack 2  
(3127219)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3122661)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3127233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3133043)  
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3122646)  
(Hoch)  
Microsoft .NET Framework 2,0 Service Pack 2  
(3127219)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3122661)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3127233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3133043)  
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
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2,0 Service Pack 2  
(3122646)  
(Hoch)  
Microsoft .NET Framework 2,0 Service Pack 2  
(3127219)  
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
<td style="border:1px solid black;" colspan="7">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
<td style="border:1px solid black;">
**Keine**
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
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3122648)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3127220)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122661)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127233)  
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
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3122648)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3127220)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122661)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127233)  
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
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3122648)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3127220)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122661)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127233)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3133043)  
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
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3122648)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3127220)  
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
<td style="border:1px solid black;" colspan="7">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
<td style="border:1px solid black;">
**Keine**
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
Windows 8.1 für 32-Bit-Systeme  
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3122651)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3127222)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122654)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127226)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122660)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3122651)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3127222)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122654)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127226)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122660)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
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
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3122649)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3127221)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122655)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127227)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122658)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127230)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3133043)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3122651)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3127222)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122654)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127226)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122660)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 3.0  
(3134222)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3133043)  
(Hoch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows RT 8.1  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.2  
(3122654)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127226)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122660)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
(Kritisch)
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
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
<td style="border:1px solid black;">
**Keine**
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
Windows 10 für 32-Bit-Systeme  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135174)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135174)  
(Hoch)  
Microsoft .NET Framework 4.6  
(3135174)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
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
(3135173)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135173)  
(Hoch)  
Microsoft .NET Framework 4.6.1  
(3135173)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
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
(3135173)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3135173)  
(Hoch)  
Microsoft .NET Framework 4.6.1  
(3135173)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3135782)  
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
[**MS16-017**](https://technet.microsoft.com/de-de/library/security/ms16-017)
</td>
<td style="border:1px solid black;">
[**MS16-018**](https://technet.microsoft.com/de-de//library/security/ms16-018)
</td>
<td style="border:1px solid black;">
[**MS16-019**](https://technet.microsoft.com/de-de/library/security/ms16-019)
</td>
<td style="border:1px solid black;">
[**MS16-020**](https://technet.microsoft.com/de-de/library/security/ms16-020)
</td>
<td style="border:1px solid black;">
[**MS16-021**](https://technet.microsoft.com/de-de/library/security/ms16-021)
</td>
<td style="border:1px solid black;">
[**MS16-022**](https://technet.microsoft.com/de-de/library/security/ms16-022)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(Server Core-Installation)  
(3134214)  
(Hoch)
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
(3133043)  
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(Server Core-Installation)  
(3134214)  
(Hoch)
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
(3133043)  
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3122648)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(3127220)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122656)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127229)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(Server Core-Installation)  
(3133043)  
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
Windows Server 2012 (Server Core-Installation)  
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3122649)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3127221)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122655)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127227)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122658)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127230)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(Server Core-Installation)  
(3133043)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3126446)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3134214)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3122651)  
(Hoch)  
Microsoft .NET Framework 3.5  
(3127222)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3122654)  
(Hoch)  
Microsoft .NET Framework 4.5.2  
(3127226)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3122660)  
(Hoch)  
Microsoft .NET Framework 4.6/4.6.1  
(3127231)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 3.0  
(3134222)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(Server Core-Installation)  
(3133043)  
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
(3114742)  
(Hoch)  
Microsoft Excel 2007 Service Pack 3  
(3114741)  
(Hoch)  
Microsoft Word 2007 Service Pack 3  
(3114748)  
(Kritisch)
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
(3114752)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(3114759)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(3114755)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3114752)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(3114759)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(3114755)  
(Kritisch)
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Excel 2013 Service Pack 1 (32-Bit-Editionen)  
(3114734)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (32-Bit-Editionen)  
(3114724)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 Service Pack 1 (64-Bit-Editionen)  
(3114734)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (64-Bit-Editionen)  
(3114724)  
(Kritisch)
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Excel 2013 RT Service Pack 1  
(3114734)  
(Hoch)  
Microsoft Word 2013 RT Service Pack 1  
(3114724)  
(Kritisch)
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (32-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2016 (32-Bit-Edition)  
(3114698)  
(Hoch)  
Microsoft Word 2016 (32-Bit-Edition)  
(3114702)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2016 (64-Bit-Edition)  
(3114698)  
(Hoch)  
Microsoft Word 2016 (64-Bit-Edition)  
(3114702)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office für Mac**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Microsoft Excel für Mac 2011  
(3137721)  
(Hoch)  
Microsoft Word für Mac 2011  
(3137721)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 für Mac
</td>
<td style="border:1px solid black;">
Microsoft Excel 2016 für Mac  
(3134241)  
(Hoch)  
Microsoft Word 2016 für Mac  
(3134241)  
(Kritisch)
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
(3114548)  
(Hoch)  
Microsoft Office Compatibility Pack Service Pack 3  
(3114745)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
Microsoft Excel Viewer  
(3114747)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(3114773)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS16-015**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

 

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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
Microsoft SharePoint Server 2007 Service Pack 3 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Excel Services  
(3114432)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Excel Services  
(3114432)  
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
Excel Services  
(3114401)  
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
Excel Services  
(3114335)  
(Hoch)  
Word-Automatisierungsdienste  
(3114481)  
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
(3114407)  
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
(3114338)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS16-015**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

 

### Microsoft Server-Software 

<p> </p>
<table style="border:1px solid black;">
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
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
Microsoft SharePoint Server 2013 Service Pack 1  
(3039768)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft SharePoint Foundation 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS16-015**](https://technet.microsoft.com/de-de/library/security/ms16-015)
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
Microsoft SharePoint Foundation 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2013 Service Pack 1  
(3114733)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS16-015**

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

-   V1.0 (9. Februar 2016): Bulletin Summary veröffentlicht.
-   V2.0 (10. Februar 2016): Für MS16-014 wurde das Bulletin Summary überarbeitet, um die Veröffentlichung des Updates 3126041 für Microsoft Windows Vista, Windows Server 2008, Windows Server 2008 für Itanium-basierte Systeme, Windows 8.1 und Windows Server 2012 R2 anzukündigen. Die Benutzer sollten die betreffenden Updates installieren, um vor den in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten geschützt zu sein. Die meisten Kunden haben automatische Updates aktiviert und müssen nichts weiter tun, weil die Updates automatisch heruntergeladen und installiert werden. In MS16-021 wurde die Bewertung der Ausnutzbarkeit von CVE-2016-0050 korrigiert.
-   V3.0 (16. Februar 2016): In MS16-015 wurde das Update 3134241 für Microsoft Office 2016 für Mac und das Update 3137721 für Microsoft Office für Mac 2011 hinzugefügt. Diese Updates sind ab dem 16. Februar 2016 verfügbar. Weitere Informationen finden Sie in [Microsoft Knowledge Base-Artikel 3134241](https://support.microsoft.com/de-de/kb/3134241) und [Microsoft Knowledge Base-Artikel 3137721](https://support.microsoft.com/de-de/kb/3137721).
-   V3.1 (24. Februar 2016): Der Tabelle in der Kurzzusammenfassung für MS16-014 wurde ein Verweis auf ein bekanntes Problem hinzugefügt. Weitere Informationen finden Sie in [Microsoft Knowledge Base-Artikel 3126041](https://support.microsoft.com/de-de/kb/3126041). Zudem wurde dem [Microsoft Knowledge Base-Artikel 3126587](https://support.microsoft.com/de-de/kb/3126587) ein zweites bekanntes Problem samt Problemumgehung hinzugefügt.

*Seite generiert am 24.02.2016 um 13:45:00-08:00.*