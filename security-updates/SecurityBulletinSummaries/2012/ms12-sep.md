---
TOCTitle: 'MS12-SEP'
Title: Microsoft Security Bulletin Summary für September 2012
ms:assetid: 'ms12-sep'
ms:contentKeyID: 61225114
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms12-sep(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für September 2012
======================================================

Veröffentlicht: Dienstag, 11. September 2012 | Aktualisiert: Freitag, 21. September 2012

**Version:** 2.0

In diesem Bulletin Summary sind die im September 2012 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für September 2012 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 19. September 2012 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, den 12. September 2012 um 20:00 Uhr (MEZ) führt Microsoft einen englischsprachigen Webcast durch, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im September.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032522555&culture=de-de) Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032522555&culture=de-de) zur Verfügung.

Am 21. September 2012 um 12:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesem außerplanmäßigen Security Bulletin zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im September.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032529852&culture=en-us) Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032529852&culture=en-us) zur Verfügung.

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=255505">MS12-063</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2744842)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich und vier vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=254184">MS12-061</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Visual Studio Team Foundation Server kann Erhöhung von Berechtigungen ermöglichen (2719584)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Visual Studio Team Foundation Server. Die Sicherheitsanfälligkeit kann Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer auf einen speziell gestalteten Link in einer E-Mail-Nachricht klickt oder zu einer Webseite navigiert, mit der die Sicherheitsanfälligkeit ausgenutzt wird. Ein Angreifer kann Endbenutzer jedoch nicht zum Ausführen solcher Aktionen zwingen. Der Angreifer muss stattdessen den Benutzer zum Besuch einer Website verleiten, z. B. indem er den Benutzer dazu auffordert, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Kein Neustart erforderlich</td>
<td style="border:1px solid black;">Microsoft-Entwicklertools</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=261858">MS12-062</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in System Center Configuration Manager</strong> <strong>kann Erhöhung von Berechtigungen ermöglichen (2741528)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft System Center Configuration Manager. Die Sicherheitsanfälligkeit kann Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer über eine speziell gestaltete URL eine betroffene Website besucht. Ein Angreifer kann Benutzer nicht zum Besuch einer solchen Website zwingen. Er muss den Benutzer zum Besuch dieser Website verleiten. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Kein Neustart erforderlich</td>
<td style="border:1px solid black;">Microsoft Server-Software</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/security/cc998259.aspx).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel der Sicherheitsanfälligkeit</th>
<th style="border:1px solid black;" >CVE-ID</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit für ältere Softwareversionen</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit durch Denial-of-Service</th>
<th style="border:1px solid black;" >Wichtige Hinweise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=254184">MS12-061</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch siteübergreifende Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1892">CVE-2012-1892</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=261858">MS12-062</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit aufgrund reflektierter siteübergreifender Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2536">CVE-2012-2536</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=255505">MS12-063</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in OnMove</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1529">CVE-2012-1529</a></td>
<td style="border:1px solid black;">Nicht betroffen[1]</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=255505">MS12-063</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Ereignislistener</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2546">CVE-2012-2546</a></td>
<td style="border:1px solid black;">Nicht betroffen[1]</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=255505">MS12-063</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit im Layout</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2548">CVE-2012-2548</a></td>
<td style="border:1px solid black;">Nicht betroffen[1]</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=255505">MS12-063</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in cloneNode</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-2557">CVE-2012-2557</a></td>
<td style="border:1px solid black;">Nicht betroffen[1]</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=255505">MS12-063</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in execCommand</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-4969">CVE-2012-4969</a></td>
<td style="border:1px solid black;">Nicht betroffen[1]</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde veröffentlicht.<br />
<br />
Microsoft ist sich begrenzter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
</tbody>
</table>
 

