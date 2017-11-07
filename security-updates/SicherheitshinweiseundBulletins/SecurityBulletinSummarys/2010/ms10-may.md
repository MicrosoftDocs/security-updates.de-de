---
TOCTitle: 'MS10-MAY'
Title: Microsoft Security Bulletin Summary für Mai 2010
ms:assetid: 'ms10-may'
ms:contentKeyID: 61225087
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms10-may(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Mai 2010
================================================

Veröffentlicht: Dienstag, 11. Mai 2010 | Aktualisiert: Mittwoch, 19. Mai 2010

**Version:** 1.2

In diesem Bulletin Summary sind die im Mai 2010 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Mai 2010 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 6. Mai 2010 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 12. Mai 2010 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Mai](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032427724&culture=en-us). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://www.microsoft.com/germany/technet/sicherheit/bulletins/aktuell/default.mspx)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

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
<th style="border:1px solid black;" >Neustartanforderung:</th>
<th style="border:1px solid black;" >Betroffene Software</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx">MS10-030</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Outlook Express und Windows Mail kann Remotecodeausführung ermöglichen (978542)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Outlook Express, Windows Mail und Windows Live Mail. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer einen schädlichen E-Mail Server besucht. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-031.mspx">MS10-031</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Visual Basic für Applikationen kann Remotecodeausführung ermöglichen (978213)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Visual Basic für Applikationen. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn eine Hostanwendung geöffnet wird und eine speziell gestaltete Datei an Visual Basic für Applikationen-Runtime übergibt. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office, Microsoft Visual Basic für Applikationen</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach absteigender Bewertung der Ausnutzbarkeit und dann CVE ID aufgeführt. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259.aspx).
  
| Kennung des Bulletins                                                                   | Titel der Sicherheitsanfälligkeit                                                       | CVE-ID                                                                           | Ausnutzbarkeitsindex – Bewertung                                                                                 | Wichtige Hinweise                                                                                                                  |  
|-----------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-031](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-031.mspx) | Sicherheitsanfälligkeit im VBE6.DLL-Stapel bezüglich Speicherbeschädigung               | [CVE-2010-0815](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0815) | [**2**](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich | (Keine)                                                                                                                            |  
| [MS10-030](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx) | Sicherheitsanfälligkeit in Outlook Express und Windows Mail bezüglich Ganzzahlüberlaufs | [CVE-2010-0816](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0816) | [**2**](http://technet.microsoft.com/de-de/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich | Ausnutzung unter Windows Vista und höheren Betriebssystemen ist aufgrund von schadensbegrenzenden Maßnahmen weniger wahrscheinlich |
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
#### Systemkomponenten des Windows-Betriebssystems

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
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 5.5 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=661f5de3-a593-4961-8e8d-2777797eb5c5)  
(KB978542)  
(Kritisch)  
[Microsoft Outlook Express 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cda75174-b535-4559-a52d-b5ec3a1df349)  
(KB978542)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=99707c3d-a3cb-47da-b38e-8ae0227fd703)  
(KB978542)  
(Kritisch)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=99707c3d-a3cb-47da-b38e-8ae0227fd703)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=44bc97bb-6f76-4c96-af72-69daaea80fff)  
(KB978542)  
(Kritisch)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=44bc97bb-6f76-4c96-af72-69daaea80fff)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=eb9742fc-0934-4b38-9ec4-3597fc71ec00)  
(KB978542)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=5678515a-97ea-4e00-8700-d3f2fcdc0efc)  
(KB978542)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=60ef635b-cb6d-402f-b904-e69b519d797f)  
(KB978542)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=a970c869-24fe-4ef4-b189-7a6bac2411f1)  
(KB978542)  
(Kritisch)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=a970c869-24fe-4ef4-b189-7a6bac2411f1)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=9a7853b5-4f9f-4467-9530-eea2efd504a5)  
(KB978542)  
(Kritisch)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=9a7853b5-4f9f-4467-9530-eea2efd504a5)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=5f77a640-247c-4ed2-9fca-4b7344f4dc7c)\*\*  
(KB978542)  
(Kritisch)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=5f77a640-247c-4ed2-9fca-4b7344f4dc7c)\*\*<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=b0eab011-5847-44e4-bc0d-5c5355e1e8d0)\*\*  
(KB978542)  
(Kritisch)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=b0eab011-5847-44e4-bc0d-5c5355e1e8d0)\*\*<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=da01ae82-895e-4739-916f-a63b9095a076)  
(KB978542)  
(Kritisch)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=da01ae82-895e-4739-916f-a63b9095a076)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=1f0c17be-ba4c-4a1c-b9c3-8ac368800947)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=a70f15e1-512c-44ca-a308-928e237ac0ce)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-030.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=e2e25c02-38ce-4868-a01a-39fc7d2a4150)\*\* <sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=53ed1055-b5ee-4fde-9550-f8b401916467)<sup>[1]</sup>  
(KB978542)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für Windows Server 2008 und Windows Server 2008 R2**

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den MSDN-Artikeln [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) und [Server Core für Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS10-030**

<sup>[1]</sup>Windows Live Mail ist eine gebrauchsfertige Komponente auf diesem Betriebssystem, die separat installiert werden muss, damit die Sicherheitsanfälligkeit existiert.

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
Microsoft Office Suites, Systeme und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-031**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-031.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=72c23b0f-4e24-4334-bc8a-334adc8bc42b)<sup>[1]</sup>   
(KB976380)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f8eac9bc-8389-4ac8-8b29-9a8180d9fd34)<sup>[1]</sup>   
(KB976382)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office System 2007 Service Pack 1 und Microsoft Office System 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=160ad53e-6475-4550-90c2-444e4abea730)<sup>[1]</sup>   
(KB976321)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für MS10-031**

