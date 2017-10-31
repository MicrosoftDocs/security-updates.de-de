---
TOCTitle: 'MS15-APR'
Title: Microsoft Security Bulletin Summary für April 2015
ms:assetid: 'ms15-apr'
ms:contentKeyID: 65308465
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms15-apr(v=Security.10)'
---

Microsoft Security Bulletin Summary für April 2015
==================================================

Veröffentlicht: 14. April 2015

**Version:** 1.0

In diesem Bulletin Summary sind die im April 2015 veröffentlichten Security Bulletins aufgeführt.

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
<td style="border:1px solid black;"><strong>Betroffene<br />
Software</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (3038314)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532628">MS15-033</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (3048019)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532630">MS15-034</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in HTTP.sys kann Remotecodeausführung ermöglichen (3042553) </strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete HTTP-Anforderung an ein betroffenes Windows-System sendet.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532631">MS15-035</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Graphics-Komponente kann Remotecodeausführung ermöglichen (3046306)</strong> <br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer erfolgreich dazu verleitet, eine speziell gestaltete Website zu besuchen, eine speziell gestaltete Datei zu öffnen oder eine Datei in einem Arbeitsverzeichnis zu öffnen, das eine speziell gestaltete Enhanced Metafile-Bilddatei (EMF) enthält. Ein Angreifer kann Benutzer jedoch nicht zum Ausführen einer solchen Aktion zwingen. Ein Angreifer muss Benutzer vielmehr zu diesen Handlungen verleiten. Zu diesem Zweck werden Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder einer Instant Messenger-Nachricht zu klicken.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532634">MS15-036</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft SharePoint Server können Rechteerweiterungen ermöglichen (3052044)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office-Server- und Produktivitätssoftware. Die Sicherheitsanfälligkeiten können Rechteerweiterungen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anforderung an einen betroffenen SharePoint-Server sendet. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann Inhalte lesen, für die er keine Leseberechtigung besitzt, die Identität des Opfers verwenden, um auf der SharePoint-Website Aktionen im Namen des Opfers auszuführen (wie z. B. Berechtigungen ändern und Inhalte löschen) und schädlichen Inhalt in den Browser des Opfers injizieren.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a>                                            <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Server-Software,<br />
Produktivitätssoftware</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532635">MS15-037</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in der Windows-Aufgabenplanung kann Rechteerweiterungen ermöglichen (3046269)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann eine bekannte ungültige Aufgabe nutzen, die bewirkt, dass die Aufgabenplanung eine speziell gestaltete Anwendung im Kontext des Systemkontos ausführt. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a>                                            <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Kein Neustart erforderlich.</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532639">MS15-038</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Windows können Rechteerweiterungen ermöglichen (3049576)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Rechteeweiterungen ermöglichen, wenn sich ein Angreifer bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Um diese Sicherheitsanfälligkeiten auszunutzen, muss sich ein Angreifer zuerst am System anmelden.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a>                                            <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532641">MS15-039</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in XML Core Services kann Umgehung der Sicherheitsfunktion ermöglichen (3046482)</strong> <br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Umgehung der Sicherheitsfunktion ermöglichen, wenn ein Benutzer auf einen speziell gestalteten Link klickt. Ein Angreifer hat jedoch keine Möglichkeit, Benutzer zum Klicken auf einen speziell gestalteten Link zu zwingen. Vielmehr muss ein Angreifer die Benutzer dazu verleiten, auf den Link zu klicken. Zu diesem Zweck werden Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder einer Instant Messenger-Nachricht zu klicken.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a>                                            <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532642">MS15-040</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory-Verbunddiensten kann Offenlegung von Informationen ermöglichen (3045711)</strong> <br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Active Directory-Verbunddiensten (AD FS). Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer den Webbrowser geöffnet lässt, nachdem er sich von einer Anwendung abgemeldet hat, und ein Angreifer die Anwendung unmittelbar nach der Abmeldung des Benutzers im Webbrowser erneut öffnet.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a>                                            <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532643">MS15-041</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework kann Offenlegung von Information ermöglichen (3048010)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft .NET Framework. Die Sicherheitsanfälligkeit kann eine Offenlegung von Information ermöglichen, wenn ein Angreifer eine speziell gestaltete Webanforderung an einen betroffenen Server sendet, auf dem benutzerdefinierte Fehlermeldungen deaktiviert sind. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann dann Teile einer Webkonfigurationsdatei anzeigen, die vertrauliche Informationen enthalten kann.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a>                                            <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532644">MS15-042</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Hyper-V kann Denial-of-Service ermöglichen (3047234) </strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann einen Denial-of-Service-Angriff ermöglichen, wenn ein authentifizierter Angreifer eine speziell gestaltete Anwendung in einer VM-Sitzung (Virtual Machine, virtueller Computer) ausführt. Beachten Sie, dass der Denial-of-Service-Angriff dem Angreifer nicht ermöglicht, auf anderen virtuellen Computern, die auf dem Hyper-V-Host ausgeführt werden, Code auszuführen oder Rechte zu erweitern, sondern dazu führt, dass andere auf dem Host ausgeführte virtuelle Computer nicht mehr im Virtual Machine Manager verwaltet werden können.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a>                                            <br />
DoS (Denial of Service)</td>
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
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259).
  
