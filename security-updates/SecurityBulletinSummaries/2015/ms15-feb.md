---
TOCTitle: 'MS15-FEB'
Title: Microsoft Security Bulletin Summary für Februar 2015
ms:assetid: 'ms15-feb'
ms:contentKeyID: 64119060
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms15-feb(v=Security.10)'
---

Microsoft Security Bulletin Summary für Februar 2015
====================================================

Veröffentlicht: 10. Februar 2015

**Version:** 1.0

In diesem Bulletin Summary sind die im Februar 2015 veröffentlichten Security Bulletins aufgeführt.

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Internet Explorer (3034682)<br />
</strong><br />
Dieses Sicherheitsupdate behebt eine öffentlich bekannt gegebene und vierzig vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525535">MS15-010</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreiber können Remotecodeausführung ermöglichen (3036220)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und fünf vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, ein speziell gestaltetes Dokument zu öffnen oder eine nicht vertrauenswürdige Website zu besuchen, in das bzw. die TrueType-Schriftartdateien eingebettet sind.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525536">MS15-011</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Gruppenrichtlinie kann Remotecodeausführung ermöglichen (3000483)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer mit einem in eine Domäne eingebundenen System dazu verleitet, eine Verbindung mit einem vom Angreifer gesteuerten Netzwerk herzustellen. Ein Angreifer, der diese Sicherheitsanfälligkeit ausnutzt, könnte im Ernstfall die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525537">MS15-012</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (3032328)<br />
</strong><br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Benutzer mit Konten, die über weniger Systemrechte verfügen, sind davon möglicherweise weniger betroffen als Benutzer mit Administratorrechten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525533">MS15-013</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office kann Umgehung der Sicherheitsfunktion ermöglichen (3033857)<br />
</strong><br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann eine Umgehung der Sicherheitsfunktion ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Die Umgehung der Sicherheitsfunktion allein ermöglicht nicht die Ausführung von beliebigem Code. Ein Angreifer kann diese Sicherheitsanfälligkeit durch die Umgehung der Sicherheitsfunktion in Verbindung mit einer anderen Sicherheitsanfälligkeit verwenden, etwa eine Sicherheitsanfälligkeit bezüglich Remotecodeausführung, um beliebigen Code auszuführen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522532">MS15-014</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Gruppenrichtlinie kann Umgehung der Sicherheitsfunktion ermöglichen (3004361)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Umgehung der Sicherheitsfunktion ermöglichen, wenn es einem Angreifer durch einen Man-in-the-Middle-Angriff gelingt, die Richtliniendatei für das Gruppenrichtlinien-Sicherheitskonfigurationsmodul auf dem betroffenen System zu beschädigen oder unlesbar zu machen. Dies führt dazu, dass die Gruppenrichtlinieneinstellungen auf dem betroffenen System auf die Standardwerte und einen möglicherweise weniger sicheren Zustand zurückgesetzt werden.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525538">MS15-015</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Windows kann Rechteerweiterungen ermöglichen (3031432)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann es einem Angreifer ermöglichen, das Fehlen von Sicherheitsprüfungen bezüglich der Identitätswechselebene auszunutzen, um während der Prozesserstellung Berechtigungen zu erhöhen. Ein authentifizierter Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann Administratoranmeldeinformationen erlangen und diese zum Erhöhen von Berechtigungen verwenden. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525539">MS15-016</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Graphics-Komponente kann Offenlegung von Informationen ermöglichen (3029944)<br />
</strong><br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Diese Sicherheitsanfälligkeit kann die Offenlegung von Informationen ermöglichen, wenn ein Benutzer eine Website besucht, die speziell gestaltete TIFF-Inhalte enthält. Diese Sicherheitsanfälligkeit ermöglicht einem Angreifer keine Codeausführung oder direkte Erhöhung von Benutzerberechtigungen, sondern kann genutzt werden, um Informationen zu sammeln, mit denen das betroffene System noch weiter gefährdet werden könnte.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525540">MS15-017</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Virtual Machine Manager kann Rechteerweiterungen ermöglichen (3035898)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Virtual Machine Manager (VMM). Die Sicherheitsanfälligkeit kann Rechteerweiterungen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet. Ein Angreifer benötigt gültige Active Directory-Anmeldeinformationen und muss sich mit diesen Anmeldeinformationen anmelden können, um diese Sicherheitsanfälligkeit ausnutzen zu können.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Server-Software</td>
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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-8967">CVE-2014-8967</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich bekannt gegeben.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0017">CVE-2015-0017</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0018">CVE-2015-0018</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0019">CVE-2015-0019</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0020">CVE-2015-0020</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0021">CVE-2015-0021</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0022">CVE-2015-0022</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0023">CVE-2015-0023</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0025">CVE-2015-0025</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0026">CVE-2015-0026</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0027">CVE-2015-0027</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0028">CVE-2015-0028</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0029">CVE-2015-0029</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0030">CVE-2015-0030</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0031">CVE-2015-0031</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0035">CVE-2015-0035</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0036">CVE-2015-0036</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0037">CVE-2015-0037</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0038">CVE-2015-0038</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0039">CVE-2015-0039</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0040">CVE-2015-0040</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0041">CVE-2015-0041</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0042">CVE-2015-0042</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0043">CVE-2015-0043</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0044">CVE-2015-0044</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0045">CVE-2015-0045</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0046">CVE-2015-0046</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0048">CVE-2015-0048</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0049">CVE-2015-0049</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0050">CVE-2015-0050</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Umgehung der Internet Explorer ASLR</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0051">CVE-2015-0051</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0052">CVE-2015-0052</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0053">CVE-2015-0053</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0054">CVE-2015-0054</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0055">CVE-2015-0055</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0066">CVE-2015-0066</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0067">CVE-2015-0067</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0068">CVE-2015-0068</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Umgehung der Internet Explorer ASLR</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0069">CVE-2015-0069</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch domänenübergreifende Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0070">CVE-2015-0070</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525534">MS15-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Umgehung der Internet Explorer ASLR</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0071">CVE-2015-0071</a></td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Microsoft ist sich begrenzter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.<br />
<br />
Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525535">MS15-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0003">CVE-2015-0003</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525535">MS15-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in CNG bezüglich Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0010">CVE-2015-0010</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich bekannt gegeben.<br />
<br />
Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525535">MS15-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0057">CVE-2015-0057</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525535">MS15-010</a></td>
<td style="border:1px solid black;">„Double Free“-Sicherheitsanfälligkeit im Windows-Cursorobjekt</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0058">CVE-2015-0058</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525535">MS15-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung bei Analyse von True Type-Schriftarten</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0059">CVE-2015-0059</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525536">MS15-011</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Gruppenrichtlinie bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0008">CVE-2015-0008</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525537">MS15-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Excel bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0063">CVE-2015-0063</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525537">MS15-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0064">CVE-2015-0064</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525537">MS15-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OneTableDocumentStream bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0065">CVE-2015-0065</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525533">MS15-013</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Microsoft Office-Komponente</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6362">CVE-2014-6362</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich bekannt gegeben.<br />
<br />
Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=522532">MS15-014</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Gruppenrichtlinie bezüglich Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0009">CVE-2015-0009</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525538">MS15-015</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows-Prozesserstellung bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0062">CVE-2015-0062</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525539">MS15-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bei TIFF-Verarbeitung durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0061">CVE-2015-0061</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=525540">MS15-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Virtual Machine Manager bezüglich Rechteerweiterungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2015-0012">CVE-2015-0012</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.</td>
</tr>
</tbody>
</table>
  
 
  
