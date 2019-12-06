---
TOCTitle: 'MS12-NOV'
Title: Microsoft Security Bulletin Summary für November 2012
ms:assetid: 'ms12-nov'
ms:contentKeyID: 61225112
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms12-nov(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für November 2012
=====================================================

Veröffentlicht: Dienstag, 13. November 2012 | Aktualisiert: Mittwoch, 14. November 2012

**Version:** 2.0

In diesem Bulletin Summary sind die im November 2012 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für November 2012 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 8. November 2012 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, den 14. November 2012 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im November.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032522560&culture=en-us) Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032522560&culture=en-us) zur Verfügung.

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

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
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/bulletin/ms12-071">MS12-071</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2761451)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, können diese Sicherheitsanfälligkeiten Remotecodeausführung ermöglichen. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=260820">MS12-072</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows Shell können Remotecodeausführung ermöglichen (2727528)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer in Windows Explorer zu einem speziell gestalteten Aktenkoffer durchsucht. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann als aktueller Benutzer beliebigen Code ausführen. Wenn der aktuelle Benutzer mit administrativen Benutzerberechtigungen angemeldet ist, kann ein Angreifer vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=255026">MS12-074</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in .NET Framework können Remotecodeausführung ermöglichen (2745030)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete Sicherheitsanfälligkeiten in .NET Framework. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Angreifer den Benutzer eines Zielsystems dazu verleitet, eine schädliche Proxy-Autokonfigurationsdatei zu verwenden, und dann Code in die derzeit ausgeführte Anwendung einschleust.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=270856">MS12-075</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Remotecodeausführung ermöglichen (2761226)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer ein speziell gestaltetes Dokument öffnet oder eine schädliche Webseite besucht, in der TrueType-Schriftartdateien eingebettet sind. Der Angreifer muss den Benutzer zum Besuch dieser Website verleiten, z. B. indem er den Benutzer dazu auffordert, in einer E-Mail-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=260964">MS12-076</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (2720184)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Excel-Datei mit einer betroffenen Version von Microsoft Excel öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=258247">MS12-073</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in den Microsoft Internetinformationsdiensten (IIS) können Offenlegung von Information ermöglichen (2733829)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Internet Information Services (IIS). Die schwerwiegendere Sicherheitsanfälligkeit kann Offenlegung von Information ermöglichen, wenn ein Angreifer speziell gestaltete FTP-Befehle an den Server sendet.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Mittel</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.
  
