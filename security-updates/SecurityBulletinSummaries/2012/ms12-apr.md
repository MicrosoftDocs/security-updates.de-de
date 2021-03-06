---
TOCTitle: 'MS12-APR'
Title: Microsoft Security Bulletin Summary für April 2012
ms:assetid: 'ms12-apr'
ms:contentKeyID: 61225103
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms12-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für April 2012
==================================================

Veröffentlicht: Dienstag, 10. April 2012 | Aktualisiert: Donnerstag, 26. April 2012

**Version:** 2.0

In diesem Bulletin Summary sind die im April 2012 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für April 2012 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 5. April 2012 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 11. April 2012 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im April](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499650). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://go.microsoft.com/fwlink/?linkid=217214)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=242739">MS12-023</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2675157)</strong><br />
<br />
Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=238623">MS12-024</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows kann Remotecodeausführung ermöglichen (2653956)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer oder eine Anwendung eine speziell gestaltete, signierte, übertragbare, ausführbare Datei (PE-Datei; PE = portable executable) auf einem betroffenen System ausführt oder installiert.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=242032">MS12-025</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework kann Remotecodeausführung</strong> <strong>ermöglichen (2671605)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft .NET Framework. Die Sicherheitsanfälligkeit kann Remotecodeausführung auf einem Clientsystem ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite in einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAPs) ausführen kann. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die Sicherheitsanfälligkeit kann auch Remotecodeausführung auf einem Serversystem ermöglichen, auf dem IIS ausgeführt wird, wenn dieser Server die Verarbeitung von ASP.NET-Seiten zulässt und ein Angreifer erfolgreich eine speziell gestaltete ASP.NET-Seite auf den Server hochlädt und dann ausführt, wie es in einem Webhostingszenario der Fall sein kann. Diese Sicherheitsanfälligkeit kann auch von Windows .NET-Anwendungen verwendet werden, um Einschränkungen durch die Codezugriffssicherheit (CAS) zu umgehen. In einem webbasierten Angriffsszenario kann ein Angreifer eine Website mit einer Seite einrichten, die diese Sicherheitsanfälligkeit ausnutzt. Außerdem können manipulierte Websites und Websites, die von Endbenutzern bereitgestellte Inhalte oder Werbemitteilungen akzeptieren oder hosten, speziell gestaltete Inhalte enthalten, über die diese Sicherheitsanfälligkeit ausgenutzt werden kann. Ein Angreifer kann Endbenutzer jedoch nicht zum Besuch solcher Websites zwingen. Er muss den Benutzer zum Besuch dieser Website verleiten. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=246275">MS12-027</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in allgemeinen Windows-Steuerelementen kann Remotecodeausführung ermöglichen (2664258)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in den allgemeinen Windows-Steuerelementen. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Website besucht, die speziell gestaltete Inhalte enthält, mit denen die Sicherheitsanfälligkeit ausgenutzt werden soll. Ein Angreifer kann Benutzer jedoch nicht zum Besuch einer solchen Website zwingen. Der Angreifer muss stattdessen den Benutzer zum Besuch dieser Website verleiten, z. B. indem er den Benutzer dazu auffordert, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken. Die schädliche Datei kann auch als E-Mail-Anlage gesendet werden, aber der Angreifer muss den Benutzer dazu verleiten, die Dateianlage zu öffnen, um die Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft Server-Software,<br />
Microsoft-Entwicklertools</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=238519">MS12-026</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Forefront Unified Access Gateway (UAG) können Offenlegung von Information ermöglichen (2663860)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Forefront Unified Access Gateway (UAG). Die schwerwiegendere der Sicherheitsanfälligkeiten kann Offenlegung von Information ermöglichen, wenn ein Angreifer eine speziell gestaltete Abfrage an den UAG-Server sendet.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Forefront United Access Gateway</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=232498">MS12-028</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office kann Remotecodeausführung ermöglichen (2639185)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office und Microsoft Works. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Works-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/security/cc998259.aspx).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.
  
