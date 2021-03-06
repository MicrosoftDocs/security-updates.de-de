---
TOCTitle: 'MS11-JUL'
Title: Microsoft Security Bulletin Summary für Juli 2011
ms:assetid: 'ms11-jul'
ms:contentKeyID: 61225096
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms11-jul(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Juli 2011
=================================================

Veröffentlicht: Dienstag, 12. Juli 2011

**Version:** 1.0

In diesem Bulletin Summary sind die im Juli 2011 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Juli 2011 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 7. Juli 2011 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 13. Juli 2011 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im Juli.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032487855&eventcategory=4) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://go.microsoft.com/fwlink/?linkid=217214)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Security Bulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im nächsten Abschnitt **Betroffene Software und Downloadadressen**.

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel des Bulletins und Kurzzusammenfassung</th>
<th style="border:1px solid black;" >Bewertung des maximalen Schweregrads und Sicherheitsauswirkung</th>
<th style="border:1px solid black;" >Neustartanforderung</th>
<th style="border:1px solid black;" >Betroffene Software</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217102">MS11-053</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Bluetooth-Stack kann Remotecodeausführung ermöglichen (2566220)</strong> <br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Windows Bluetooth-Stack. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine Reihe speziell gestalteter Bluetooth-Pakete an ein betroffenes System sendet. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Diese Sicherheitsanfälligkeit betrifft nur Bluetooth-fähige Systeme</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=220172">MS11-054</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Erhöhung von Berechtigungen ermöglichen (2555917)</strong> <br />
<br />
Dieses Sicherheitsupdate behebt fünfzehn vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217465">MS11-056</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows Client/Server-Runtime-Subsystem können Erhöhung von Berechtigungen ermöglichen (2507938) </strong><br />
<br />
Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete Sicherheitsanfälligkeiten im Microsoft Windows Client/Server-Runtime-Subsystem (CSRSS). Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei dem System eines Benutzers anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=220276">MS11-055</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Visio können Remotecodeausführung ermöglichen (2560847) </strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Visio. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine gültige Datei in Visio öffnet, die sich in demselben Netzwerkverzeichnis befindet wie eine speziell gestaltete Bibliotheksdatei. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der angemeldete Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.
  