| Kennung des Bulletins                                                     | Titel der Sicherheitsanfälligkeit                                                                | CVE-ID                                                                           | Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen                                             | Bewertung der Ausnutzbarkeit für ältere Softwareversionen                                               | Bewertung der Ausnutzbarkeit durch Denial-of-Service | Wichtige Hinweise                                                                              |  
|---------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|------------------------------------------------------|------------------------------------------------------------------------------------------------|  
| [MS12-071](http://technet.microsoft.com/de-de/security/bulletin/ms12-071) | Use-after-free-Sicherheitsanfälligkeit in CFormElement                                           | [CVE-2012-1538](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1538) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-071](http://technet.microsoft.com/de-de/security/bulletin/ms12-071) | Use-after-free-Sicherheitsanfälligkeit in CTreePos                                               | [CVE-2012-1539](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1539) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Vorläufig                                            | (Keine)                                                                                        |  
| [MS12-071](http://technet.microsoft.com/de-de/security/bulletin/ms12-071) | Use-after-free-Sicherheitsanfälligkeit in CTreeNode                                              | [CVE-2012-4775](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-4775) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-072](http://go.microsoft.com/fwlink/?linkid=260820)                 | Sicherheitsanfälligkeit durch Ganzzahlunterlauf in Windows Aktenkoffer                           | [CVE-2012-1527](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1527) | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-072](http://go.microsoft.com/fwlink/?linkid=260820)                 | Sicherheitsanfälligkeit durch Ganzzahlüberlauf in Windows Aktenkoffer                            | [CVE-2012-1528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1528) | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Vorläufig                                            | (Keine)                                                                                        |  
| [MS12-074](http://go.microsoft.com/fwlink/?linkid=255026)                 | Sicherheitsanfälligkeit durch Umgehung der Reflektion                                            | [CVE-2012-1895](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1895) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-074](http://go.microsoft.com/fwlink/?linkid=255026)                 | Sicherheitsanfälligkeit durch Offenlegung von Informationen bezüglich der Codezugriffssicherheit | [CVE-2012-1896](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1896) | Nicht betroffen                                                                                         | [3](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode unwahrscheinlich         | Nicht anwendbar                                      | Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht. |  
| [MS12-074](http://go.microsoft.com/fwlink/?linkid=255026)                 | Sicherheitsanfälligkeit in .NET Framework durch nicht sicheres Laden von Bibliotheken            | [CVE-2012-2519](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2519) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-074](http://go.microsoft.com/fwlink/?linkid=255026)                 | Sicherheitsanfälligkeit in Web Proxy Auto-Discovery                                              | [CVE-2012-4776](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-4776) | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Dauerhaft                                            | (Keine)                                                                                        |  
| [MS12-074](http://go.microsoft.com/fwlink/?linkid=255026)                 | Sicherheitsanfälligkeit durch Optimierung der WPF-Reflektion                                     | [CVE-2012-4777](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-4777) | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-075](http://go.microsoft.com/fwlink/?linkid=270856)                 | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                   | [CVE-2012-2530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2530) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Dauerhaft                                            | (Keine)                                                                                        |  
| [MS12-075](http://go.microsoft.com/fwlink/?linkid=270856)                 | Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung                                   | [CVE-2012-2553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2553) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Dauerhaft                                            | (Keine)                                                                                        |  
| [MS12-075](http://go.microsoft.com/fwlink/?linkid=270856)                 | Sicherheitsanfälligkeit bei der Analyse von TrueType-Schriftarten                                | [CVE-2012-2897](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2897) | [2](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wäre schwer zu erstellen | [2](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wäre schwer zu erstellen | Dauerhaft                                            | (Keine)                                                                                        |  
| [MS12-076](http://go.microsoft.com/fwlink/?linkid=260964)                 | Sicherheitsanfälligkeit in Excel SerAuxErrBar durch Heapüberlauf                                 | [CVE-2012-1885](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1885) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-076](http://go.microsoft.com/fwlink/?linkid=260964)                 | Sicherheitsanfälligkeit in Excel bezüglich Speicherbeschädigung                                  | [CVE-2012-1886](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1886) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-076](http://go.microsoft.com/fwlink/?linkid=260964)                 | Use-after-free-Sicherheitsanfälligkeit in durch ungültige Länge in Excel SST                     | [CVE-2012-1887](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1887) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS12-076](http://go.microsoft.com/fwlink/?linkid=260964)                 | Sicherheitsanfälligkeit in Excel durch Stapelüberlauf                                            | [CVE-2012-2543](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2543) | Nicht betroffen                                                                                         | [1](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
#### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="6" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
</td>
</tr>
<tr class="alternateRow">
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=fcc633d6-fe18-4220-9b68-ff1479e4dec5)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f5472e86-2b2f-42bd-abca-6adf84973efa)  
(KB2698035)  
(nur Media Center Edition 2005 Service Pack 3 und Tablet PC Edition 2005 Service Pack 3)  
(Hoch)  
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7e75292-efcf-4c97-960c-958f81931cbf)  
(KB2729450)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=31f2c645-b171-4f11-884b-f5056ef57b4f)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a736c3f0-0326-4a0a-9c12-f61bafa537bb)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7e75292-efcf-4c97-960c-958f81931cbf)  
(KB2729450)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=828699ac-eb88-4ff8-9110-69c206f5ef54)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
</td>
</tr>
<tr class="alternateRow">
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
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
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0383bdea-53d1-4799-b380-14da1595882a)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=efe0de22-8ca3-474e-acda-7203bf66d0a3)  
(KB2698032)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7e75292-efcf-4c97-960c-958f81931cbf)  
(KB2729450)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=73f5dec6-ccda-426d-8d2c-a2db3e59734a)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=615a96fe-88a5-498b-ae20-bbfc43e3b652)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7e75292-efcf-4c97-960c-958f81931cbf)  
(KB2729450)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dc9cd62a-c42d-4c54-bc14-7abd34aeb865)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=36962e96-0eaa-45a9-b2d6-6bec3242c73e)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7e75292-efcf-4c97-960c-958f81931cbf)  
(KB2729450)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=e4ec19ea-06f2-4164-8e39-84f1d7a47ae7)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=205f1cf3-5431-4740-96c2-eaf019edeeeb)  
(KB2761451)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c19585e3-a358-40b0-80a3-8dbb25ba8557)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d742523-5f51-4db7-b05f-a9055b36b090)  
(KB2729453)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c4b3fb44-338d-48be-9981-53fa2cf3094a)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=e1785af2-a211-467e-a696-d53840581bca)<sup>[1]</sup>
(KB2716513)  
(Mittel)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=b91091d0-176f-4ff9-98d2-74768b747c3a)<sup>[1]</sup>
(KB2716513)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=7e7b681c-c580-4671-a515-e5b469002c93)  
(KB2761451)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=31f5ad28-ffe9-4370-b3fc-62eb9fc0c4dd)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d742523-5f51-4db7-b05f-a9055b36b090)  
(KB2729453)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7a58e874-f3fc-4db8-8de0-cbfc6ebbf349)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=2db93767-f364-49c6-9a03-39604173771f)<sup>[1]</sup>
(KB2716513)  
(Mittel)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=0c499445-595f-459f-86cf-b821cbb5fa65)<sup>[1]</sup>
(KB2716513)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=0161baaa-5d7b-4442-a202-41c64a73c9a8)  
(KB2761451)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=258048b5-d992-4821-8836-72262a7b5bb7)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d742523-5f51-4db7-b05f-a9055b36b090)  
(KB2729453)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17b987db-0551-45c3-aab1-0cc11ae60dcc)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=cb3598ae-b647-4aaa-90fb-b4d8aa1cf211)<sup>[1]</sup>
(KB2716513)  
(Mittel)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=8b135d6f-0f6c-4bd5-bf64-d79ae16ac6a5)<sup>[1]</sup>
(KB2716513)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=52f652bd-edc4-4450-91b4-f19401d2201c)  
(KB2761451)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1c067cb2-71a5-4f8d-9b11-243c9e5318ce)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d742523-5f51-4db7-b05f-a9055b36b090)  
(KB2729453)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dd9bd994-41e3-46a1-9dfb-c6d89a3ef883)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=74d130a4-f42a-48af-87fc-349a1e107529)<sup>[1]</sup>
(KB2716513)  
(Mittel)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=b061a0b0-66e2-49a2-8d20-0c5a6948aecf)<sup>[1]</sup>
(KB2716513)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17a110d1-ef31-4230-9f2a-0df190c28747)  
(KB2698023)  
(Hoch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d742523-5f51-4db7-b05f-a9055b36b090)  
(KB2729453)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fab87b20-398f-4043-9cbe-ffcae8e19ff0)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
</td>
</tr>
<tr class="alternateRow">
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=279ac887-2420-48d7-bb85-c7cab49f7ff8)  
(KB2761451)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=22ab8987-2506-433f-9f12-0ab60d569949)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bbdf1e16-67d9-413c-bad2-31d164fea0da)  
(KB2729451)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=c222943e-9888-4fb9-b9a2-7a035311c887)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=77a4ae4e-a75c-490a-a0b1-137816ed5c89)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=fb265aa5-0e09-411a-a0fe-bbb42c409a81)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=279ac887-2420-48d7-bb85-c7cab49f7ff8)  
(KB2761451)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=22ab8987-2506-433f-9f12-0ab60d569949)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=aa5b1e9c-3068-40e3-b04f-6a71f1a51d45)  
(KB2729452)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c222943e-9888-4fb9-b9a2-7a035311c887)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=77a4ae4e-a75c-490a-a0b1-137816ed5c89)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=fb265aa5-0e09-411a-a0fe-bbb42c409a81)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=eb9babdc-3fac-4ce9-a7ca-85e26a9cb11d)  
(KB2761451)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=fc70708e-9de9-4618-b0ab-d9aa3e2baea0)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bbdf1e16-67d9-413c-bad2-31d164fea0da)  
(KB2729451)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=50d7c25f-a67f-4946-b6db-70d9bd4dc178)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=bda21ea5-f160-4361-8ede-40f6a53a30da)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=52b6ed39-b7c1-4d49-a6a7-e6208fab24fa)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=eb9babdc-3fac-4ce9-a7ca-85e26a9cb11d)  
(KB2761451)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=fc70708e-9de9-4618-b0ab-d9aa3e2baea0)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=aa5b1e9c-3068-40e3-b04f-6a71f1a51d45)  
(KB2729452)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=50d7c25f-a67f-4946-b6db-70d9bd4dc178)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=bda21ea5-f160-4361-8ede-40f6a53a30da)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=52b6ed39-b7c1-4d49-a6a7-e6208fab24fa)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
</td>
</tr>
<tr class="alternateRow">
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=3d0a4455-b788-4ad7-be0c-5824f6103694)  
(KB2761451)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=800cd622-d271-41a4-bd21-a76177d2b272)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bbdf1e16-67d9-413c-bad2-31d164fea0da)  
(KB2729451)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=114b596c-36e1-45f5-99e2-f5fdd96b1a30)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=87f3aa7a-ee84-4e7e-972c-e83a2a06a0ef)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=e1502884-1149-47b8-93af-7f82c5d83819)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=3d0a4455-b788-4ad7-be0c-5824f6103694)  
(KB2761451)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=800cd622-d271-41a4-bd21-a76177d2b272)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=aa5b1e9c-3068-40e3-b04f-6a71f1a51d45)  
(KB2729452)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=114b596c-36e1-45f5-99e2-f5fdd96b1a30)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=87f3aa7a-ee84-4e7e-972c-e83a2a06a0ef)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=e1502884-1149-47b8-93af-7f82c5d83819)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bbdf1e16-67d9-413c-bad2-31d164fea0da)  
(KB2729451)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=70447115-957d-48a4-bc27-395abaf22149)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=92cd0488-03c2-400d-a506-eb2eb8fce7c7)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=1eea7e7f-83bf-40fc-a978-a4d08af8162a)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=aa5b1e9c-3068-40e3-b04f-6a71f1a51d45)  
(KB2729452)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=70447115-957d-48a4-bc27-395abaf22149)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=92cd0488-03c2-400d-a506-eb2eb8fce7c7)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=1eea7e7f-83bf-40fc-a978-a4d08af8162a)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows 8
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
</td>
</tr>
<tr class="alternateRow">
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=d7c93ade-f7e3-4b6f-b93d-894ca313282f)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=89faa423-42fa-48ff-be71-8fd58fa523a8)  
(KB2729462)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=c9778a0f-264e-476b-8e40-742e0ab56200)  
(KB2737084)  
(Hoch)  
[Microsoft .NET Framework](https://www.microsoft.com/download/details.aspx?familyid=b120a7a2-0eff-41d6-981e-60e5ecd55869)4.5<sup>[2]</sup>
(KB2756872)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=24ce3f78-fb25-4f51-8bb0-8cebf19d8843)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=7c4a17b7-bb7f-456c-9cb3-3a355e192734)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=89faa423-42fa-48ff-be71-8fd58fa523a8)  
(KB2729462)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=c9778a0f-264e-476b-8e40-742e0ab56200)  
(KB2737084)  
(Hoch)  
[Microsoft .NET Framework](https://www.microsoft.com/download/details.aspx?familyid=c7a417e6-72e5-4087-bb89-fb8e7f57894c)4.5<sup>[2]</sup>
(KB2756872)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=72c49d94-757c-4da4-a895-96d0830bc667)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2012
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
</td>
</tr>
<tr class="alternateRow">
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
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
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=ad6189ae-9341-409b-a53e-486fef094fd0)  
(KB2727528)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=89faa423-42fa-48ff-be71-8fd58fa523a8)  
(KB2729462)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=c9778a0f-264e-476b-8e40-742e0ab56200)  
(KB2737084)  
(Hoch)  
[Microsoft .NET Framework](https://www.microsoft.com/download/details.aspx?familyid=0a7da3d1-a0ac-42a2-9929-b6d831deb9e3)4.5<sup>[2]</sup>
(KB2756872)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=2e69d496-25b4-4f24-97e0-47cb59c178aa)  
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows RT
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)****
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)****
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr class="alternateRow">
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
Microsoft .NET Framework 4.5<sup>[3]</sup>
(KB2737084)  
(Hoch)  
Microsoft .NET Framework 4.5<sup>[2]</sup><sup>[3]</sup>
(KB2756872)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Windows RT<sup>[1]</sup>
(KB2761226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Server Core-Installationsoption
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-071**](http://technet.microsoft.com/de-de/security/bulletin/ms12-071)
</td>
<td style="border:1px solid black;">
[**MS12-072**](http://go.microsoft.com/fwlink/?linkid=260820)
</td>
<td style="border:1px solid black;">
[**MS12-074**](http://go.microsoft.com/fwlink/?linkid=255026)
</td>
<td style="border:1px solid black;">
[**MS12-075**](http://go.microsoft.com/fwlink/?linkid=270856)
</td>
<td style="border:1px solid black;">
[**MS12-073**](http://go.microsoft.com/fwlink/?linkid=266541)
</td>
</tr>
<tr class="alternateRow">
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
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
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
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17b987db-0551-45c3-aab1-0cc11ae60dcc) (Server Core-Installation)  
(KB2761226)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=cb3598ae-b647-4aaa-90fb-b4d8aa1cf211)<sup>[1]</sup>
(KB2716513)  
(Mittel)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=8b135d6f-0f6c-4bd5-bf64-d79ae16ac6a5)<sup>[1]</sup>
(KB2716513)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
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
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dd9bd994-41e3-46a1-9dfb-c6d89a3ef883) (Server Core-Installation)  
(KB2761226)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=74d130a4-f42a-48af-87fc-349a1e107529)<sup>[1]</sup>
(KB2716513)  
(Mittel)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=b061a0b0-66e2-49a2-8d20-0c5a6948aecf)<sup>[1]</sup>
(KB2716513)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bbdf1e16-67d9-413c-bad2-31d164fea0da)  
(KB2729451)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=114b596c-36e1-45f5-99e2-f5fdd96b1a30) (Server Core-Installation)  
(KB2761226)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=87f3aa7a-ee84-4e7e-972c-e83a2a06a0ef)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=e1502884-1149-47b8-93af-7f82c5d83819)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=aa5b1e9c-3068-40e3-b04f-6a71f1a51d45)  
(KB2729452)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=f89c10fb-9f85-47b6-8204-d970d7e84e33)<sup>[1]</sup>
(KB2729449)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=ca52497c-8023-42de-b707-2bc1bcee4579)  
(KB2729460)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=4c57041f-0ffc-47c9-82d9-8b1d24d27489)<sup>[1]</sup>
(KB2737019)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=48f57fe1-e180-4b6b-87f5-8dd0c8e821d3)  
(KB2737083)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=114b596c-36e1-45f5-99e2-f5fdd96b1a30) (Server Core-Installation)  
(KB2761226)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=87f3aa7a-ee84-4e7e-972c-e83a2a06a0ef)  
(KB2716513)  
(Mittel)  
[Internetinformationsdienste 7.5](https://www.microsoft.com/download/details.aspx?familyid=e1502884-1149-47b8-93af-7f82c5d83819)  
(KB2719033)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=89faa423-42fa-48ff-be71-8fd58fa523a8)  
(KB2729462)  
(Kritisch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=c9778a0f-264e-476b-8e40-742e0ab56200)  
(KB2737084)  
(Hoch)  
[Microsoft .NET Framework](https://www.microsoft.com/download/details.aspx?familyid=0a7da3d1-a0ac-42a2-9929-b6d831deb9e3)4.5<sup>[2]</sup>
(KB2756872)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=2e69d496-25b4-4f24-97e0-47cb59c178aa) (Server Core-Installation)  
(KB2761226)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis** **für MS12-073**