| Kennung des Bulletins                                     | Titel der Sicherheitsanfälligkeit                                               | CVE-ID                                                                           | Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen                                     | Bewertung der Ausnutzbarkeit für ältere Softwareversionen                                     | Bewertung der Ausnutzbarkeit durch Denial-of-Service | Wichtige Hinweise                                                                                                     |  
|-----------------------------------------------------------|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|  
| [MS12-023](https://go.microsoft.com/fwlink/?linkid=242739) | Sicherheitsanfälligkeit in Jscript9 bezüglich Remotecodeausführung              | [CVE-2012-0169](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0169) | [3](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode unwahrscheinlich | Nicht betroffen                                                                               | Vorläufig                                            | (Keine)                                                                                                               |  
| [MS12-023](https://go.microsoft.com/fwlink/?linkid=242739) | Sicherheitsanfälligkeit in OnReadyStateChange bezüglich Remotecodeausführung    | [CVE-2012-0170](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0170) | Nicht betroffen                                                                                 | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich | Vorläufig                                            | (Keine)                                                                                                               |  
| [MS12-023](https://go.microsoft.com/fwlink/?linkid=242739) | Sicherheitsanfälligkeit in SelectAll bezüglich Remotecodeausführung             | [CVE-2012-0171](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0171) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich   | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich | Vorläufig                                            | (Keine)                                                                                                               |  
| [MS12-023](https://go.microsoft.com/fwlink/?linkid=242739) | Sicherheitsanfälligkeit in VML-Stil bezüglich Remotecodeausführung              | [CVE-2012-0172](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0172) | Nicht betroffen                                                                                 | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich | Vorläufig                                            | (Keine)                                                                                                               |  
| [MS12-024](https://go.microsoft.com/fwlink/?linkid=238623) | Sicherheitsanfälligkeit in WinVerifyTrust bei Signaturüberprüfung               | [CVE-2012-0151](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0151) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich   | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich | Nicht anwendbar                                      | (Keine)                                                                                                               |  
| [MS12-025](https://go.microsoft.com/fwlink/?linkid=242032) | Sicherheitsanfälligkeit in .NET Framework bezüglich Überprüfung der Parameter   | [CVE-2012-0163](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0163) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich   | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich | Nicht anwendbar                                      | (Keine)                                                                                                               |  
| [MS12-026](https://go.microsoft.com/fwlink/?linkid=238519) | Sicherheitsanfälligkeit durch ungefilterten Zugriff auf die UAG-Standardwebsite | [CVE-2012-0147](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0147) | [3](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode unwahrscheinlich | Nicht betroffen                                                                               | Nicht anwendbar                                      | Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.                        |  
| [MS12-027](https://go.microsoft.com/fwlink/?linkid=246275) | Sicherheitsanfälligkeit in MSCOMCTL.OCX bezüglich Remotecodeausführung          | [CVE-2012-0158](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0158) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich   | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich | Nicht anwendbar                                      | Microsoft ist sich gezielter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.    |  
| [MS12-028](https://go.microsoft.com/fwlink/?linkid=232498) | Sicherheitsanfälligkeit in Office WPS-Konverter durch Heapüberlauf              | [CVE-2012-0177](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0177) | [3](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode unwahrscheinlich | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich | Nicht anwendbar                                      | Microsoft Office 2007 Service Pack 3 und alle unterstützten Editionen von Microsoft Office 2010 sind nicht betroffen. |
  
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
<th colspan="4" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-023**](https://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](https://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](https://go.microsoft.com/fwlink/?linkid=242032)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=2a490c62-16c4-402a-b2d9-3e8cfb5bcebd)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=81b28dd9-87aa-46cc-94c6-2da39d0298db)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=74ce0e29-046b-4ac3-89a1-b292a177972f)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=575afd20-cee4-4fa9-b781-9f8dfdd41ebe)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=1cfeae57-d4e9-4fff-8956-523e7b71453c)  
(KB2656378)  
(Nur Media Center Edition 2005 und Tablet PC Edition 2005)  
(Kritisch)  
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=a1b7be43-a32e-456b-8df0-c26cdf187682)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=29ec7b06-c7aa-4149-bb2c-25af7d38a6a9)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=646c6352-4d99-413a-a75b-71289b5d2b25)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=adc31695-1be6-4976-869c-007df8ac8508)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-023**](https://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](https://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](https://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=020e0d68-dd1c-4297-b565-fcc6dcf5f280)  
(KB2675157)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=17b0c139-2709-424d-9d17-827af468e858)  
(KB2675157)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=3289a80a-d1b1-4494-bede-03d0be579acf)  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f79c8940-ca31-4ff7-924e-847f5eef7864)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ffd26218-e149-44ea-a0b9-f2a1315fce9e)  
(KB2656376)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=295292d3-01a3-4574-b994-8cdbcf5a0d2e)  
(KB2675157)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=04656a93-e958-4764-afe8-27c476855506)  
(KB2675157)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=dff4fb63-b319-49ed-8a9d-6b15e43d5bfd)  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=03ebf111-1e7b-4dc2-b84f-a26c6b5f0d58)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=09011393-c7d5-4225-9b8e-5a234d4dbcd1)  
(KB2675157)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a5ef0147-595e-43b5-819f-73780fcef10d)  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=734ff97a-7d72-4bfe-9557-7fac91902f8e)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
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
[**MS12-023**](https://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](https://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](https://go.microsoft.com/fwlink/?linkid=242032)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=f598cad1-4d1a-40ce-a016-bb58778d5dc0)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=44284277-06a7-405d-9187-8f50a042604d)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=51088164-13b7-4216-90f1-20c92c8b8ca9)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c7683919-6d46-4b3e-aa98-1bef20141835)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=2717a997-2066-4a83-ae9b-4611a0851101)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=19684033-ddeb-464f-9a22-f580a9c19f8e)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=bbb99aee-aadd-4ec7-9e27-91cb8d90803e)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4d9f8a6e-17bd-4ed3-8bc7-d5e3b11ca12a)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-023**](https://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](https://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](https://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=3e361edd-234b-4053-aa49-278b9fde4d5c)\*\*  
(KB2675157)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=6eb6781e-7b38-4679-afbc-4e3bb5747fd8)\*\*  
(KB2675157)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=d34d7981-ed63-460d-95e4-e6da1ac41d2f)\*\*  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c36c20f7-a742-4151-b8f2-85ef80479d06)\*  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=60b76a3c-4530-4101-931f-45df621e1eed)\*\*  
(KB2675157)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=fd657467-a45c-4354-b947-3a3cceb9b690)\*\*  
(KB2675157)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c9d773e9-6a2e-45db-8f30-7da0082d909c)\*\*  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=330cea47-221d-439e-b106-58a146fc28ee)\*  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=3235216f-497f-4934-81b8-1eb9929e98c9)  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1ec74522-ec1e-4b3c-bfeb-6a505cc4f11a)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-023**](https://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](https://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](https://go.microsoft.com/fwlink/?linkid=242032)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-023**](https://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](https://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](https://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)\*  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)\*  
(KB2656372)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)\*  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)\*  
(KB2656373)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)\*<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/de-de/server/windows-server/2008/editionen.aspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/de-de/server/windows-server/2008/editionen.aspx).

