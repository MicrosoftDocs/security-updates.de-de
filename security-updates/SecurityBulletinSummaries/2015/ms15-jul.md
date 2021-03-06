---
TOCTitle: 'MS15-JUL'
Title: Microsoft Security Bulletin Summary für Juli 2015
ms:assetid: 'ms15-jul'
ms:contentKeyID: 66484718
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms15-jul(v=Security.10)'
---

Microsoft Security Bulletin Summary für Juli 2015
=================================================

Veröffentlicht: 14. Juli 2015 | Aktualisiert: 25. Mai 2016

**Version:** 3.1

In diesem Bulletin Summary sind die im Juli 2015 veröffentlichten Sicherheitsbulletins aufgeführt.

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft-Sicherheitsbulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

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
und Auswirkung der Sicherheitsanfälligkeit</strong></td>
<td style="border:1px solid black;"><strong>Neustartanforderung</strong></td>
<td style="border:1px solid black;"><strong>Bekannte<br />
Probleme</strong></td>
<td style="border:1px solid black;"><strong>Betroffene Software</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-058">MS15-058</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SQL Server können Remotecodeausführung ermöglichen (3065718)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft SQL Server. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein authentifizierter Angreifer eine speziell gestaltete Abfrage ausführt, die darauf ausgelegt ist, eine virtuelle Funktion von einer falschen Adresse auszuführen, was zu einem Funktionsaufruf in nicht initialisiertem Speicher führt. Um diese Sicherheitsanfälligkeit ausnutzen zu können, benötigt der Angreifer Berechtigungen zum Erstellen oder Ändern einer Datenbank.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3065718">3065718</a></td>
<td style="border:1px solid black;">Microsoft SQL Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Internet Explorer (3076321)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-066">MS15-066</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im VBScript-Skriptmodul kann Remotecodeausführung ermöglichen (3072604)</strong> <br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit im VBScript-Skriptmodul in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Website besucht. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Wenn der aktuelle Benutzer mit Administratorrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, die vollständige Kontrolle über ein betroffenes System übernehmen. Der Angreifer könnte dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit uneingeschränkten Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-067">MS15-067</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in RDP kann Remotecodeausführung ermöglichen (3073094)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit könnte Remotecodeausführung ermöglichen, wenn ein Angreifer eine Reihe speziell gestalteter Pakete an ein Zielsystem sendet, auf dem RDP (Remotedesktopprotokoll) aktiviert ist. Standardmäßig ist RDP in keinem Windows-Betriebssystem aktiviert. Systeme, bei denen RDP nicht aktiviert ist, sind nicht gefährdet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-068">MS15-068</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows Hyper-V können Remotecodeausführung ermöglichen (3072000)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Remotecodeausführung in einem Hostkontext ermöglichen, wenn von einem authentifizierten Benutzer mit Administratorrechten auf einem virtuellen Gastcomputer, der von Hyper-V gehostet wird, eine speziell gestaltete Anwendung ausgeführt wird. Ein Angreifer muss über gültige Anmeldeinformationen für einen virtuellen Gastcomputer verfügen, um diese Sicherheitsanfälligkeit ausnutzen zu können.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-069">MS15-069</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Windows können Remotecodeausführung ermöglichen (3072631)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Angreifer zunächst eine speziell gestaltete DLL-Datei (Dynamic Link Library) in das aktuelle Arbeitsverzeichnis des Zielbenutzers einfügt und den Benutzer dann dazu verleitet, eine RTF-Datei zu öffnen oder ein Programm zu starten, die bzw. das darauf ausgelegt ist, eine vertrauenswürdige DLL zu laden, stattdessen jedoch die speziell gestaltete DLL-Datei lädt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, könnte die vollständige Kontrolle über das betroffene System erlangen. Der Angreifer könnte dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit uneingeschränkten Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (3072620)</strong> <br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-071">MS15-071</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Netlogon kann eine Erhöhung von Berechtigungen ermöglichen (3068457)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer mit Zugriff auf einen primären Domänencontroller (PDC) in einem Zielnetzwerk eine speziell gestaltete Anwendung ausführt, um als Reservedomänencontroller einen sicheren Verbindungskanal mit dem PDC einzurichten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-072">MS15-072</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Grafikkomponente kann eine Erhöhung von Berechtigungen ermöglichen (3069392)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn die Grafikkomponente von Windows Bitmapkonvertierungen nicht ordnungsgemäß verarbeitet. Ein authentifizierter Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann seine Berechtigungen auf einem Zielsystem erhöhen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen. Ein Angreifer muss sich zunächst am System anmelden, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-073">MS15-073</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Kernelmodustreiber kann eine Erhöhung von Berechtigungen ermöglichen(3070102)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet und eine speziell entworfene Anwendung ausführt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-074">MS15-074</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows-Installationsdienst kann eine Erhöhung von Berechtigungen ermöglichen (3072630)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn der Windows-Installationsdienst Skripts für benutzerdefinierte Aktionen nicht ordnungsgemäß ausführt. Ein Angreifer muss zunächst Zugriff auf das Konto eines beim Zielsystem angemeldeten Benutzers erlangen, um die Sicherheitsanfälligkeit ausnutzen zu können. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-075">MS15-075</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in OLE können eine Erhöhung von Berechtigungen ermöglichen (3072633)</strong><br />
Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sie in Verbindung mit einer anderen Sicherheitsanfälligkeit, welche die Ausführung beliebigen Codes ermöglicht, ausgenutzt werden. Nachdem die andere Sicherheitsanfälligkeit ausgenutzt wurde, kann der Angreifer dann die in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten ausnutzen, um zu bewirken, dass beliebiger Code auf einer mittleren Integritätsebene ausgeführt wird.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-076">MS15-076</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Remoteprozeduraufruf kann eine Erhöhung von Berechtigungen ermöglichen (3067505)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit, die in der Windows RPC-Authentifizierung (Remote Procedure Call) vorliegt, kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem System anmeldet und eine speziell entworfene Anwendung ausführt. Wenn ein Angreifer diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann er die vollständige Kontrolle über das betroffene System erlangen. Der Angreifer könnte dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit uneingeschränkten Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;"><a href="https://support.microsoft.com/de-de/kb/3067505">3067505</a></td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-077">MS15-077</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im ATM-Schriftartentreiber kann eine Erhöhung von Berechtigungen ermöglichen (3077657)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem Zielsystem anmeldet und eine speziell entworfene Anwendung ausführt. Ein Angreifer, der diese Sicherheitsanfälligkeit ausnutzt, könnte im Ernstfall die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-078">MS15-078</a><br />
(Außerplanmäßige Veröffentlichung am 20. Juli 2015)</td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Microsoft-Schriftartentreiber kann Remotecodeausführung ermöglichen (3079904)</strong> <br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Windows. Das Sicherheitsrisiko kann Remotecodeausführung ermöglichen, wenn ein Benutzer ein speziell gestaltetes Dokument öffnet oder eine nicht vertrauenswürdige Website besucht, das bzw. die eingebettete OpenType-Schriftarten enthält.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-058">MS15-058</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in SQL Server bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1761">CVE-2015-1761</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-058">MS15-058</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in SQL Server bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1762">CVE-2015-1762</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-058">MS15-058</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in SQL Server bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1763">CVE-2015-1763</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1729">CVE-2015-1729</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1733">CVE-2015-1733</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1738">CVE-2015-1738</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-1767">CVE-2015-1767</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in VBScript bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2372">CVE-2015-2372</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2383">CVE-2015-2383</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2384">CVE-2015-2384</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2385">CVE-2015-2385</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2388">CVE-2015-2388</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2389">CVE-2015-2389</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2390">CVE-2015-2390</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2391">CVE-2015-2391</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2397">CVE-2015-2397</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Umgehung des XSS-Filters in Internet Explorer</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2398">CVE-2015-2398</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2401">CVE-2015-2401</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2402">CVE-2015-2402</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2403">CVE-2015-2403</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2404">CVE-2015-2404</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2406">CVE-2015-2406</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2408">CVE-2015-2408</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2410">CVE-2015-2410</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2411">CVE-2015-2411</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2412">CVE-2015-2412</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2413">CVE-2015-2413</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2414">CVE-2015-2414</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Jscript9-Sicherheitsanfälligkeit durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2419">CVE-2015-2419</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">ASLR-Umgehung durch Internet Explorer</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2421">CVE-2015-2421</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2422">CVE-2015-2422</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-065">MS15-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2425">CVE-2015-2425</a></td>
<td style="border:1px solid black;">0 – Ausnutzung erkannt</td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-066">MS15-066</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in VBScript bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2372">CVE-2015-2372</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-067">MS15-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Remotedesktopprotokoll (RDP) bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2373">CVE-2015-2373</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-068">MS15-068</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Hyper-V bezüglich Pufferüberlauf</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2361">CVE-2015-2361</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-068">MS15-068</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Hyper-V bezüglich Systemdatenstrukturen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2362">CVE-2015-2362</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-069">MS15-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows bezüglich Remotecodeausführung durch DLL</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2368">CVE-2015-2368</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-069">MS15-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung durch DLL-Positionierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2369">CVE-2015-2369</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Excel durch Umgehung der ASLR-Sicherheitsfunktion</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2375">CVE-2015-2375</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2376">CVE-2015-2376</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2377">CVE-2015-2377</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Excel bezüglich Remotecodeausführung durch DLL</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2378">CVE-2015-2378</a></td>
<td style="border:1px solid black;">4 – Nicht betroffen</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2379">CVE-2015-2379</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2380">CVE-2015-2380</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2415">CVE-2015-2415</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-070">MS15-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2424">CVE-2015-2424</a></td>
<td style="border:1px solid black;">0 – Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 – Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-071">MS15-071</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Netlogon bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2374">CVE-2015-2374</a></td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 – Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-072">MS15-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Grafikkomponente bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2364">CVE-2015-2364</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-073">MS15-073</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2363">CVE-2015-2363</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-073">MS15-073</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2365">CVE-2015-2365</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-073">MS15-073</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2366">CVE-2015-2366</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-073">MS15-073</a></td>
<td style="border:1px solid black;">Win32k-Sicherheitsanfälligkeit für die Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2367">CVE-2015-2367</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-073">MS15-073</a></td>
<td style="border:1px solid black;">Win32k-Sicherheitsanfälligkeit für die Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2381">CVE-2015-2381</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-073">MS15-073</a></td>
<td style="border:1px solid black;">Win32k-Sicherheitsanfälligkeit für die Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2382">CVE-2015-2382</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-074">MS15-074</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Installer bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2371">CVE-2015-2371</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-075">MS15-075</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OLE bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2416">CVE-2015-2416</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-075">MS15-075</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OLE bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2417">CVE-2015-2417</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-076">MS15-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows RPC bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2370">CVE-2015-2370</a></td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 – Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-077">MS15-077</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in ATMFD.DLL durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2387">CVE-2015-2387</a></td>
<td style="border:1px solid black;">0 – Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 – Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms15-078">MS15-078</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im OpenType-Schriftartentreiber</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-2426">CVE-2015-2426</a></td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 – Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
</tr>
</tbody>
</table>
  
