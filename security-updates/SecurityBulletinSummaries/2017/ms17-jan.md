---
TOCTitle: 'MS17-JAN'
Title: Microsoft Security Bulletin Summary für Januar 2017
ms:assetid: 'ms17-jan'
ms:contentKeyID: 74294004
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms17-jan(v=Security.10)'
---

Microsoft Security Bulletin Summary für Januar 2017
===================================================

Veröffentlicht: 10. Januar 2017

**Version:** 1.1

In diesem Bulletin Summary sind die im Januar 2017 veröffentlichten Security Bulletins aufgeführt.

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft-Sicherheitsbulletins finden Sie unter [Technische Sicherheitsbenachrichtigungen von Microsoft](https://go.microsoft.com/fwlink/?linkid=21163).

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

**Hinweis:** Für die Veröffentlichung des Updates am Dienstag für Januar 2017 gibt es keine Sicherheitsfixes oder Qualitätsverbesserungen. Demzufolge gibt es für diesen Monat kein reines Sicherheitsqualitätsupdate bzw. keinen monatlichen Sicherheitsqualitätsrollup.

Zur Erinnerung: Der [Leitfaden für Sicherheitsupdates](https://portal.msrc.microsoft.com/de-de/security-guidance) wird ab Februar 2017 Sicherheitsbulletins ersetzen. Details finden Sie in unserem Blog-Eintrag [Furthering our commitment to security updates](https://blogs.technet.microsoft.com/msrc/2016/11/08/furthering-our-commitment-to-security-updates/).

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=838331">MS17-001</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Microsoft Edge (3214288)</strong><br />
Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Edge. Diese Sicherheitsanfälligkeit kann Rechteerweiterungen ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Microsoft Edge anzeigt. Ein Angreifer, der diese Anfälligkeit erfolgreich ausnutzt, könnte erweiterte Rechte auf dem Namespace-Verzeichnis eines anfälligen Systems und erweiterte Rechte erhalten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a><br />
Rechteerweiterungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Edge</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=838332">MS17-002</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Microsoft Office (3214291)<br />
</strong>Dieses Sicherheitsupdate behebt eine Sicherheitsanfälligkeit in Microsoft Office. Diese Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Microsoft Office-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit Administratorrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Office-Dienste und Web Apps</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=838351">MS17-003</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Adobe Flash Player (3214628)<br />
</strong>Dieses Sicherheitsupdate behebt Sicherheitsanfälligkeiten in Adobe Flash Player unter allen unterstützten Editionen von Windows 8.1, Windows Server 2012, Windows Server 2012 R2, Windows RT 8.1, Windows 10 und Windows 2016.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Adobe Flash Player</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=838352">MS17-004</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für den Subsystemdienst für die lokale Sicherheitsautorität (3216771)<br />
</strong>Es gibt eine Sicherheitsanfälligkeit bezüglich Denial-of-Service bei der Art und Weise, wie der Subsystemdienst für die lokale Sicherheitsautorität (Local Security Authority Subsystem Service, LSASS) Authentifizierungsanforderungen verarbeitet. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann einen Denial-of-Service-Fehler für den LSASS-Dienst des Zielsystems verursachen, wodurch ein automatischer Neustart des Systems ausgelöst wird. Das Sicherheitsupdate behebt diese Sicherheitsanfälligkeit, indem geändert wird, wie LSASS speziell gestaltete Authentifizierungsanforderungen verarbeitet.</td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140">Hoch</a> <br />
Denial-of-Service</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">---------</td>
<td style="border:1px solid black;">Microsoft Windows</td>
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
[**MS17-001: Kumulatives Sicherheitsupdate für Microsoft Edge (3214288)**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0002](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0002)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Edge bezüglich Rechteerweiterungen
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
[**MS17-002: Sicherheitsupdate für Microsoft Office (3214291)**](https://go.microsoft.com/fwlink/?linkid=838332)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0003](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0003)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in GDI bezüglich der Offenlegung von Informationen
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
[**MS17-003: Sicherheitsupdate für Adobe Flash Player (3214628)**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[APSB17-02](https://helpx.adobe.com/de/security/products/flash-player/apsb17-02.html)
</td>
<td style="border:1px solid black;">
Die Bewertungen des Schweregrads und der Updatepriorität finden Sie unter [APSB17-02](https://helpx.adobe.com/de/security/products/flash-player/apsb17-02.html).
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
<tr>
<td style="border:1px solid black;" colspan="5">
[**MS17-004: Sicherheitsupdate für den Subsystemdienst für die lokale Sicherheitsautorität (3216771)**](https://go.microsoft.com/fwlink/?linkid=838352)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[CVE-2017-0004](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0004)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Subsystemdienst für die lokale Sicherheitsautorität bezüglich Denial-of-Service
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
</table>
 

Betroffene Software
-------------------

In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.

In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.

**Hinweis** Für ein Sicherheitsrisiko müssen möglicherweise mehrere Sicherheitsupdates installiert werden. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.

### Windows-Betriebssysteme und -Komponenten

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista für Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista für Service Pack 2  
(3216775)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3216775)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3216775)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3216775)  
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
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3216775)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x32-Bit-Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x32-Bit-Systeme Service Pack 1  
(3212642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3212646)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x32-Bit-Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x32-Bit-Systeme Service Pack 1  
(3212642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3212646)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack  
(3212642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3212646)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3212642)  
(Hoch)
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
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3212646)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
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
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
[**Mittel**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
Nur Sicherheit
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
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
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows 10**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3210720)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3210720)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3210721)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1511 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3210721)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3211320)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 10 Version 1607 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Microsoft Edge  
(3211320)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Adobe Flash Player  
(3214628)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Windows Server 2016**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
[**Kritisch**](https://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="4">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS17-001**](https://go.microsoft.com/fwlink/?linkid=838331)
</td>
<td style="border:1px solid black;">
[**MS17-003**](https://go.microsoft.com/fwlink/?linkid=838351)
</td>
<td style="border:1px solid black;">
[**MS17-004**](https://go.microsoft.com/fwlink/?linkid=838352)
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3216775)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
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
(3216775)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack (Server Core-Installation)  
(3212642)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1(Server Core-Installation)  
Monatlicher Rollup
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3212646)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012  
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
Windows Server 2012 R2  
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
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2  
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
Nicht anwendbar
</td>
</tr>
</table>
 
### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
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
[**MS17-002**](https://go.microsoft.com/fwlink/?linkid=838332)
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
Microsoft Office 2016 (32-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Word 2016 (32-Bit-Edition)  
(3128057)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2016 (64-Bit-Edition)
</td>
<td style="border:1px solid black;">
Microsoft Word 2016 (64-Bit-Edition)  
(3128057)  
(Hoch)
</td>
</tr>
</table>
 
### Microsoft Office-Dienste und Web Apps

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Microsoft Office-Dienste und Web Apps</strong></td>
<td style="border:1px solid black;"><strong>Microsoft Office-Dienste und Web Apps</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=838332"><strong>MS17-002</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bewertung des Gesamtschweregrads</strong></td>
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=21140"><strong>Hoch</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SharePoint Enterprise Server 2016 (64-Bit-Edition)</td>
<td style="border:1px solid black;">Microsoft SharePoint Foundation 2016 (64-Bit-Edition)<br />
(3141486)<br />
(Kritisch)</td>
</tr>
</tbody>
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

Microsoft erkennt die Bemühungen der Mitglieder der Sicherheitscommunity an, die uns durch die verantwortungsvolle Offenlegung von Sicherheitsanfälligkeiten helfen, unsere Kunden zu schützen. Weitere Informationen finden Sie unter [Danksagung](https://technet.microsoft.com/de-de/library/security/mt745121.aspx).

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

-   V1.0 (10. Januar 2017): Bulletin Summary veröffentlicht.
-   V1.1 (10. Januar 2017): Schweregrad auf “Hoch” heruntergestuft.

*Seite generiert am 06.01.2017 um 14:39-08:00.*