<sup>[1]</sup>Nicht der standardmäßige FTP-Dienst für dieses Betriebssystem.

**Hinweise für MS12-074**

<sup>[1]</sup>**.NET Framework 4 und .NET Framework 4 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4 und .NET Framework 4 Client Profile. .NET Framework 4 Client Profile ist Teil von .NET Framework 4. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4 als auch .NET Framework 4 Client Profile. Weitere Informationen finden Sie im MSDN-Artikel [Installieren von .NET Framework](http://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

<sup>[2]</sup>Endbenutzer, die Microsoft .NET Framework 4.5 unter Windows 8, Windows Server 2012 oder Windows RT ausführen, sind nicht von diesem Problem betroffen. Das kumulative Update (KB2756872) für die allgemeine Verfügbarkeit von Windows 8 Client und Windows Server 2012, das am 10. Oktober 2012 veröffentlicht wurde, enthält zusätzliche Tiefenverteidigungsänderungen. Endbenutzer, die dieses Update nicht bereits installiert haben, sind angehalten, dies als Tiefenverteidigungsmaßnahme durchzuführen. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 2745030](http://support.microsoft.com/kb/2745030) im Abschnitt „Weitere Informationen“. Downloadadressen und weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 2756872](http://support.microsoft.com/kb/2756872/de). Dieses Update enthält nicht sicherheitsbezogene Inhalte.

<sup>[3]</sup>Sicherheitsupdates für Windows RT werden nur über [Windows Update](http://update.microsoft.com/windowsupdate/) bereitgestellt.

**Hinweis** **für MS12-075**

<sup>[1]</sup>Das Update ist nur über [Windows-Update](http://update.microsoft.com/windowsupdate/) verfügbar.

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
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
[**MS12-076**](http://go.microsoft.com/fwlink/?linkid=260964)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=5bb12b2b-a8e2-4324-afee-e4d26dbc658f)  
(KB2687481)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e12aafe1-4445-4047-ad05-3db151a6fa4e)<sup>[1]</sup>
(KB2687307)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e12aafe1-4445-4047-ad05-3db151a6fa4e)<sup>[1]</sup>
(KB2687307)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 Service Pack 1 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=37a1074d-bf4f-4b96-b394-1edc581748d0)  
(KB2597126)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 Service Pack 1 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=5db02eae-966e-41a9-8b64-ddda5f8b2e2a)  
(KB2597126)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-076**](http://go.microsoft.com/fwlink/?linkid=260964)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=d3d801a2-d57f-4b4c-970a-c296bc716521)  
(KB2764048)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
[Microsoft Office für Mac 2011](https://www.microsoft.com/download/details.aspx?familyid=0f4e073f-4fec-440d-a9bf-1e01ee9e92ad)  
(KB2764047)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Andere Microsoft Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-076**](http://go.microsoft.com/fwlink/?linkid=260964)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Excel Viewer](https://www.microsoft.com/download/details.aspx?familyid=a0917aeb-1e94-4142-bc20-5f1998ac249c)<sup>[2]</sup>
(KB2687313)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=79686714-9418-4516-81c3-555fe1ea9e84)  
(KB2687311)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=79686714-9418-4516-81c3-555fe1ea9e84)  
(KB2687311)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise** **für MS12-076**

