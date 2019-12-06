---
TOCTitle: 'MS15-JAN'
Title: Microsoft Security Bulletin Summary für Januar 2015
ms:assetid: 'ms15-jan'
ms:contentKeyID: 63898314
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms15-jan(v=Security.10)'
---

Microsoft Security Bulletin Summary für Januar 2015
===================================================

Veröffentlicht: 13. Januar 2015

**Version:** 1.0

In diesem Bulletin Summary sind die im Januar 2015 veröffentlichten Security Bulletins aufgeführt.

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Security Bulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im nächsten Abschnitt **Betroffene Software**.

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522536">MS15-001</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko in Windows Application Compatibility-Cache kann Rechteerweiterungen ermöglichen (3023266)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt ein öffentlich gemeldetes Sicherheitsrisiko in Microsoft Windows. Das Sicherheitsrisiko kann Rechteerweiterungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein authentifizierter Angreifer, der dieses Sicherheitsrisiko erfolgreich ausnutzt, kann vorhandene Berechtigungsprüfungen, die während der Cacheänderung in der Komponente Microsoft Windows Application Compatibility durchgeführt werden, umgehen und beliebigen Code mit erhöhten Berechtigungen ausführen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522537">MS15-002</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko im Windows-Telnetdienst kann Remotecodeausführung ermöglichen (3020393)</strong><br />
<br />
Dieses Sicherheitsupdate behebt ein vertraulich gemeldetes Sicherheitsrisiko in Microsoft Windows. Das Sicherheitsrisiko kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine Reihe speziell gestalteter Pakete an einen betroffenen Windows-Server sendet. Standardmäßig wird Telnet unter keiner Version der betroffenen Betriebssysteme installiert. Nur Computer von Kunden, die diesen Dienst manuell installieren, können anfällig sein.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch </a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522528">MS15-003</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko in Windows-User Profile Service kann Rechteerweiterungen ermöglichen (3021674)</strong><br />
<br />
Dieses Sicherheitsupdate behebt ein öffentlich gemeldetes Sicherheitsrisiko in Microsoft Windows. Das Sicherheitsrisiko kann Rechteerweiterungen ermöglichen, wenn ein Angreifer sich bei dem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein lokaler Angreifer, der dieses Sicherheitsrisiko erfolgreich ausnutzt, kann auf einem Zielsystem beliebigen Code mit höheren Berechtigungen ausführen. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um dieses Sicherheitsrisiko auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522521">MS15-004</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko in Windows-Komponenten kann Rechteerweiterungen ermöglichen (3025421)</strong><br />
<br />
Dieses Sicherheitsupdate behebt ein vertraulich gemeldetes Sicherheitsrisiko in Microsoft Windows. Das Sicherheitsrisiko kann Rechteerweiterungen ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, eine speziell gestaltete Anwendung auszuführen. Ein Angreifer, der das Sicherheitsrisiko erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Wenn der aktuelle Benutzer mit Administratorbenutzerrechten angemeldet ist, kann ein Angreifer Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für jene, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522531">MS15-005</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko im Dienst für Netzwerkadressinformationen kann Umgehung von Sicherheitsfunktionen ermöglichen (3022777)</strong><br />
<br />
Dieses Sicherheitsupdate behebt ein vertraulich gemeldetes Sicherheitsrisiko in Microsoft Windows. Das Sicherheitsrisiko kann die Umgehung von Sicherheitsfunktionen ermöglichen, indem die Firewallrichtlinie und/oder die Konfiguration bestimmter Dienste ungewollt gelockert wird, wenn ein Angreifer im selben Netzwerk wie das Opfer Antworten auf vom Opfer initiierten DNS- und LDAP-Verkehr vortäuscht.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522535">MS15-006</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko in Windows-Fehlerberichterstattung kann Umgehung der Sicherheitsfunktion ermöglichen (3004365)</strong><br />
<br />
Dieses Sicherheitsupdate behebt ein vertraulich gemeldetes Sicherheitsrisiko in der Windows-Fehlerberichterstattung (WER: Windows Error Reporting). Das Sicherheitsrisiko kann die Umgehung von Sicherheitsfunktionen ermöglichen, wenn es von einem Angreifer erfolgreich ausgenutzt wird. Ein Angreifer, der dieses Sicherheitsrisiko erfolgreich ausnutzt, kann Zugriff auf den Arbeitsspeicher eines zurzeit ausgeführten Prozesses erlangen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=519134">MS15-007</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko in RADIUS-Implementierung des Netzwerkrichtlinienservers kann Denial-of-Service-Angriffe ermöglichen (3014029)</strong><br />
<br />
Dieses Sicherheitsupdate behebt ein vertraulich gemeldetes Sicherheitsrisiko in Microsoft Windows. Das Sicherheitsrisiko kann einen Denial-of-Service-Angriff auf einen Internetauthentifizierungsdienst (IAS: Internet Authentication Service) oder Netzwerkrichtlinienserver (NPS: Network Policy Server) ermöglichen, wenn ein Angreifer speziell gestaltete Benutzernamenszeichenfolgen an den IAS oder NPS sendet. Beachten Sie, dass ein Sicherheitsrisiko vom Typ Denial-of-Service einem Angreifer keine Codeausführung oder Rechteerweiterungen ermöglicht. Allerdings kann dadurch die RADIUS-Authentifizierung auf dem IAS oder NPS verhindert werden.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522533">MS15-008</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsrisiko in Windows-Kernelmodustreiber kann Rechteerweiterungen ermöglichen (3019215)</strong><br />
<br />
Dieses Sicherheitsupdate behebt ein vertraulich gemeldetes Sicherheitsrisiko in Microsoft Windows. Das Sicherheitsrisiko kann Rechterweiterungen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anwendung auf einem betroffenen System ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um dieses Sicherheitsrisiko auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
 
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsrisiken bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsrisiken sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Im Ausnutzbarkeitsindex sind nur Sicherheitsrisiken enthalten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
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
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit für ältere Softwareversionen</strong></td>
<td style="border:1px solid black;"><strong>Bewertung der Ausnutzbarkeit durch Denial-of-Service</strong></td>
<td style="border:1px solid black;"><strong>Wichtige Hinweise</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522536">MS15-001</a></td>
<td style="border:1px solid black;">Sicherheitsrisiko in Windows Application Compatibility-Infrastruktur bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0002">CVE-2015-0002</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dieses Sicherheitsrisiko wurde öffentlich bekannt gegeben.<br />
<br />
Dieses Sicherheitsrisiko kann für die Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522537">MS15-002</a></td>
<td style="border:1px solid black;">Pufferüberlauf-Sicherheitsrisiko beim Windows-Telnetdienst</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0014">CVE-2015-0014</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Dieses Sicherheitsrisiko kann Remotecodeausführung ermöglichen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522528">MS15-003</a></td>
<td style="border:1px solid black;">Sicherheitsrisiko in Windows-User Profile Service bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0004">CVE-2015-0004</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dieses Sicherheitsrisiko wurde öffentlich bekannt gegeben.<br />
<br />
Dieses Sicherheitsrisiko kann für die Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522521">MS15-004</a></td>
<td style="border:1px solid black;">Sicherheitsrisiko durch Verzeichnisüberquerung kann Rechteerweiterungen ermöglichen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0016">CVE-2015-0016</a></td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dieses Sicherheitsrisiko kann für die Erhöhung von Berechtigungen ausgenutzt werden.<br />
<br />
Dieses Sicherheitsrisiko wird in begrenzten, gezielten Angriffen als Sandbox-Umgehung verwendet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522531">MS15-005</a></td>
<td style="border:1px solid black;">Sicherheitsrisiko in NLA bezüglich Umgehung von Sicherheitsfunktionen – CVE-2015-0006</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0006">CVE-2015-0006</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dies ist ein Sicherheitsrisiko, das eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522535">MS15-006</a></td>
<td style="border:1px solid black;">Sicherheitsrisiko in Windows-Fehlerberichterstattung kann Umgehung der Sicherheitsfunktion ermöglichen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0001">CVE-2015-0001</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dies ist ein Sicherheitsrisiko, das eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=519134">MS15-007</a></td>
<td style="border:1px solid black;">Sicherheitsrisiko in RADIUS-Implementierung von Netzwerkrichtlinienserver bezüglich Denial-of-Service-Angriffen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0015">CVE-2015-0015</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Dieses Sicherheitsrisiko kann auch zu einer Dienstverweigerung (Denial-of-Service) führen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522533">MS15-008</a></td>
<td style="border:1px solid black;">WebDAV-Sicherheitsrisiko bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0011">CVE-2015-0011</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dieses Sicherheitsrisiko kann für die Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
</tbody>
</table>
  
 
  