Betroffene Software  
-------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.
  
**Hinweis** Für eine Sicherheitsanfälligkeit müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
### Systemkomponenten des Windows-Betriebssystems

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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3021952)  
(Mittel)  
Internet Explorer 7  
(3021952)  
(Mittel)  
Internet Explorer 8  
(3021952)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3013455)  
(Hoch)  
Windows Server 2003 Service Pack 2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3021952)  
(Mittel)  
Internet Explorer 7  
(3021952)  
(Mittel)  
Internet Explorer 8  
(3021952)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3013455)  
(Hoch)  
Windows Server 2003 x64 Edition Service Pack 2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3021952)  
(Mittel)  
Internet Explorer 7  
(3021952)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3013455)  
(Hoch)  
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3029944)  
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3021952)  
(Kritisch)  
Internet Explorer 8  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3013455)  
(Hoch)  
Windows Vista Service Pack 2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3021952)  
(Kritisch)  
Internet Explorer 8  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3013455)  
(Hoch)  
Windows Vista x64 Edition Service Pack 2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3029944)  
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3021952)  
(Mittel)  
Internet Explorer 8  
(3021952)  
(Mittel)  
Internet Explorer 9  
(3021952)  
(Mittel)  
Internet Explorer 9  
(3034196)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3013455)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3021952)  
(Mittel)  
Internet Explorer 8  
(3021952)  
(Mittel)  
Internet Explorer 9  
(3021952)  
(Mittel)  
Internet Explorer 9  
(3034196)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3013455)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3021952)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3013455)  
(Hoch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3029944)  
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
Internet Explorer 8  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3034196)  
(Hoch)  
Internet Explorer 10  
(3021952)  
(Kritisch)  
Internet Explorer 10  
(3034196)  
(Hoch)  
Internet Explorer 11  
(3021952)  
(Kritisch)  
Internet Explorer 11  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3013455)  
(Kritisch)  
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3021952)  
(Kritisch)  
Internet Explorer 9  
(3034196)  
(Hoch)  
Internet Explorer 10  
(3021952)  
(Kritisch)  
Internet Explorer 10  
(3034196)  
(Hoch)  
Internet Explorer 11  
(3021952)  
(Kritisch)  
Internet Explorer 11  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3013455)  
(Kritisch)  
Windows 7 für x64-basierte Systeme Service Pack 1  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3029944)  
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3021952)  
(Mittel)  
Internet Explorer 9  
(3021952)  
(Mittel)  
Internet Explorer 9  
(3034196)  
(Niedrig)  
Internet Explorer 10  
(3021952)  
(Mittel)  
Internet Explorer 10  
(3034196)  
(Niedrig)  
Internet Explorer 11  
(3021952)  
(Mittel)  
Internet Explorer 11  
(3034196)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3013455)  
(Kritisch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3021952)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3013455)  
(Kritisch)  
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3029944)  
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
Internet Explorer 10  
(3021952)  
(Kritisch)  
Internet Explorer 10  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3013455)  
(Kritisch)  
Windows 8 für 32-Bit-Systeme  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3021952)  
(Kritisch)  
Internet Explorer 10  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3013455)  
(Kritisch)  
Windows 8 für x64-basierte Systeme  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3021952)  
(Kritisch)  
Internet Explorer 11  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3013455)  
(Kritisch)  
Windows 8.1 für 32-Bit-Systeme  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3021952)  
(Kritisch)  
Internet Explorer 11  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3013455)  
(Kritisch)  
Windows 8.1 für x64-basierte Systeme  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3029944)  
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3021952)  
(Mittel)  
Internet Explorer 10  
(3034196)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3013455)  
(Kritisch)  
Windows Server 2012  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3021952)  
(Mittel)  
Internet Explorer 11  
(3034196)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3013455)  
(Kritisch)  
Windows Server 2012 R2  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3029944)  
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
Internet Explorer 10  
(3021952)  
(Kritisch)  
Internet Explorer 10  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3013455)  
(Kritisch)  
Windows RT  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3029944)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3021952)  
(Kritisch)  
Internet Explorer 11  
(3034196)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3013455)  
(Kritisch)  
Windows RT 8.1  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3029944)  
(Hoch)
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
[**MS15-009**](https://go.microsoft.com/fwlink/?linkid=525534)
</td>
<td style="border:1px solid black;">
[**MS15-010**](https://go.microsoft.com/fwlink/?linkid=525535)
</td>
<td style="border:1px solid black;">
[**MS15-011**](https://go.microsoft.com/fwlink/?linkid=525536)
</td>
<td style="border:1px solid black;">
[**MS15-014**](https://go.microsoft.com/fwlink/?linkid=522532)
</td>
<td style="border:1px solid black;">
[**MS15-015**](https://go.microsoft.com/fwlink/?linkid=525538)
</td>
<td style="border:1px solid black;">
[**MS15-016**](https://go.microsoft.com/fwlink/?linkid=525539)
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
(3013455)  
(Hoch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3029944)  
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
(3013455)  
(Hoch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3029944)  
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
(3013455)  
(Kritisch)  
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3029944)  
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
(3013455)  
(Kritisch)  
Windows Server 2012 (Server Core-Installation)  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3029944)  
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
(3013455)  
(Kritisch)  
Windows Server 2012 R2 (Server Core-Installation)  
(3023562)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3000483)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3004361)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3031432)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3029944)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-009 und MS15-010**