**Hinweis** **für** **MS12-025**

<sup>[1]</sup>**.NET Framework 4 und .NET Framework 4 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4 und .NET Framework 4 Client Profile. .NET Framework 4 Client Profile ist Teil von .NET Framework 4. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4 als auch .NET Framework 4 Client Profile. Weitere Informationen finden Sie im MSDN-Artikel [Installieren von .NET Framework](https://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office Suites und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](https://go.microsoft.com/fwlink/?linkid=232498)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(Allgemeine Windows-Steuerelemente)  
(KB2597112)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fbf24cc6-89e1-48dd-bb83-23eed30195e1)  
(KB2596871)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(Allgemeine Windows-Steuerelemente)  
(KB2598039)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(Allgemeine Windows-Steuerelemente)  
(KB2598039)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office Web Components
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](https://go.microsoft.com/fwlink/?linkid=232498)
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
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Web Components Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Web Components Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(Allgemeine Windows-Steuerelemente)  
(KB2597112)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Andere Microsoft Office-Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](https://go.microsoft.com/fwlink/?linkid=232498)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](https://www.microsoft.com/download/details.aspx?familyid=94e17a66-cf09-4314-89ec-53deadabfa66)  
(KB2680317)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 6-9-Dateikonverter
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Works 6-9-Dateikonverter](https://www.microsoft.com/download/details.aspx?familyid=4605f684-6314-4758-adeb-2a8810dfc8d1)  
(KB2680326)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS12-027**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Analysis Services Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=198f1819-818b-4b2e-a424-4a45729746eb)  
(KB983807)  
(Kritisch)  
GDR-Update:  
[Microsoft SQL Server 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2a9d97e8-79e0-4997-88fe-1224707e1b37)  
(KB983808)  
(Kritisch)  
QFE-Update:  
[Microsoft SQL Server 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=8d0cac2f-f227-4e00-9454-4df62be86407)  
(KB983809)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SQL Server-Komponenten
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2005 für 32-Bit-Systeme Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 für 32-Bit-Systeme Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2597112)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2005 für Itanium-basierte Systeme Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 für Itanium-basierte Systeme Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2597112)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2005 für x64-basierte Systeme Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 für x64-basierte Systeme Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2597112)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2005 Express Edition mit Advanced Services Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 Express Edition mit Advanced Services Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2597112)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 für 32-Bit-Systeme Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 für x64-basierte Systeme Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 für Itanium-basierte Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 für Itanium-basierte Systeme Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Allgemeine Windows-Steuerelemente)  
(KB2598041)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweise** **für** **MS12-027**

<sup>[1]</sup>Dieses Update ist identisch mit dem KB2597112-Update für Microsoft Office 2003.