In den nachfolgenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.
 
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
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für<br />
aktuelle Softwareversion</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für<br />
ältere Softwareversionen</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit<br />
durch Denial-of-Service</strong></td>
<td style="border:1px solid black;"><strong>Wichtige Hinweise</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1652">CVE-2015-1652</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1657">CVE-2015-1657</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1659">CVE-2015-1659</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1660">CVE-2015-1660</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Umgehung der Internet Explorer ASLR</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1661">CVE-2015-1661</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1662">CVE-2015-1662</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1665">CVE-2015-1665</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1666">CVE-2015-1666</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1667">CVE-2015-1667</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532626">MS15-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1668">CVE-2015-1668</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532628">MS15-033</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Outlook Mac-App bezüglich XSS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1639">CVE-2015-1639</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532628">MS15-033</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1641">CVE-2015-1641</a></td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich bekannt gegeben.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532628">MS15-033</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Microsoft Office-Komponente</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1649">CVE-2015-1649</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532628">MS15-033</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Microsoft Office-Komponente</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1650">CVE-2015-1650</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532628">MS15-033</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Microsoft Office-Komponente</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1651">CVE-2015-1651</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532630">MS15-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit HTTP.sys bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1635">CVE-2015-1635</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532631">MS15-035</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit EMF-Verarbeitung bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1645">CVE-2015-1645</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532634">MS15-036</a></td>
<td style="border:1px solid black;">Microsoft SharePoint-Sicherheitsanfälligkeit bezüglich XSS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1640">CVE-2015-1640</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532634">MS15-036</a></td>
<td style="border:1px solid black;">Microsoft SharePoint-Sicherheitsanfälligkeit bezüglich XSS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1653">CVE-2015-1653</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532635">MS15-037</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in der Windows-Aufgabenplanung bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0098">CVE-2015-0098</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532639">MS15-038</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Objekttypverwechslung in NtCreateTransactionManager</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1643">CVE-2015-1643</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532639">MS15-038</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Windows MS-DOS-Gerätenamen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1644">CVE-2015-1644</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532641">MS15-039</a></td>
<td style="border:1px solid black;">MSXML3-Sicherheitsanfälligkeit durch Umgehung der Sicherheitsfunktion SOP</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1646">CVE-2015-1646</a></td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532642">MS15-040</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Active Directory-Verbunddiensten kann Offenlegung von Information ermöglichen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1638">CVE-2015-1638</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532643">MS15-041</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in ASP.NET bezüglich der Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1648">CVE-2015-1648</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=532644">MS15-042</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Hyper-V bezüglich Denial-of-Service</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1647">CVE-2015-1647</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">4 - Nicht betroffen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann zu einem Denial-of-Service-Angriff führen.</td>
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3038314)  
(Mittel)  
Internet Explorer 7  
(3038314)  
(Mittel)  
Internet Explorer 8  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 Service Pack 2  
(3045685)  
(Hoch)  
Windows Server 2003 Service Pack 2  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3038314)  
(Mittel)  
Internet Explorer 7  
(3038314)  
(Mittel)  
Internet Explorer 8  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 x64 Edition Service Pack 2  
(3045685)  
(Hoch)  
Windows Server 2003 x64 Edition Service Pack 2  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3038314)  
(Mittel)  
Internet Explorer 7  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3038314)  
(Kritisch)  
Internet Explorer 8  
(3038314)  
(Kritisch)  
Internet Explorer 9  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3045685)  
(Hoch)  
Windows Vista Service Pack 2  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3038314)  
(Kritisch)  
Internet Explorer 8  
(3038314)  
(Kritisch)  
Internet Explorer 9  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3045685)  
(Hoch)  
Windows Vista x64 Edition Service Pack 2  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3038314)  
(Mittel)  
Internet Explorer 8  
(3038314)  
(Mittel)  
Internet Explorer 9  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3045685)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3038314)  
(Mittel)  
Internet Explorer 8  
(3038314)  
(Mittel)  
Internet Explorer 9  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3045685)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3045685)  
(Hoch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
(3038314)  
(Kritisch)  
Internet Explorer 9  
(3038314)  
(Kritisch)  
Internet Explorer 10  
(3038314)  
(Kritisch)  
Internet Explorer 11  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3046269)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3045685)  
(Hoch)  
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3038314)  
(Kritisch)  
Internet Explorer 9  
(3038314)  
(Kritisch)  
Internet Explorer 10  
(3038314)  
(Kritisch)  
Internet Explorer 11  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3046269)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3045685)  
(Hoch)  
Windows 7 für x64-basierte Systeme Service Pack 1  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
(3038314)  
(Mittel)  
Internet Explorer 9  
(3038314)  
(Mittel)  
Internet Explorer 10  
(3038314)  
(Mittel)  
Internet Explorer 11  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3046269)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3045685)  
(Hoch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3046269)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3045685)  
(Hoch)  
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
**Keine**
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
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3042553)  
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
(3045685)  
(Hoch)  
Windows 8 für 32-Bit-Systeme  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3042553)  
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
(3045685)  
(Hoch)  
Windows 8 für x64-basierte Systeme  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3042553)  
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
(3045685)  
(Hoch)  
Windows 8.1 für 32-Bit-Systeme  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3038314)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3042553)  
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
(3045685)  
(Hoch)  
Windows 8.1 für x64-basierte Systeme  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
**Keine**
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
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3045685)  
(Hoch)  
Windows Server 2012  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3038314)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3045685)  
(Hoch)  
Windows Server 2012 R2  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
**Keine**
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3038314)  
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
Windows RT  
(3045685)  
(Hoch)  
Windows RT  
(3045999)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3038314)  
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
(3045685)  
(Hoch)  
Windows RT 8.1  
(3045999)  
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
[**MS15-032**](http://go.microsoft.com/fwlink/?linkid=532626)
</td>
<td style="border:1px solid black;">
[**MS15-034**](http://go.microsoft.com/fwlink/?linkid=532630)
</td>
<td style="border:1px solid black;">
[**MS15-035**](http://go.microsoft.com/fwlink/?linkid=532631)
</td>
<td style="border:1px solid black;">
[**MS15-037**](http://go.microsoft.com/fwlink/?linkid=532635)
</td>
<td style="border:1px solid black;">
[**MS15-038**](http://go.microsoft.com/fwlink/?linkid=532639)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3045685)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3045999)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3045685)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3045999)  
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
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3046306)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3046269)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3045685)  
(Hoch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3045999)  
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
(3042553)  
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
(3045685)  
(Hoch)  
Windows Server 2012 (Server Core-Installation)  
(3045999)  
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
(3042553)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3045685)  
(Hoch)  
Windows Server 2012 R2 (Server Core-Installation)  
(3045999)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-032 und MS15-034**

Windows Technical Preview und Windows Server Technical Preview sind betroffen. Benutzern mit diesen Betriebssystemen wird empfohlen, das Update über [Windows Update](http://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) zu installieren.

### Windows-Betriebssystem und -Komponenten (Tabelle 2 von 2)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="5">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1 Service Pack 1  
(3037572)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(3037577)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3037577)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)
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
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3037577)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3037573)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
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
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3037573)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3037573)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
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
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3037573)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
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
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(3037573)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3037574)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
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
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3037574)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3037574)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
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
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3037574)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037580)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037580)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037576)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3037579)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037576)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3037579)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3047234)  
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037580)  
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
Active Directory-Verbunddienste 3.0  
(3045711)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037576)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3037579)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3047234)  
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037580)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.1/4.5.2  
(3037579)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
[**MS15-039**](http://go.microsoft.com/fwlink/?linkid=532641)
</td>
<td style="border:1px solid black;">
[**MS15-040**](http://go.microsoft.com/fwlink/?linkid=532642)
</td>
<td style="border:1px solid black;">
[**MS15-041**](http://go.microsoft.com/fwlink/?linkid=532643)
</td>
<td style="border:1px solid black;">
[**MS15-042**](http://go.microsoft.com/fwlink/?linkid=532644)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3046482)  
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3046482)  
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3046482)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(3037574)  
(Hoch)  
Microsoft .NET Framework 4  
(3037578)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037581)  
(Hoch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(3037580)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
Active Directory-Verbunddienste 3.0  
(3045711)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(3037576)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(3037579)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3047234)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-040 und MS15-042:**

Windows Technical Preview und Windows Server Technical Preview sind betroffen. Benutzern mit diesen Betriebssystemen wird empfohlen, die Updates über [Windows Update](http://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) zu installieren.

 

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
[**MS15-036**](http://go.microsoft.com/fwlink/?linkid=532634)
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
Microsoft SharePoint Foundation 2013 Service Pack 1  
(2965219)  
(Hoch)  
Microsoft SharePoint Server 2013 Service Pack 1  
(2965219)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-036**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

 

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
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
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
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Word 2007 Service Pack 3  
(2965284)  
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
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
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
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2965236)  
(Kritisch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(2553428)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2965236)  
(Kritisch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(2553428)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2013 und Microsoft Office 2013 RT**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
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
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Word 2013 Service Pack 1 (32-Bit-Editionen)  
(2965224)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Word 2013 Service Pack 1 (64-Bit-Editionen)  
(2965224)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 RT Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 RT Service Pack 1  
(2965224)  
(Hoch)
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
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
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
Microsoft Outlook für Mac für Office 365
</td>
<td style="border:1px solid black;">
Microsoft Outlook für Mac für Office 365  
(3055707)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011  
(3051737)  
(Hoch)  
Microsoft Word für Mac 2011  
(3051737)  
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
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
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
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(2965289)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2965210)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-033**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

 

### Microsoft Office-Dienste und Web Apps

<p> </p>
<table style="border:1px solid black;">
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
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
</td>
<td style="border:1px solid black;">
[**MS15-036**](http://go.microsoft.com/fwlink/?linkid=532634)
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
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Word-Automatisierungsdienste  
(2553164)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Project Server 2010 Service Pack 2  
(2965302)  
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
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
</td>
<td style="border:1px solid black;">
[**MS15-036**](http://go.microsoft.com/fwlink/?linkid=532634)
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
Word-Automatisierungsdienste  
(2965215)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Project Server 2013 Service Pack 1  
(2965278)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office Web Apps 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
</td>
<td style="border:1px solid black;">
[**MS15-036**](http://go.microsoft.com/fwlink/?linkid=532634)
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
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2010 Service Pack 2  
(2965238)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office Web Apps 2013**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-033**](http://go.microsoft.com/fwlink/?linkid=532628)
</td>
<td style="border:1px solid black;">
[**MS15-036**](http://go.microsoft.com/fwlink/?linkid=532634)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2013 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2013 Service Pack 1  
(2965306)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis zu MS15-033 und MS15-036**

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

Weitere Informationen:
----------------------

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

-   V1.0 (14. April 2015): Bulletin Summary veröffentlicht.

*Seite generiert am 13.04.2015 um 11:48Z-07:00.*
