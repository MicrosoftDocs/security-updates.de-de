---
TOCTitle: 'MS09-SEP'
Title: Microsoft Security Bulletin Summary für September 2009
ms:assetid: 'ms09-sep'
ms:contentKeyID: 61225078
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-sep(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für September 2009
======================================================

Veröffentlicht: Dienstag, 8. September 2009 | Aktualisiert: Dienstag, 10. November 2009

**Version:** 3.0

In diesem Bulletin Summary sind die im September 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für September 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 3. September 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 9. September 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im September.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032407486&eventcategory=4&culture=en-us&countrycode=us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://technet.microsoft.com/security/bulletin/summary)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=157304">MS09-045</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Skriptmodul JScript kann Remotecodeausführung ermöglichen (971961)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Skriptmodul JScript, das Remotecodeausführung ermöglichen kann, wenn ein Benutzer eine speziell gestaltete Datei öffnet oder eine speziell gestaltete Website besucht und ein fehlerhaftes Skript aufruft. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=151360">MS09-049</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im WLAN-Autokonfigurationsdienst kann Remotecodeausführung ermöglichen (970710)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im WLAN-Autokonfigurationsdienst. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Client oder Server, bei dem eine drahtlose Netzwerkschnittstelle aktiviert ist, speziell gestaltete drahtlose Frames empfängt. Systeme, bei denen keine drahtlose Netzwerkkarte aktiviert ist, sind nicht durch diese Sicherheitsanfälligkeit gefährdet.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=158082">MS09-047</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows Media-Format können Remotecodeausführung ermöglichen (973812)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Windows Media Format. Jede dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Mediendatei öffnet. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=155978">MS09-048</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows TCP/IP können Remotecodeausführung ermöglichen (967723)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in der TCP/IP-Verarbeitung (Transmission Control-Protokoll/Internetprotokoll). Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Angreifer speziell gestaltete TCP/IP-Pakete über das Netzwerk an einen Computer mit einem abfragenden Dienst sendet. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=158009">MS09-046</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im ActiveX-Steuerelement der DHTML-Bearbeitungskomponente kann Remotecodeausführung ermöglichen (956844)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im ActiveX-Steuerelement der DHTML-Bearbeitungskomponente. Ein Angreifer kann die Sicherheitsanfälligkeit ausnutzen, indem er eine speziell gestaltete Website erstellt. Wenn ein Benutzer die Website anzeigt, kann die Sicherheitsanfälligkeit die Codeausführung von Remotestandorten aus ermöglichen. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der angemeldete Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID geordnet.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Kennung des Bulletins                                     | Titel des Bulletins                                                                                                              | CVE-ID                                                                           | Ausnutzbarkeitsindex – Bewertung                                                                                     | Wichtige Hinweise                                                                                                                        |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-045](https://go.microsoft.com/fwlink/?linkid=157304) | Sicherheitsanfälligkeit in Skriptmodul JScript kann Remotecodeausführung ermöglichen (971961)                                    | [CVE-2009-1920](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1920) | [**1**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                  |  
| [MS09-046](https://go.microsoft.com/fwlink/?linkid=158009) | Sicherheitsanfälligkeit im ActiveX-Steuerelement der DHTML-Bearbeitungskomponente kann Remotecodeausführung ermöglichen (956844) | [CVE-2009-2519](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2519) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                                                                                  |  
| [MS09-047](https://go.microsoft.com/fwlink/?linkid=158082) | Sicherheitsanfälligkeiten im Windows Media-Format können Remotecodeausführung ermöglichen (973812)                               | [CVE-2009-2498](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2498) | [**1**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                  |  
| [MS09-047](https://go.microsoft.com/fwlink/?linkid=158082) | Sicherheitsanfälligkeiten im Windows Media-Format können Remotecodeausführung ermöglichen (973812)                               | [CVE-2009-2499](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2499) | [**1**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                                                                                  |  
| [MS09-048](https://go.microsoft.com/fwlink/?linkid=155978) | Sicherheitsanfälligkeiten in Windows TCP/IP können Remotecodeausführung ermöglichen (967723)                                     | [CVE-2008-4609](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4609) | [**3**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dies ist ein Denial-of-Service durch Arbeitsspeichernutzung.                                                                             |  
| [MS09-048](https://go.microsoft.com/fwlink/?linkid=155978) | Sicherheitsanfälligkeiten in Windows TCP/IP können Remotecodeausführung ermöglichen (967723)                                     | [CVE-2009-1925](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1925) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Funktionierender Angreifercode ist möglich, aber wahrscheinlich nicht zuverlässig. Denial-of-Service ist das wahrscheinlichere Resultat. |  
| [MS09-048](https://go.microsoft.com/fwlink/?linkid=155978) | Sicherheitsanfälligkeiten in Windows TCP/IP können Remotecodeausführung ermöglichen (967723)                                     | [CVE-2009-1926](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1926) | [**3**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Dies ist ein Denial-of-Service durch Arbeitsspeichernutzung.                                                                             |  
| [MS09-049](https://go.microsoft.com/fwlink/?linkid=151360) | Sicherheitsanfälligkeit im WLAN-Autokonfigurationsdienst kann Remotecodeausführung ermöglichen (970710)                          | [CVE-2009-1132](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1132) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Durch Heapschutz ist diese Sicherheitsanfälligkeit schwierig zuverlässig auszunutzen.                                                    |
  
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
<th colspan="6" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-045**](https://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](https://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](https://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](https://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](https://go.microsoft.com/fwlink/?linkid=158009)
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
Keine
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[JScript 5.1 und JScript 5.6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2bb3af8d-f36c-4497-9f48-fc59bcff2583)  
(KB971961)  
(Kritisch)  
[JScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=b2773db5-b17d-4b98-b4e2-219b23854abd)  
(KB975542)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.0](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=02b9dc42-38c2-44b1-a77c-34854f4a86c4)  
(KB968816)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4<sup>[3]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6dd4b0f8-6b54-49a6-a6df-9420f9fd3333)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-045**](https://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](https://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](https://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](https://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](https://go.microsoft.com/fwlink/?linkid=158009)
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
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[JScript 5.6 unter Windows XP Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0af373b2-2240-4079-a748-a38d1bc06f39)  
(KB971961)  
(Kritisch)  
[JScript 5.7 unter Windows XP Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c933377d-e0bc-4334-bc75-029045d7a62a)<sup>[1]</sup>
(KB971961)  
(Kritisch)  
[JScript 5.7 unter Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c933377d-e0bc-4334-bc75-029045d7a62a)  
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=992602d8-d857-41cf-b7b1-527afdc1dc0f)<sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.0, Windows Media Format Runtime 9.5 und Windows Media Format Runtime 11](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6ffc081e-f892-4818-acb9-6d79e15d473c)  
(KB968816)  
(Kritisch)  
(Nur Windows XP Service Pack 2)  
[Windows Media Format Runtime 9.0, Windows Media Format Runtime 9.5 und Windows Media Format Runtime 11](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=31585f5a-9aaa-40da-b15a-11284b4b800c)  
(KB968816)  
(Kritisch)  
(Nur Windows XP Service Pack 3)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3<sup>[3]</sup>
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8523d5be-88a2-4124-9b02-660f612e2a12)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=0d671004-da4e-4dbd-a066-861b53b0c59c)  
(KB971961)  
(Kritisch)  
[JScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=9aae426d-ee9a-4736-b0a2-e0f8890a6895)<sup>[1]</sup>
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=00bae02a-64eb-4b91-965f-da2dc987a2ff)<sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.5](https://www.microsoft.com/download/details.aspx?familyid=3780d565-d027-4f54-8fc0-05f5c3c6ba1a)  
(KB968816)  
(Kritisch)  
[Windows Media Format Runtime 9.5 x64 Edition](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ce515188-db3c-4694-85da-177c8f76b68c)  
(KB968816)  
(Kritisch)  
[Windows Media Format Runtime 11](https://www.microsoft.com/download/details.aspx?familyid=9a465f92-3067-4a5a-9882-1fc2cf796c99)  
(KB968816)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2<sup>[3]</sup>
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dbc33f6b-61bf-409a-89b5-60002192e0e0)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-045**](https://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](https://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](https://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](https://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](https://go.microsoft.com/fwlink/?linkid=158009)
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
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6acc9d2d-b71f-4b5c-9aea-b217b6ae240b)  
(KB971961)  
(Kritisch)  
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6af5d034-fd89-42e2-bc18-d44b7a6b0a85)<sup>[1]</sup>
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ecf9f7e2-3104-4de2-8b3d-99dcdcae6e62)<sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4ab34e3d-34cb-4e35-a2da-b348ace8a8f7)  
(KB968816)  
(Kritisch)  
[Windows Media-Dienste 9.1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=61cd0581-c36e-4da6-ae95-41609adbe922)  
(KB972554)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=48d82036-2fde-4bb0-a60e-92eed83ddc3f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7478f73f-dd20-4cfa-a650-4c84f37ada2f)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d0de3ab1-73e9-4a09-841f-81ade41a8c81)  
(KB971961)  
(Kritisch)  
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8f48bc05-ffac-4a21-8d21-dd20355cda8a)<sup>[1]</sup>
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=643f9e2f-2e5b-48dd-b1a0-22ccb633ed18)<sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8654ee33-6083-447f-ae5b-43ef8d8b613d)  
(KB968816)  
(Kritisch)  
[Windows Media Format Runtime 9.5 x64 Edition](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ce515188-db3c-4694-85da-177c8f76b68c)  
(KB968816)  
(Kritisch)  
[Windows Media-Dienste 9.1](https://www.microsoft.com/download/details.aspx?familyid=67c46f26-e6df-4ba2-9c03-1590b31e454c)  
(KB972554)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e0298ddf-026e-4137-8197-ed9d9b889825)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=88bf502d-1a7c-447a-ac4c-401e1698669b)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[JScript 5.6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e78cf021-54f5-4526-b5f0-f781aebf9d72)  
(KB971961)  
(Kritisch)  
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=fb1ca290-cea4-49c0-a37e-613a654bff3c)<sup>[1]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c948c4d8-5788-4c1a-9fb6-a969b06a888d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8d881ff8-f51f-4476-8cb6-2bebd5b2047f)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-045**](https://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](https://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](https://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](https://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](https://go.microsoft.com/fwlink/?linkid=158009)
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
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bcb12e57-f5d6-4b4e-88ab-13c28137f11a)  
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=80e7390f-df39-4d99-b2e1-01c7f6a951bb)<sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e9fe967f-d78d-43c2-bbcc-5098bd20267e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 und Microsoft Media Foundation](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d2bdefcc-f6b9-47c3-a55d-a4f33f967828)  
(KB968816)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7d72f845-9feb-4685-a669-f9d6ab54f9ed)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8b1b76d5-a6b0-4c2f-8768-e55e82c2c118)  
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24457cdd-1973-40c9-9c2d-c1a75fdfa7fa)<sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f93470bd-2e6d-4340-88c6-bb212baf750a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 und Microsoft Media Foundation](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=97f00b25-fb8f-4300-80c0-c63179f32182)  
(KB968816)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b2930ff1-5f0a-4a5d-bf2a-9fb76dd8da63)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-045**](https://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](https://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](https://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](https://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](https://go.microsoft.com/fwlink/?linkid=158009)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=df88e6e5-78d3-4fa6-858d-b935d812cada)\*  
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e7b07be6-a4f8-4847-9c55-9b3d2965fa77)\* <sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ac3f6800-bc3e-4b35-a482-54e1a2da1ab5)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 und Microsoft Media Foundation](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9c111bff-aff6-4ff7-81f6-e736cfcbe3ed)\*\*  
(KB968816)  
(Kritisch)  
[Windows Media-Dienste 2008](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2801f69b-37d0-4d0f-9632-31382b824d36)\*  
(KB972554)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=35c1d5a9-a953-4fc6-90c0-d2358c7b89e6)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f584f8ca-f6b1-4285-a44c-3df5e51e75de)\*  
(KB971961)  
(Kritisch)  
[JScript 5.8](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9eddbb89-4178-49c2-836a-2d292fe50936)\* <sup>[2]</sup>
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7d1b9b4f-bf35-44aa-a660-afb2ef2c9e30)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 und Microsoft Media Foundation](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=59615c8b-a07f-4326-836d-f17b2fcc4695)\*\*  
(KB968816)  
(Kritisch)  
[Windows Media-Dienste 2008](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7fad3793-174f-46db-9d0a-873a0ea8be65)\*  
(KB972554)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6e46822e-f79d-492d-ad01-ee680ad324f5)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b84fca1d-914d-45af-a48c-d9bc5d20c6b7)  
(KB971961)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2ac76ee2-b1b6-4300-9cba-af33d9dd54eb)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008**