| Kennung des Bulletins                                     | Titel der Sicherheitsanfälligkeit                                                                           | CVE-ID                                                                           | Bewertung der Ausnutzbarkeit durch Codeausführung für aktuelle Softwareversion                              | Bewertung der Ausnutzbarkeit durch Codeausführung für ältere Softwareversionen                              | Bewertung der Ausnutzbarkeit durch Denial-of-Service | Wichtige Hinweise                                                                                                                            |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS11-053](https://go.microsoft.com/fwlink/?linkid=217102) | Sicherheitsanfälligkeit im Bluetooth-Stack                                                                  | [CVE-2011-1265](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1265) | [2](https://technet.microsoft.com/en-us/security/cc998259.aspx)- Inkonsistenter Angreifercode wahrscheinlich | [2](https://technet.microsoft.com/de-de/security/cc998259) – Inkonsistenter Angreifercode wahrscheinlich     | Dauerhaft                                            | Diese Sicherheitsanfälligkeit betrifft nur Bluetooth-fähige Clientsysteme (unterstützte Veröffentlichungen von Windows Vista und Windows 7). |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1874](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1874) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1875](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1875) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1876](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1876) | [2](https://technet.microsoft.com/de-de/security/cc998259) – Inkonsistenter Angreifercode wahrscheinlich     | [2](https://technet.microsoft.com/de-de/security/cc998259) – Inkonsistenter Angreifercode wahrscheinlich     | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1877](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1877) | [2](https://technet.microsoft.com/de-de/security/cc998259) – Inkonsistenter Angreifercode wahrscheinlich     | [2](https://technet.microsoft.com/de-de/security/cc998259) – Inkonsistenter Angreifercode wahrscheinlich     | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1878](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1878) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1879](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1879) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung                                     | [CVE-2011-1880](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1880) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung                                     | [CVE-2011-1881](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1881) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1882](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1882) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1883](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1883) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                              | [CVE-2011-1884](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1884) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung                                     | [CVE-2011-1885](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1885) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Sicherheitsanfälligkeit in Win32k bezüglich Offenlegung von Informationen durch falschen Parameter          | [CVE-2011-1886](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1886) | [3](https://technet.microsoft.com/de-de/security/cc998259) – Funktionierender Angreifercode unwahrscheinlich | [3](https://technet.microsoft.com/de-de/security/cc998259) – Funktionierender Angreifercode unwahrscheinlich | Dauerhaft                                            | Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht                                                |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung                                     | [CVE-2011-1887](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1887) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-054](https://go.microsoft.com/fwlink/?linkid=220172) | Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung                                     | [CVE-2011-1888](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1888) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-055](https://go.microsoft.com/fwlink/?linkid=220276) | Sicherheitsanfälligkeit in Microsoft Visio durch nicht sicheres Laden von Bibliotheken                      | [CVE-2010-3148](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3148) | Nicht betroffen                                                                                             | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Nicht anwendbar                                      | Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.                                                                                     |  
| [MS11-056](https://go.microsoft.com/fwlink/?linkid=217465) | Sicherheitsanfälligkeit in CSRSS AllocConsole bezüglich lokaler Erhöhung von Berechtigungen                 | [CVE-2011-1281](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1281) | [3](https://technet.microsoft.com/de-de/security/cc998259) – Funktionierender Angreifercode unwahrscheinlich | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Nicht anwendbar                                      | (Keine)                                                                                                                                      |  
| [MS11-056](https://go.microsoft.com/fwlink/?linkid=217465) | Sicherheitsanfälligkeit in CSRSS SrvSetConsoleLocalEUDC bezüglich lokaler Erhöhung von Berechtigungen       | [CVE-2011-1282](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1282) | [3](https://technet.microsoft.com/de-de/security/cc998259) – Funktionierender Angreifercode unwahrscheinlich | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-056](https://go.microsoft.com/fwlink/?linkid=217465) | Sicherheitsanfälligkeit in CSRSS SrvSetConsoleNumberOfCommand bezüglich lokaler Erhöhung von Berechtigungen | [CVE-2011-1283](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1283) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-056](https://go.microsoft.com/fwlink/?linkid=217465) | Sicherheitsanfälligkeit in CSRSS SrvWriteConsoleOutput bezüglich lokaler Erhöhung von Berechtigungen        | [CVE-2011-1284](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1284) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |  
| [MS11-056](https://go.microsoft.com/fwlink/?linkid=217465) | Sicherheitsanfälligkeit in CSRSS SrvWriteConsoleOutputString bezüglich lokaler Erhöhung von Berechtigungen  | [CVE-2011-1870](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1870) | [3](https://technet.microsoft.com/de-de/security/cc998259) – Funktionierender Angreifercode unwahrscheinlich | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich       | Dauerhaft                                            | (Keine)                                                                                                                                      |
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
**Hinweis**: Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
#### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-053**](https://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](https://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](https://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=d7a47370-f415-46ea-9a82-a943f743c8b6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=425c705e-94f2-4fa6-9df2-dc71897215fa)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=db89d88f-d0d4-4ed6-8589-bf27557c0304)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c389fa20-677e-49b6-af44-781e5522d08b)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-053**](https://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](https://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](https://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7a26a437-a705-4d48-8389-50f159a39891)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=dff4c67a-8c8b-4d7d-84c7-57429becf0ff)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=95393f89-0b05-4243-95ed-17bcdad24bfb)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=1615a995-9a04-440a-ae52-5917738f0ecb)  
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
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=3b094bdb-4150-44f2-a638-afd5f41b00a3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=a81c011d-eeea-4383-9efb-df70515ab357)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-053**](https://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](https://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](https://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=6bff74ac-45f3-4585-92da-316921b458fa)<sup>[1]</sup>
(KB2561109)  
(Kritisch)  
[Windows Vista Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=a1e5aa7d-5f38-4ce2-9575-4b4cb7520160)  
(KB2532531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=c1fe1e53-34d5-497e-8ba2-50caa8dc1158)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=a5e192af-dae5-47ef-a9d0-f761a8caa974)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=849d2694-c8b3-4670-8203-912661bccabf)<sup>[1]</sup>
(KB2561109)  
(Kritisch)  
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=4287eeb4-ab29-4727-83f2-260d838b44d4)  
(KB2532531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7bc0a285-cc32-4c6b-abee-d92130d459b7)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=1007f5d3-9be1-4f03-a3f0-12ddb555653c)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-053**](https://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](https://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](https://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=b88d0471-4427-4835-9446-db71116481f0)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=36e3dbaf-36f5-4c74-8f11-ecbef46f58e1)\*  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=d3df6184-3e3c-4949-a1ee-293ec68f8149)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=b43d2ab5-e281-4c6b-bb37-1f1b5d86ac82)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=9e021d69-7f0c-457f-af86-07e760d8f421)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=b70209f2-1c51-45af-b3c4-3473aebcdb35)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-053**](https://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](https://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](https://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7f811b75-c3ff-411a-aaa9-126dce34cc01)  
(KB2532531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=41db1b2f-f862-43bb-89bc-4b97737e5cb9)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=ac3b435c-8caf-40cc-8f13-b52261b3b9e6)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=90b2da71-18f9-46ee-9e3d-b08620ca06aa)  
(KB2532531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=211abdc6-40c7-4bfc-8c2d-be72981f311e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=64e5f889-fa46-4884-9b22-3ba4e2fba1b9)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-053**](https://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](https://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](https://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=4f54e498-3825-407d-a036-1900a65d34f1)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=b99a40cf-8a31-43d9-bd0b-a458a533068b)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=e7ae39e8-1154-4a13-8598-29d4a6358762)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=784efc20-3a41-42ab-b48d-51fd59d71523)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS11-053**

<sup>[1]</sup>Windows Vista Service Pack 1 ist nur betroffen, wenn das optionale Windows Vista Feature Pack für Wireless installiert wurde.

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office Suites und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-055**](https://go.microsoft.com/fwlink/?linkid=220276)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2003 Service Pack 3](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=1c7b2a5b-4aa6-4006-90bf-89f8b2b7becd)  
(KB2493523)  
(Hoch)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://technet.microsoft.com/de-de/windowsserver/bb332157).

**System Center Configuration Manager 2007**

Configuration Manager 2007-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit Configuration Manager 2007 können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in Configuration Manager 2007 erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in Configuration Manager 2007 ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen dazu, wie Administratoren mithilfe von Configuration Manager 2007 Updates bereitstellen können, finden Sie in [Softwareupdateverwaltung](https://www.microsoft.com/germany/systemcenter/sccm/evaluation/updatemgmt.mspx). Weitere Informationen zu Configuration Manager finden Sie auf der Website [System Center Configuration Manager](https://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](https://support.microsoft.com/common/international.aspx?rdpath=dm;de-de;lifecycle). Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager 2007**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](https://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24da89e9-b581-47b0-b45e-492dd6da2971&amp;displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Tarjei Mandt von [Norman](https://www.norman.com) für den Hinweis auf 14 in MS11-054 beschriebene Probleme.
-   Herr Liang Yin, Prof. Sihan Qing und Weiping Wen und Herr Husheng Zhou, [Department of Information Security, Beijing University](https://www.ss.pku.edu.cn/en/), für den Hinweis auf ein in MS11-054 beschriebenes Problem.
-   Matthew ‘j00 ru‘ Jurczyk von [Hispasec](https://www.hispasec.com/) [Virustotal](https://www.virustotal.com/) für den Hinweis auf fünf in MS11-056 beschriebene Probleme.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (12. Juli 2011): Bulletin Summary veröffentlicht.

*Built at 2014-04-18T01:50:00Z-07:00*