Betroffene Software  
-------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.
  
**Hinweis** Für eine Sicherheitsanfälligkeit müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
### Windows-Betriebssystem und -Komponenten (Tabelle 1 von 3)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://technet.microsoft.com/de-de/library/security/ms15-069)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)                                          
</td>
<td style="border:1px solid black;">
**Nicht bewertet**                                             
</td>
<td style="border:1px solid black;">
**Nicht bewertet**                                             
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
Internet Explorer 6  
(3065822)  
(Mittel)  
Internet Explorer 7  
(3065822)  
(Mittel)  
Internet Explorer 8  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.6  
(3068404)  
(Kritisch)  
VBScript 5.7  
(3068368)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3067903)  
(Hoch)  
Windows Media Format SDK 11  
(3067903)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3065822)  
(Mittel)  
Internet Explorer 7  
(3065822)  
(Mittel)  
Internet Explorer 8  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.6  
(3068404)  
(Kritisch)  
VBScript 5.7  
(3068368)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3067903)  
(Hoch)  
Windows Media Format SDK 11  
(3067903)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3065822)  
(Mittel)  
Internet Explorer 7  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.6  
(3068404)  
(Kritisch)  
VBScript 5.7  
(3068368)  
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
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 R2 Service Pack 2
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
Windows Server 2003 R2 Service Pack 2  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 R2 x64 Edition Service Pack 2
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
Windows Server 2003 R2 x64 Edition Service Pack 2  
(3068457)  
(Hoch)
</td>
</tr>
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
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://technet.microsoft.com/de-de/library/security/ms15-069)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3065822)  
(Kritisch)  
Internet Explorer 8  
(3065822)  
(Kritisch)  
Internet Explorer 9  
(3065822)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.7  
(3068368)  
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
(3067903)  
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
(3065822)  
(Kritisch)  
Internet Explorer 8  
(3065822)  
(Kritisch)  
Internet Explorer 9  
(3065822)  
(Kritisch)
</td>
<td style="border:1px solid black;">
VBScript 5.7  
(3068368)  
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
(3067903)  
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
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://go.microsoft.com/fwlink/?linkid=??????)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3065822)  
(Mittel)  
Internet Explorer 8  
(3065822)  
(Mittel)  
Internet Explorer 9  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.7  
(3068368)  
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
(3067903)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3065822)  
(Mittel)  
Internet Explorer 8  
(3065822)  
(Mittel)  
Internet Explorer 9  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.7  
(3068368)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3046339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3067903)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
VBScript 5.7  
(3068368)  
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
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3068457)  
(Hoch)
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
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://go.microsoft.com/fwlink/?linkid=??????)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3065822)  
(Kritisch)  
Internet Explorer 9  
(3065822)  
(Kritisch)  
Internet Explorer 10  
(3065822)  
(Kritisch)  
Internet Explorer 11  
(3065822)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3067904)  
(Kritisch)  
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3069762)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3067903)  
(Hoch)  
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3070738)  
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
(3065822)  
(Kritisch)  
Internet Explorer 9  
(3065822)  
(Kritisch)  
Internet Explorer 10  
(3065822)  
(Kritisch)  
Internet Explorer 11  
(3065822)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3067904)  
(Kritisch)  
Windows 7 für x64-basierte Systeme Service Pack 1  
(3069762)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3067903)  
(Hoch)  
Windows 7 für x64-basierte Systeme Service Pack 1  
(3070738)  
(Hoch)
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
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://go.microsoft.com/fwlink/?linkid=??????)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3065822)  
(Mittel)  
Internet Explorer 9  
(3065822)  
(Mittel)  
Internet Explorer 10  
(3065822)  
(Mittel)  
Internet Explorer 11  
(3065822)  
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
(3046339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3067903)  
(Hoch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3070738)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3065822)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://go.microsoft.com/fwlink/?linkid=??????)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3065822)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3067904)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3065822)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3067904)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3046339)  
(Kritisch)
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
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3065822)  
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
Windows 8.1 für 32-Bit-Systeme  
(3061512)  
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
Internet Explorer 11  
(3065822)  
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
(3046339)  
(Kritisch)  
Windows 8.1 für x64-basierte Systeme  
(3046359)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3061512)  
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
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://technet.microsoft.com/de-de/library/security/ms15-069)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3067904)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3046339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3065822)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3046339)  
(Kritisch)  
Windows Server 2012 R2  
(3046359)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3061512)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3068457)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://go.microsoft.com/fwlink/?linkid=??????)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3065822)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3065822)  
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
(3061512)  
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
[**MS15-065**](https://technet.microsoft.com/de-de/library/security/ms15-065)
</td>
<td style="border:1px solid black;">
[**MS15-066**](https://technet.microsoft.com/de-de/library/security/ms15-066)
</td>
<td style="border:1px solid black;">
[**MS15-067**](https://technet.microsoft.com/de-de/library/security/ms15-067)
</td>
<td style="border:1px solid black;">
[**MS15-068**](https://technet.microsoft.com/de-de/library/security/ms15-068)
</td>
<td style="border:1px solid black;">
[**MS15-069**](https://go.microsoft.com/fwlink/?linkid=??????)
</td>
<td style="border:1px solid black;">
[**MS15-071**](https://technet.microsoft.com/de-de/library/security/ms15-071)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
VBScript 5.7  
(3068368)  
(Keine Bewertung des Schweregrads)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3068457)  
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
VBScript 5.7  
(3068368)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3046339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3068457)  
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
VBScript 5.8  
(3068364)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3046339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3068457)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3067904)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3046339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3068457)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3046339)  
(Kritisch)  
Windows Server 2012 R2 (Server Core-Installation)  
(3046359)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3068457)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-067**