<sup>[1]</sup>Internet Explorer 10 ist von dieser Sicherheitsanfälligkeit nicht betroffen.

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
<th colspan="2" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-063**](https://go.microsoft.com/fwlink/?linkid=255505)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=967c9ef3-db48-4c2f-9a67-87851fd54962)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=6ba78d4c-3657-4963-b2da-7a3763c6b5c9)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=ac71ffe3-f077-4753-a238-47a2e9623363)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=020b36c6-7050-4458-8762-bae35eb713cd)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=1e2e412a-be97-407e-9f02-fc074db3bb07)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c727d956-be3e-4cd2-913c-f26cb6c33227)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-063**](https://go.microsoft.com/fwlink/?linkid=255505)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=7aaaa15b-87d8-4afc-b183-8ce5becda026)  
(KB2744842)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=aef34ce4-a6ce-4f5e-9892-0a7fbd90c3b4)  
(KB2744842)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d63e25ad-ab8c-425f-89cd-29cd2b7b69d6)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=366feacb-16ad-455c-b2ad-5038f998c432)  
(KB2744842)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=baa47c53-2724-43ef-8590-d3733b47e75b)  
(KB2744842)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=84144e56-f653-4c92-bf49-d44d9ba10489)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=c28d6dc3-c2f0-4505-a545-85b7a0e3e2dc)  
(KB2744842)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=86c28695-86a5-4c17-82d6-7f98b3162aa6)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-063**](https://go.microsoft.com/fwlink/?linkid=255505)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=053546fc-ed41-43c2-b4f2-b76334314f5c)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=0a5a446d-0a48-4eec-b424-87339b34a3be)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=daba1ef1-62db-43db-9d5b-495aa2d3550f)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=cbe5681b-c28e-4a6a-9b97-0bfe44acf077)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=5642136e-68f6-42e8-b48e-1549733c6e7d)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=aae496ef-fca2-4632-9a8f-2108722d2b28)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-063**](https://go.microsoft.com/fwlink/?linkid=255505)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=df861b42-bcf2-4f7a-9019-f49e6725f5dc)  
(KB2744842)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=1d4f0f25-9539-4c38-babb-4af7f0f4c6cf)  
(KB2744842)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=0b2965d7-e0b2-4035-a9e4-f6badb389098)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=fa9878c0-b7e5-43ac-b1eb-679e62cf62fc)  
(KB2744842)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=10bab7d4-0dd8-4fa7-b26c-715a68553707)  
(KB2744842)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=612a94ef-0950-41e8-9875-a8f0e71eba6f)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=ded887a4-a06d-4447-b19d-19d0f4928523)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-063**](https://go.microsoft.com/fwlink/?linkid=255505)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=93591461-39ff-4cbd-8df3-88cb80ed6255)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=b303f86a-df17-4961-b677-0c38bd6a86d3)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=93591461-39ff-4cbd-8df3-88cb80ed6255)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=b303f86a-df17-4961-b677-0c38bd6a86d3)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e2083388-19a9-4754-9449-1dad2a7f7543)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=01045ee2-c7c4-4078-969f-905fd7e8774f)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e2083388-19a9-4754-9449-1dad2a7f7543)  
(KB2744842)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=01045ee2-c7c4-4078-969f-905fd7e8774f)  
(KB2744842)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-063**](https://go.microsoft.com/fwlink/?linkid=255505)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d46ec8ea-b8c8-42d9-a201-f36eb97b91b8)  
(KB2744842)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c44a0253-fefc-4ce6-9cfd-396fdea71f8d)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d46ec8ea-b8c8-42d9-a201-f36eb97b91b8)  
(KB2744842)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c44a0253-fefc-4ce6-9cfd-396fdea71f8d)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c132173b-f869-47ec-bb70-6307081473fe)  
(KB2744842)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c132173b-f869-47ec-bb70-6307081473fe)  
(KB2744842)  
(Mittel)
</td>
</tr>
</table>
 

#### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Visual Studio Team Foundation Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-061**](https://go.microsoft.com/fwlink/?linkid=254184)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio Team Foundation Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio Team Foundation Server 2010 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=721c4a38-b255-4792-83a5-7526a680a79a)<sup>[1]</sup>
(KB2719584)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS12-061**

<sup>[1]</sup>Dieses Update ist kumulativ und ersetzt vorherige kumulative Updates für die angegebene Software.

#### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft System Center Configuration Manager
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS12-062**](https://go.microsoft.com/fwlink/?linkid=261858)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Systems Management Server 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Systems Management Server 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f3a3d8e1-d551-43b4-9d54-9536f30c074d)<sup>[1]</sup>
(KB2733631)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft System Center Configuration Manager 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft System Center Configuration Manager 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=89890c0e-118b-49ea-9fd1-6d23c674f9e8)<sup>[1]</sup>
(KB2721642)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS12-062**

<sup>[1]</sup>Dieses Update ist nur im Microsoft Download Center verfügbar.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/bb245732). Im [TechNet Sicherheitscenter](https://technet.microsoft.com/de-de/security/default.aspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Endbenutzer können das [Microsoft-Sicherheitscenter](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS12-001“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung:**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://technet.microsoft.com/de-de/security/cc184924.aspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx).

**SystemCenter Configuration Manager**

System Center Configuration Manager-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit System Center Configuration Manager können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in System Center Configuration Manager erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in System Center Configuration Manager ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen zu System Center Configuration Manager finden Sie auf der Website [System Center Technical Resources](https://technet.microsoft.com/de-de/systemcenter/bb980621).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de). Die nächste Version von SMS, System Center Configuration Manager, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/download/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](https://technet.microsoft.com/de-de/systemcenter/bb545936).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://technet.microsoft.com/en-us/library/cc917507.aspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc749197), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Sunil Yadav von INR Labs ([Network Intelligence India](https://niiconsulting.com/)) für den Hinweis auf ein in MS12-061 beschriebenes Problem.
-   Andy Yang von [Stratsec](https://www.stratsec.net) für den Hinweis auf ein in MS12-062 beschriebenes Problem.
-   Einer Person, die mit [VeriSign iDefense Labs](https://labs.idefense.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-063 beschriebenes Problem.
-   [Rosario Valotta](https://sites.google.com/site/tentacoloviola) für den Hinweis auf ein in MS12-063 beschriebenes Problem.
-   Stephen Fewer von [Harmony Security](https://www.harmonysecurity.com/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.hpenterprisesecurity.com/products/hp-tippingpoint-network-security/) für den Hinweis auf ein in MS12-063 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](https://www.hpenterprisesecurity.com/products/hp-tippingpoint-network-security/)[Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-063 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](https://www.hpenterprisesecurity.com/products/hp-tippingpoint-network-security/)[Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS12-063 beschriebenes Problem.
-   [Mitre](https://www.mitre.org/) für die Zusammenarbeit mit uns an einem in MS12-063 beschriebenen Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617.aspx)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (11. September 2012): Bulletin Summary veröffentlicht.
-   V2.0 (21. September 2012): Microsoft Security Bulletin MS12-063, kumulatives Sicherheitsupdate für Internet Explorer (2744842), wurde hinzugefügt. Außerdem wurde der Bulletin-Webcastlink für dieses außerplanmäßige Security Bulletin hinzugefügt.

*Built at 2014-04-18T01:50:00Z-07:00*