**\*Die Server Core-Installation von Windows Server 2008 ist betroffen.** Für unterstützte Editionen von Windows Server 2008 gilt dieses Update mit der gleichen Bewertung des Schweregrads. Dabei spielt es keine Rolle, ob Windows Server 2008 mit der Server Core-Installationsoption installiert wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 nicht, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweise für MS09-045**

<sup>[1]</sup>Auf Systemen mit Internet Explorer 7

<sup>[2]</sup>Auf Systemen mit Internet Explorer 8

**Hinweis für MS09-048**

<sup>[3]</sup> Kein Update verfügbar. Weitere Informationen finden Sie in dem Eintrag **Häufig gestellte Fragen (FAQs) im Zusammenhang mit diesem Sicherheitsupdate** in [MS09-048](https://go.microsoft.com/fwlink/?linkid=155978).

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) und [Windows-Update](https://go.microsoft.com/fwlink/?linkid=21130) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Hinweis:** Am 1. August 2009 hat Microsoft den Support für Office Update und das Inventurprogramm für Office-Update eingestellt. Verwenden Sie [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747), um weiterhin die aktuellen Updates für Microsoft Office-Produkte zu erhalten. Weitere Informationen finden Sie in [Informationen zum Microsoft Office Update: Häufig gestellte Fragen (FAQs)](https://office.microsoft.com/de-de/downloads/fx010402221031.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 für Windows 2000 und neuere Betriebssysteme schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](https://technet.microsoft.com/en-us/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch das Sicherheitsupdate-Inventurprogramm (SUIT) verwenden, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/download/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) und im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Microsoft Application Compatibility Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Ling und Wushi von [team509](https://www.team509.com/) in Zusammenarbeit mit [Zero Day Initiative](https://www.zerodayinitiative.com/) von Tipping Point für den Hinweis auf ein in MS09-045 beschriebenes Problem.
-   Tavis Ormandy von [Google Inc.](https://www.google.com/) für den Hinweis auf ein in MS09-046 beschriebenes Problem.
-   Peter Winter-Smith von [NGS Software](https://www.ngssoftware.com/) für den Hinweis auf ein in MS09-047 beschriebenes Problem.
-   Hiroshi Noguchi vom Alice Carroll-Fanklub für den Hinweis auf ein in MS09-047 beschriebenes Problem.
-   Jack C. Louis von [Outpost24](https://www.outpost24.com/) für den Hinweis auf ein in MS09-048 beschriebenes Problem.
-   Fabian Yamaguchi von [Recurity Labs GmbH](https://www.recurity-labs.com/) für den Hinweis auf ein in MS09-048 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (8. September 2009): Bulletin Summary veröffentlicht.
-   V2.0 (9. September 2009): Windows XP Service Pack 2, Windows XP Service Pack 3 und Windows XP Professional x64 Edition Service Pack 2 wurden der Tabelle „Betroffene Software“ für MS09-048 hinzugefügt. Für diese Plattformen ist jedoch kein Update verfügbar. Siehe den Eintrag in **Häufig gestellte Fragen (FAQs) im Zusammenhang mit diesem Sicherheitsupdate** in MS09-048. Die in diesem Bulletin angebotenen Sicherheitsupdates wurden nicht verändert.
-   V3.0 (10. November 2009): JScript 5.7 unter Microsoft Windows 2000 Service Pack 4 wurde zur Tabelle „Betroffene Software“ für MS09-045 hinzugefügt.

*Built at 2014-04-18T01:50:00Z-07:00*