Enterprise- und Ultimate-Editionen von Windows 7 sind betroffen. Alle unterstützten Editionen von Windows 7 sind betroffen, wenn RDP 8.0 auf dem System installiert ist.

**Hinweis zu MS15-069**

Für das Update 3067903 gilt, dass Systeme mit Windows Server 2008 oder Windows Server 2008 R2 nur dann betroffen sind, wenn „Desktopdarstellung“ installiert worden ist.

Für das Update 3070738 gilt, dass Systeme nur dann betroffen sind, wenn RDP 8.1 installiert worden ist.

### Windows-Betriebssystem und -Komponenten (Tabelle 2 von 3)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx) 
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 R2 Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 R2 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 x64 Edition Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 x64 Edition Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 x64 Edition Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 R2 x64 Edition Service Pack 2  
(3067505)  
(Hoch)
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
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3077657)  
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
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3077657)  
(Hoch)
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
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3077657)  
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
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Windows RT  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3077657)  
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
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3074683)  
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
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3074683)  
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
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-072**](https://technet.microsoft.com/de-de/library/security/ms15-072)
</td>
<td style="border:1px solid black;">
[**MS15-073**](https://technet.microsoft.com/de-de/library/security/ms15-073)
</td>
<td style="border:1px solid black;">
[**MS15-074**](https://technet.microsoft.com/de-de/library/security/ms15-074)
</td>
<td style="border:1px solid black;">
[**MS15-075**](https://technet.microsoft.com/de-de/library/security/ms15-075)
</td>
<td style="border:1px solid black;">
[**MS15-076**](https://technet.microsoft.com/de-de/library/security/ms15-076)
</td>
<td style="border:1px solid black;">
[**MS15-077**](https://technet.microsoft.com/de-de/library/security/ms15-077)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3077657)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3069392)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3070102)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3072630)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3072633)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3067505)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3077657)  
(Hoch)
</td>
</tr>
</table>
 
### Windows-Betriebssystem und -Komponenten (Tabelle 3 von 3)

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows Server 2012
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows RT
</td>
<td style="border:1px solid black;">
Windows RT  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme  
(3074683)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme  
(3074683)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-078**](https://technet.microsoft.com/de-de/library/security/ms15-078)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3079904)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3079904)  
(Kritisch)
</td>
</tr>
</table>
 
### Microsoft SQL Server

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**SQL Server 2008 Service Pack 3**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-058**](https://technet.microsoft.com/de-de/library/security/ms15-058)
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
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 3  
(GDR)  
(3045305)  
(Hoch)  
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 3  
(QFE)  
(3045303)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 3  
(GDR)  
(3045305)  
(Hoch)  
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 3  
(QFE)  
(3045303)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für Itanium-basierte Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für Itanium-basierte Systeme Service Pack 3  
(GDR)  
(3045305)  
(Hoch)  
Microsoft SQL Server 2008 für Itanium-basierte Systeme Service Pack 3  
(QFE)  
(3045303)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**SQL Server 2008 Service Pack 4**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-058**](https://technet.microsoft.com/de-de/library/security/ms15-058)
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
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 4
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 4  
(GDR)  
(3045311)  
(Hoch)  
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 4  
(QFE)  
(3045308)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 4
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 4  
(GDR)  
(3045311)  
(Hoch)  
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 4  
(QFE)  
(3045308)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**SQL Server 2008 R2 Service Pack 2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-058**](https://technet.microsoft.com/de-de/library/security/ms15-058)
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
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 2  
(GDR)  
(3045313)  
(Hoch)  
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 2  
(QFE)  
(3045312)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 2  
(GDR)  
(3045313)  
(Hoch)  
Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 2  
(QFE)  
(3045312)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für Itanium-basierte Systeme Service Pack 2  
(GDR)  
(3045313)  
(Hoch)  
Microsoft SQL Server 2008 R2 für Itanium-basierte Systeme Service Pack 2  
(QFE)  
(3045312)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**SQL Server 2008 R2 Service Pack 3**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-058**](https://technet.microsoft.com/de-de/library/security/ms15-058)
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
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 3  
(GDR)  
(3045316)  
(Hoch)  
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 3  
(QFE)  
(3045314)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 3  
(GDR)  
(3045316)  
(Hoch)  
Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 3  
(QFE)  
(3045314)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**SQL Server 2012 Service Pack 1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-058**](https://technet.microsoft.com/de-de/library/security/ms15-058)
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
Microsoft SQL Server 2012 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2012 für 32-Bit-Systeme Service Pack 1  
(GDR)  
(3045318)  
(Hoch)  
Microsoft SQL Server 2012 für 32-Bit-Systeme Service Pack 1  
(QFE)  
(3045317)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2012 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2012 für x64-basierte Systeme Service Pack 1  
(GDR)  
(3045318)  
(Hoch)  
Microsoft SQL Server 2012 für x64-basierte Systeme Service Pack 1  
(QFE)  
(3045317)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**SQL Server 2012 Service Pack 2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-058**](https://technet.microsoft.com/de-de/library/security/ms15-058)
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
Microsoft SQL Server 2012 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2012 für 32-Bit-Systeme Service Pack 2  
(GDR)  
(3045321)  
(Hoch)  
Microsoft SQL Server 2012 für 32-Bit-Systeme Service Pack 2  
(QFE)  
(3045319)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2012 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2012 für x64-basierte Systeme Service Pack 2  
(GDR)  
(3045321)  
(Hoch)  
Microsoft SQL Server 2012 für x64-basierte Systeme Service Pack 2  
(QFE)  
(3045319)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**SQL Server 2014**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-058**](https://technet.microsoft.com/de-de/library/security/ms15-058)
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
Microsoft SQL Server 2014 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2014 für 32-Bit-Systeme  
(GDR)  
(3045324)  
(Hoch)  
Microsoft SQL Server 2014 für 32-Bit-Systeme  
(QFE)  
(3045323)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2014 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Microsoft SQL Server 2014 für x64-basierte Systeme  
(GDR)  
(3045324)  
(Hoch)  
Microsoft SQL Server 2014 für x64-basierte Systeme  
(QFE)  
(3045323)  
(Hoch)
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
Microsoft Excel 2007 Service Pack 3  
(2965281)  
(Hoch)  
Microsoft PowerPoint 2007 Service Pack 3  
(2965283)  
(Hoch)  
Microsoft Word 2007 Service Pack 3  
(3054996)  
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
(3054971)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(3054981)  
(Hoch)  
Microsoft PowerPoint 2010 Service Pack 2 (32-Bit-Editionen)  
(3054963)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(3054973)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(3054971)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(3054981)  
(Hoch)  
Microsoft PowerPoint 2010 Service Pack 2 (64-Bit-Editionen)  
(3054963)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(3054973)  
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
Microsoft Excel 2013 Service Pack 1 (32-Bit-Editionen)  
(3054949)  
(Hoch)  
Microsoft PowerPoint 2013 Service Pack 1 (32-Bit-Editionen)  
(3054999)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (32-Bit-Editionen)  
(3054990)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 Service Pack 1 (64-Bit-Editionen)  
(3054949)  
(Hoch)  
Microsoft PowerPoint 2013 Service Pack 1 (64-Bit-Editionen)  
(3054999)  
(Hoch)  
Microsoft Word 2013 Service Pack 1 (64-Bit-Editionen)  
(3054990)  
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
Microsoft Excel 2013 RT Service Pack 1  
(3054949)  
(Hoch)  
Microsoft PowerPoint 2013 RT Service Pack 1  
(3054999)  
(Hoch)  
Microsoft Word 2013 RT Service Pack 1  
(3054990)  
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
Microsoft Excel für Mac 2011  
(3073865)  
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
Microsoft Office Excel Viewer 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer 2007 Service Pack 3  
(2965209)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2965208)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(3054958)  
(Hoch)
</td>
</tr>
</table>
 
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
(2837612)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Excel Services  
(2837612)  
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
(3054968)  
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
[**MS15-070**](https://technet.microsoft.com/de-de/library/security/ms15-070)
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
(3054861)  
(Hoch)
</td>
</tr>
</table>
 

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

-   V1.0 (14. Juli 2015): Bulletin Summary veröffentlicht.
-   V2.0 (20. Juli 2015): Das Bulletin Summary wurde zur Dokumentation der außerplanmäßigen Veröffentlichung von MS15-078 überarbeitet.
-   V3.0 (29. Juli 2015): Das Bulletin Summary wurde für MS15-074 und MS15-078 überarbeitet, um die Verfügbarkeit eines Updatepakets für Windows 10-Systeme bekannt zu geben. Benutzer, die Windows 10 ausführen, sollten das Update 3074683 installieren, um vor den in diesen Bulletins beschriebenen Sicherheitsanfälligkeiten geschützt zu sein. Das Update ist nur über Windows Update erhältlich. Die meisten Kunden haben automatische Updates aktiviert und müssen nichts weiter tun, weil das Update automatisch heruntergeladen und installiert wird.
-   V3.1 (25. Mai 2016): Bei MS15-076 wurde der Tabelle mit Kurzzusammenfassungen ein Verweis auf bekannte Probleme hinzugefügt. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 3067505](https://support.microsoft.com/de-de/kb/3067505). Informationen zur Lösung dieses bekannten Problems finden Sie im [Microsoft Knowledge Base-Artikel 3155218](https://support.microsoft.com/de-de/kb/3155218).

*Seite generiert am 25.05.2016 um 10:57Z-07:00.*