<sup>[1]</sup>Diese Updates für Microsoft Office gelten für alle unterstützten Microsoft Office Suites und weitere Microsoft Office-Software, die die anfällige, gemeinsam genutzte Office-Komponente enthalten. Dieses beinhaltet, ist aber nicht beschränkt auf, unterstützte Versionen von Microsoft Office Visio und Microsoft Office Project.

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft Entwicklertools und Software

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
Microsoft Visual Basic für Applikationen
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-031**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms10-031.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Basic für Applikationen
</td>
<td style="border:1px solid black;">
[Microsoft Visual Basic für Applikationen](http://www.microsoft.com/downloads/details.aspx?familyid=436a8a66-352e-44d1-a610-c825083ad24a)<sup>[1]</sup>  
(KB974945)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Basic für Applikationen SDK
</td>
<td style="border:1px solid black;">
Microsoft Visual Basic für Applikationen SDK<sup>[2]</sup><sup>[3]</sup>  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweise für MS10-031**

<sup>[1]</sup>Dieses Updatepaket gilt für unterstützte Versionen der Microsoft Visual Basic für Applikationen-Runtime (Vbe6.dll) und ist nur im Microsoft Download Center verfügbar.

<sup>[2]</sup>Die unterstützten Versionen des VBA SDK sind Microsoft Visual Basic für Applikationen SDK 6.3, Microsoft Visual Basic für Applikationen SDK 6.4 und Microsoft Visual Basic für Applikationen SDK 6.5.

<sup>[3]</sup>Die aktualisierte Version der Visual Basic für Applikationen SDK, mit der die in diesem Bulletin beschriebene Sicherheitsanfälligkeit behoben wird, ist für unabhängige Softwareanbieter von der [Summit Software Company](http://www.summsoft.com/) erhältlich.

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) und [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Hinweis:** Am 1. August 2009 hat Microsoft den Support für Office Update und das Inventurprogramm für Office-Update eingestellt. Verwenden Sie [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), um weiterhin die aktuellen Updates für Microsoft Office-Produkte zu erhalten. Weitere Informationen finden Sie in [Informationen zum Microsoft Office Update: Häufig gestellte Fragen (FAQs)](http://office.microsoft.com/de-de/downloads/fx010402221031.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](http://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](http://technet.microsoft.com/de-de/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch das Sicherheitsupdate-Inventurprogramm (SUIT) verwenden, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](http://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Microsoft Application Compatibility Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Francis Provencher vom Protek Research Lab für den Hinweis auf ein in MS10-030 beschriebenes Problem.
-   [NSFocus Security Team](http://www.nsfocus.com/) für den Hinweis auf ein in MS10-031 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](http://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (11. Mai 2010): Bulletin Summary veröffentlicht.
-   V1.1 (12. Mai 2010): Die Neustartanforderungen für MS10-030 wurden korrigiert.
-   V1.2 (19. Mai 2010): In MS10-030 wurden fehlerhafte Verweise auf Windows Mail bei Installation unter Windows 7 und Windows Server 2008 R2 entfernt. Außerdem wurde MS10-031 ein zusätzlicher Hinweis zur betroffenen Software hinzugefügt, um zu erklären, dass die Updates für Microsoft Office für alle unterstützten Microsoft Office Suites und weitere Microsoft Office-Software gelten, die eine anfällige Version von VBE6.dll enthalten.

*Built at 2014-04-18T01:50:00Z-07:00*