Windows Technical Preview und Windows Server Technical Preview sind betroffen. Benutzern, die diese Betriebssysteme verwenden, wird empfohlen, das Update über [Windows Update](https://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) zu installieren.

**Hinweis zu MS15-011**

<sup>[1]</sup>Windows Server 2003 ist betroffen, aber es wurde kein Update veröffentlicht. Weitere Informationen finden Sie im Bulletin.

 

### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft System Center Virtual Machine Manager 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-017**](https://go.microsoft.com/fwlink/?linkid=525540)
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
Microsoft System Center Virtual Machine Manager 2012 R2 Updaterollup 4
</td>
<td style="border:1px solid black;">
Microsoft System Center Virtual Machine Manager 2012 R2 Updaterollup 4  
(VMM-Serverupdate 2992024)<sup>[1]</sup>
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-017**

<sup>[1]</sup>Benutzer, die diese Software ausführen, sollten das Sicherheitsupdate für Microsoft System Center 2012 R2 – Virtual Machine Manager 2012 R2 UR5 (KB3023195) herunterladen und installieren, um die in MS15-017 beschriebene Sicherheitsanfälligkeit zu beheben. Weitere Informationen finden Sie im Bulletin.

 

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
[**MS15-012**](https://go.microsoft.com/fwlink/?linkid=525537)
</td>
<td style="border:1px solid black;">
[**MS15-013**](https://go.microsoft.com/fwlink/?linkid=525533)
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
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Excel 2007 Service Pack 3  
(2920788)  
(Hoch)  
Microsoft Word 2007 Service Pack 3  
(2956099)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(2920795)  
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
[**MS15-012**](https://go.microsoft.com/fwlink/?linkid=525537)
</td>
<td style="border:1px solid black;">
[**MS15-013**](https://go.microsoft.com/fwlink/?linkid=525533)
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
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen) (Korrekturhilfen)  
(2956073)  
(Hoch)  
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2956058)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(2956081)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(2956066)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2920748)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen) (Korrekturhilfen)  
(2956073)  
(Hoch)  
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2956058)  
(Hoch)  
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(2956081)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(2956066)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2920748)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2013 und Microsoft Office 2013 RT**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS15-012**](https://go.microsoft.com/fwlink/?linkid=525537)
</td>
<td style="border:1px solid black;">
[**MS15-013**](https://go.microsoft.com/fwlink/?linkid=525533)
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
Microsoft Office 2013 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 (32-Bit-Editionen)  
(2920753)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 (32-Bit-Editionen)  
(2910941)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 Service Pack 1 (32-Bit-Editionen)  
(2920753)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (32-Bit-Editionen)  
(2910941)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 (64-Bit-Editionen)  
(2920753)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 (64-Bit-Editionen)  
(2910941)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 Service Pack 1 (64-Bit-Editionen)  
(2920753)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2013 Service Pack 1 (64-Bit-Editionen)  
(2910941)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 RT
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 RT  
(2920753)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 RT Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 RT Service Pack 1  
(2920753)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
[**MS15-012**](https://go.microsoft.com/fwlink/?linkid=525537)
</td>
<td style="border:1px solid black;">
[**MS15-013**](https://go.microsoft.com/fwlink/?linkid=525533)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(2956092)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
Microsoft Excel Viewer  
(2920791)<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2956097)  
(Hoch)  
Microsoft Office Compatibility Pack Service Pack 3  
(2956098)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise zu MS15-012**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

<sup>[1]</sup>Update 2920791 behebt auch die im Bulletin [MS14-083](https://technet.microsoft.com/de-de/library/security/ms14-083) beschriebene Sicherheitsanfälligkeit. Das Bulletin wird derzeit neu veröffentlicht.

 

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
[**MS15-012**](https://go.microsoft.com/fwlink/?linkid=525537)
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
(2920810)  
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
[**MS15-012**](https://go.microsoft.com/fwlink/?linkid=525537)
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
Microsoft Web Applications 2010 Service Pack 2  
(2956070)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis zu MS15-012**

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

Weitere Informationen:
----------------------

### Microsoft Windows-Tool zum Entfernen bösartiger Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
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

-   V1.0 (10. Februar 2015): Bulletin Summary veröffentlicht.

*Seite generiert am 06.02.2015 um 12:47Z-08:00.*