Betroffene Software  
-------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.
  
**Hinweis** Für ein Sicherheitsrisiko müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3019215)  
(Hoch)
</td>
</tr>
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
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2 (mit installiertem Remotedesktop-Client 7.0)  
(3023299)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3019215)  
(Hoch)
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
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2 (mit installiertem Remotedesktop-Client 7.0)  
(3023299)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3019215)  
(Hoch)
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
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3019215)  
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
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3022777)  
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
<td style="border:1px solid black;" colspan="9">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3019978)  
(Hoch)  
Windows 7 für 32--Bit-Systeme Service Pack 1 (mit installiertem Remotedesktop-Client 8.0)  
(3020387)  
(Hoch)  
Windows 7 für 32--Bit-Systeme Service Pack 1 (mit installiertem Remotedesktop-Client 8.1)  
(3020388)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3022777)  
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
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3019978)  
(Hoch)  
Windows 7 für x64-basierte Systeme Service Pack 1 (mit installiertem Remotedesktop-Client 8.0)  
(3020387)  
(Hoch)  
Windows 7 für x64-basierte Systeme Service Pack 1 (mit installiertem Remotedesktop-Client 8.1)  
(3020388)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3022777)  
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
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3019978)  
(Hoch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (mit installiertem Remotedesktop-Client 8.0)  
(3020387)  
(Hoch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (mit installiertem Remotedesktop-Client 8.1)  
(3020388)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3022777)  
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
<td style="border:1px solid black;" colspan="9">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3022777) )  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3022777) )  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3022777) )  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3019215)  
(Hoch)
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
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3014029)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="9">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Windows RT  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(3019215)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3019215)  
(Hoch)
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
[**MS15-001**](https://go.microsoft.com/fwlink/?linkid=522536)
</td>
<td style="border:1px solid black;">
[**MS15-002**](https://go.microsoft.com/fwlink/?linkid=522537)
</td>
<td style="border:1px solid black;">
[**MS15-003**](https://go.microsoft.com/fwlink/?linkid=522528)
</td>
<td style="border:1px solid black;">
[**MS15-004**](https://go.microsoft.com/fwlink/?linkid=522521)
</td>
<td style="border:1px solid black;">
[**MS15-005**](https://go.microsoft.com/fwlink/?linkid=522531)
</td>
<td style="border:1px solid black;">
[**MS15-006**](https://go.microsoft.com/fwlink/?linkid=522535)
</td>
<td style="border:1px solid black;">
[**MS15-007**](https://go.microsoft.com/fwlink/?linkid=519134)
</td>
<td style="border:1px solid black;">
[**MS15-008**](https://go.microsoft.com/fwlink/?linkid=522533)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
<td style="border:1px solid black;">
**Keine**
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
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3022777)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3022777)  
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
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3022777)  
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
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3004365)  
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
Windows Server 2012 R2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3023266)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3020393)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3021674)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3019978)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3022777)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3004365)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis zu MS15-005**  
<sup>[1]</sup>Windows Server 2003 ist betroffen, aber es wurde kein Update veröffentlicht. Weitere Informationen finden Sie im Bulletin.