<sup>[2]</sup>Dieses Update ist identisch mit dem KB2598041-Update für Microsoft Office 2007.

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft BizTalk Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft BizTalk Server 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft BizTalk Server 2002 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d90b78d2-551b-499b-9bd2-85b40646dbc7)  
(KB2645025)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Commerce Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2002 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2002 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=35de8833-50ae-482d-aa07-497bf68fb38e)  
(KB2658674)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3f04fb90-8f11-4392-a4bc-800903091f04)  
(KB2658677)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2009
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009](https://www.microsoft.com/download/details.aspx?familyid=a8998b6b-e9a4-457e-a34f-0458dda81f2f)  
(KB2655547)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2009 R2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009 R2](https://www.microsoft.com/download/details.aspx?familyid=e9221811-8913-412b-ae04-21a55ce7c4c5)  
(KB2658676)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweis für MS12-027**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Visual FoxPro
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3a7ff474-f1e0-4c86-9555-64e8e7357890)  
(KB2647488)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=53c0132e-7724-4e94-abe9-e79b76ce35d7)  
(KB2647490)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Visual Basic
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-027**](https://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Basic 6.0 Runtime
</td>
<td style="border:1px solid black;">
[Visual Basic 6.0 Runtime](https://www.microsoft.com/download/details.aspx?familyid=0afe933a-1e62-45c4-910c-ea94b203df5a)  
(KB2641426)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweis für MS12-027**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft-Software für Remotezugriff

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Forefront Unified Access Gateway
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-026**](https://go.microsoft.com/fwlink/?linkid=238519)
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
Microsoft Forefront Unified Access Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d4b4ecc4-8bc6-43d0-b872-93673e0d9a6f)<sup>[1]</sup>
(KB2649261)  
(Hoch)  
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1 Update 1](https://www.microsoft.com/download/details.aspx?familyid=e0f9acab-bfb8-4758-b60d-64e68a84fba0)<sup>[1]</sup>
(KB2649262)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis** **für** **MS12-026**

<sup>[1]</sup>Dieses Update ist nur im Microsoft Download Center verfügbar.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheitscenter](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung:**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://technet.microsoft.com/de-de/windowsserver/bb332157).

**System Center Configuration Manager 2007**

Configuration Manager 2007-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit Configuration Manager 2007 können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in Configuration Manager 2007 erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in Configuration Manager 2007 ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen dazu, wie Administratoren mithilfe von Configuration Manager 2007 Updates bereitstellen können, finden Sie in [Softwareupdateverwaltung](https://www.microsoft.com/germany/systemcenter/sccm/evaluation/updatemgmt.mspx). Weitere Informationen zu Configuration Manager finden Sie auf der Website [System Center Configuration Manager](https://www.microsoft.com/de-de/server/system-center/configuration-manager/default.aspx).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](https://support.microsoft.com/common/international.aspx?rdpath=dm;de-de;lifecycle). Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager 2007**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](https://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://technet.microsoft.com/en-us/library/cc917507.aspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   linx2008 von [AISec](https://www.aisec.cn/) für den Hinweis auf ein in MS12-023 beschriebenes Problem.
-   Roel Spilker von [TOPdesk](https://www.topdesk.com) für den Hinweis auf ein in MS12-023 beschriebenes Problem.
-   Jose Antonio Vazquez Gonzalez in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com) für den Hinweis auf ein in MS12-023 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](https://www.tippingpoint.com)[Zero Day Initiative](https://www.zerodayinitiative.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-023 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](https://www.tippingpoint.com)[Zero Day Initiative](https://www.zerodayinitiative.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-023 beschriebenes Problem.
-   Masato Kinugawa für die Zusammenarbeit mit uns an den in MS12-023 enthaltenen Tiefenverteidigungsänderungen.
-   Robert Zacek und Igor Glucksmann von [Avast Software](https://www.avast.com/) für den Hinweis auf ein in MS12-024 beschriebenes Problem.
-   Vitaliy Toropov in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS12-025 beschriebenes Problem.
-   Shaun Colley von [IOActive, Ltd.](https://ioactive.co.uk/) für den Hinweis auf ein in MS12-028 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (10. April 2012): Bulletin Summary veröffentlicht.
-   V2.0 (26. April 2012): In MS12-027 wurden der Tabelle der betroffenen Software Service Pack 1-Versionen von SQL Server 2008 R2 hinzugefügt. Unter „Betroffene Software“ wurde verdeutlicht, dass das Update für alle Installationen von Microsoft SQL Server 2000 Analysis Services Service Pack 4 gilt, da die Unterscheidung zwischen QFE und GDR nicht auf dieses Produkt zutrifft. Dies sind lediglich Informationsänderungen. An den Dateien des Sicherheitsupdates oder der Erkennungslogik wurden keine Änderungen vorgenommen. Da die Updates seit der anfänglichen Veröffentlichung richtig angeboten wurden, müssen Benutzer, die diese Updates bereits erfolgreich installiert haben, keine Maßnahmen ergreifen.

*Built at 2014-04-18T01:50:00Z-07:00*