<sup>[1]</sup>Für Microsoft Excel 2007 müssen Benutzer zusätzlich zu dem Sicherheitsupdatepaket KB2687307 auch das Sicherheitsupdate für Microsoft Office Compatibility Pack (KB2687311) installieren, um vor der in diesem Bulletin beschriebenen Sicherheitsanfälligkeit geschützt zu sein.

<sup>[2]</sup>Microsoft Excel Viewer muss mit einem unterstützen Service Pack (Excel Viewer 2007 Service Pack 2 oder Excel Viewer 2007 Service Pack 3) aktualisiert werden, bevor dieses Update installiert werden kann. Weitere Informationen zu unterstützten Office Viewer-Versionen finden Sie im [Microsoft Knowledge Base-Artikel 979860](http://support.microsoft.com/kb/979860/de).

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/bb245732). Im [TechNet Sicherheitscenter](http://technet.microsoft.com/de-de/security/default.aspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Endbenutzer können das [Microsoft-Sicherheitscenter](http://www.microsoft.com/de-de/security/default.aspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](http://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. und können am einfachsten durch eine Suche nach dem Begriff „Sicherheitsupdate“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](http://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS12-001“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung:**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](http://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://technet.microsoft.com/de-de/security/cc184924.aspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://technet.microsoft.com/de-de/windowsserver/bb332157.aspx).

**SystemCenter Configuration Manager**

System Center Configuration Manager-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit System Center Configuration Manager können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in System Center Configuration Manager erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in System Center Configuration Manager ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen zu System Center Configuration Manager finden Sie auf der Website [System Center Technical Resources](http://technet.microsoft.com/de-de/systemcenter/bb980621).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de). Die nächste Version von SMS, System Center Configuration Manager, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/download/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/de-de/systemcenter/bb545936).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://technet.microsoft.com/en-us/library/cc917507.aspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet.microsoft.com/de-de/library/cc749197), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](http://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Jose A. Vazquez von spa-s3c.blogspot.com in Zusammenarbeit mit [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf zwei in MS12-071 beschriebene Probleme.
-   [Omair](http://krash.in/) für den Hinweis auf ein in MS12-071 beschriebenes Problem.
-   Cheng-da Tsai (Orange), Sung-ting Tsai und Ming-Chieh Pan (Nanika) von [Trend Micro](http://www.trendmicro.com/) für den Hinweis auf ein in MS12-071 beschriebenes Problem.
-   Tal Zeltzer in Zusammenarbeit mit [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf zwei in MS12-072 beschriebene Probleme.
-   Justin Royce von ProDX für den Hinweis auf ein in MS12-073 beschriebenes Problem.
-   James Forshaw von Context Information Security für den Hinweis auf vier in MS12-074 beschriebene Probleme.
-   [Mateusz „j00 ru“ Jurczyk](http://j00ru.vexillium.org/) von [Google Inc](http://www.google.com) für den Hinweis auf ein in MS12-075 beschriebenes Problem.
-   Eetu Luodemaa und Joni Vähämäki von [Documill](http://www.documill.com) für den Hinweis auf ein in MS12-075 beschriebenes Problem.
-   Sean Larsson in Zusammenarbeit mit [iDefense VCP](http://labs.idefense.com) für den Hinweis auf ein in MS12-076 beschriebenes Problem.
-   Einer Person, die mit [iDefense VCP](http://labs.idefense.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-076 beschriebenes Problem.
-   Einer Person, die mit [iDefense VCP](http://labs.idefense.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-076 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](http://www.hpenterprisesecurity.com/products/hp-tippingpoint-network-security/)[Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-076 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](http://technet.microsoft.com/de-de/security/bb980617.aspx)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](http://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (13. November 2012): Bulletin Summary veröffentlicht.
-   V1.1 (13. November 2012): Für MS12-075 wurde der CVE-Titel sowie die Bewertung der Ausnutzbarkeit durch Denial-of-Service im **Ausnutzbarkeitsindex** für CVE-2012-2897 korrigiert.
-   V2.0 (14. November 2012): Das Bulletin Summary wurde in Bezug auf MS12-073 überarbeitet, um widerzuspiegeln, dass das Update KB2716513 für Windows Vista und Windows Server 2008 jetzt über alle Verteilungskanäle verfügbar ist, einschließlich Windows Update und Microsoft Update. Weitere Informationen finden Sie in dem Bulletin MS12-073.

*Built at 2014-04-18T01:50:00Z-07:00*