Tools und Hinweise zur Erkennung und Bereitstellung von Sicherheitsupdates
--------------------------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter.

Windows Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager erleichtern Administratoren die Verteilung von Sicherheitsupdates.

Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](https://technet.microsoft.com/de-de/security/cc297183).

Danksagung
----------

Microsoft würdigt die Bemühungen derjenigen Benutzer der Sicherheitscommunity, die uns dabei helfen, Kunden durch eine verantwortliche Offenlegung von Sicherheitsrisiken zu schützen. Weitere Informationen finden Sie unter [Danksagung](https://technet.microsoft.com/de-de/library/security/dn820091.aspx). 

Weitere Informationen:
----------------------

### Microsoft Windows-Tool zum Entfernen bösartiger Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsrisiken bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsrisiken dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://technet.microsoft.com/de-de/security/dn467918) aufgeführt sind.

### Sicherheitsstrategien und Community

**Updateverwaltungsstrategien**

Auf der Seite [Patchmanagement](https://technet.microsoft.com/de-de/library/bb466251.aspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

### Support

Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://go.microsoft.com/fwlink/?linkid=21742), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.

Sicherheitslösungen für IT-Profis: [TechNet Security – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)

Hilfe beim Schützen des Computers, auf dem Windows ausgeführt wird, vor Viren und Schadsoftware: [Safety and Security Center](https://www.microsoft.com/de-de/security/default.aspx)

Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx?ln=de)

### Haftungsausschluss

Die Informationen in der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (13. Januar 2015): Bulletin Summary veröffentlicht.

*Seite generiert am 09.01.2015 15:31Z-08:00.*
