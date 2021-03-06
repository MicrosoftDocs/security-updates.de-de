---
TOCTitle: 'MS09-MAR'
Title: Microsoft Security Bulletin Summary für März 2009
ms:assetid: 'ms09-mar'
ms:contentKeyID: 61225074
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-mar(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für März 2009
=================================================

Veröffentlicht: Dienstag, 10. März 2009 | Aktualisiert: Mittwoch, 11. März 2009

**Version:** 1.1

In diesem Bulletin Summary sind die im März 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für März 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 5. März 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 11. März 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im März](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395124). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://technet.microsoft.com/security/bulletin/summary)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=132503">MS09-006</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Remotecodeausführung ermöglichen (958690)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten im Windows-Kernel. Die schwerwiegendere Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete EMF- oder WMF-Bilddatei von einem betroffenen System anzeigt.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=139854">MS09-007</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in SChannel kann Spoofing ermöglichen (960225)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im SChannel-Sicherheitspaket (Secure Channel) in Windows. Die Sicherheitsanfälligkeit kann Spoofing ermöglichen, wenn ein Angreifer Zugriff auf das Zertifikat erhält, das vom Endbenutzer zur Authentifizierung verwendet wird. Benutzer sind nur betroffen, wenn die öffentliche Schlüsselkomponente des Zertifikats, das zur Authentifizierung verwendet wird, anderweitig vom Angreifer erhalten wurde.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Spoofing</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=139821">MS09-008</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in DNS- und WINS-Server können Spoofing ermöglichen (962238)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten und zwei öffentlich gemeldete Sicherheitsanfälligkeiten in Windows DNS-Server und Windows WINS-Server. Diese Sicherheitsanfälligkeiten können einem Remoteangreifer ermöglichen, für Internet bestimmten Netzwerkverkehr auf seine eigenen Systeme umzuleiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Spoofing</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID geordnet.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Kennung des Bulletins                                     | Titel des Bulletins                                                                          | CVE-ID                                                                           | Ausnutzbarkeitsindex – Bewertung                                                                                     | Wichtige Hinweise                                                                                                                                                                    |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-006](https://go.microsoft.com/fwlink/?linkid=132503) | Sicherheitsanfälligkeiten im Windows-Kernel können Remotecodeausführung ermöglichen (958690) | [CVE-2009-0081](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0081) | [**3**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Konsistenter Denial-of-Service ist wahrscheinlicher als die zuverlässige Ausführung von funktionalem Code                                                                            |  
| [MS09-006](https://go.microsoft.com/fwlink/?linkid=132503) | Sicherheitsanfälligkeiten im Windows-Kernel können Remotecodeausführung ermöglichen (958690) | [CVE-2009-0082](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0082) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Konsistenter Denial-of-Service ist wahrscheinlicher als die zuverlässige Ausführung von funktionalem Code                                                                            |  
| [MS09-006](https://go.microsoft.com/fwlink/?linkid=132503) | Sicherheitsanfälligkeiten im Windows-Kernel können Remotecodeausführung ermöglichen (958690) | [CVE-2009-0083](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0083) | [**3**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Funktionierender Angreifercode unwahrscheinlich | Lokale Bedrohung existiert nur für konsistenten Denial-of-Service oder Offenlegung von Informationen, was wahrscheinlicher als die zuverlässige Ausführung von funktionalem Code ist |  
| [MS09-007](https://go.microsoft.com/fwlink/?linkid=139854) | Sicherheitsanfälligkeit in SChannel kann Spoofing ermöglichen (960225)                       | [CVE-2009-0085](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0085) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Die Anforderungen für zuverlässige Ausnutzungsmöglichkeiten sind hoch, und die Anzahl maßgeblicher Benutzerszenarien ist gering                                                      |  
| [MS09-008](https://go.microsoft.com/fwlink/?linkid=139821) | Sicherheitsanfälligkeiten in DNS- und WINS-Server können Spoofing ermöglichen (962238)       | [CVE-2009-0093](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0093) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Nach der Machbarkeitsstudie ist konsistentes Spoofing wahrscheinlich, doch funktionaler Angreifercode, der zur Ausführung von schädlichem Code führt, ist sehr unwahrscheinlich      |  
| [MS09-008](https://go.microsoft.com/fwlink/?linkid=139821) | Sicherheitsanfälligkeiten in DNS- und WINS-Server können Spoofing ermöglichen (962238)       | [CVE-2009-0094](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0094) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Nach der Machbarkeitsstudie ist konsistentes Spoofing wahrscheinlich, doch funktionaler Angreifercode, der zur Ausführung von schädlichem Code führt, ist sehr unwahrscheinlich      |  
| [MS09-008](https://go.microsoft.com/fwlink/?linkid=139821) | Sicherheitsanfälligkeiten in DNS- und WINS-Server können Spoofing ermöglichen (962238)       | [CVE-2009-0233](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0233) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Nach der Machbarkeitsstudie ist konsistentes Spoofing wahrscheinlich, doch funktionaler Angreifercode, der zur Ausführung von schädlichem Code führt, ist sehr unwahrscheinlich      |  
| [MS09-008](https://go.microsoft.com/fwlink/?linkid=139821) | Sicherheitsanfälligkeiten in DNS- und WINS-Server können Spoofing ermöglichen (962238)       | [CVE-2009-0234](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0234) | [**2**](https://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich     | Nach der Machbarkeitsstudie ist konsistentes Spoofing wahrscheinlich, doch funktionaler Angreifercode, der zur Ausführung von schädlichem Code führt, ist sehr unwahrscheinlich      |
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Prüfen Sie für jede aufgeführte Kennung der Bulletins die gesamte Spalte, um basierend auf den in Ihrem System installierten Programmen und Komponenten alle Updates zu finden, die Sie installieren müssen.
  
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
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-006**](https://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](https://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](https://go.microsoft.com/fwlink/?linkid=139821)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=98bb7d40-89a0-470a-8eb7-06f15072a635)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bf7065bc-c183-4a78-8d46-72fe7385c07c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[DNS-Server unter Microsoft Windows 2000 Server Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=110354f7-5ece-4c4d-b563-3adba6ac0116)  
(961063)  
(Hoch)  
[WINS-Server unter Microsoft Windows 2000 Server Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4319abb3-1ea2-466a-a815-c0b3b86b4462)  
(961064)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-006**](https://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](https://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](https://go.microsoft.com/fwlink/?linkid=139821)
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
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e09641ba-6cbe-4095-82b5-703d3a7dc33b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=942d87f6-3cb1-4d36-a70a-70d9c34488f3)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d0d704c6-48c2-4907-b6c3-2455d7cf21c8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d02306e-9e2e-4ae8-bd21-8a2c1a229472)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-006**](https://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](https://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](https://go.microsoft.com/fwlink/?linkid=139821)
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
Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f5cfb8da-e7cc-4183-8631-507c2a406500)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0b3f6fdd-276e-4267-99d8-8f00d91ad6a2)  
(Hoch)
</td>
<td style="border:1px solid black;">
[DNS-Server unter Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6cc42c9e-c34e-4577-8b23-9e07e2369878)  
(961063)  
(Hoch)  
[WINS-Server unter Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=049e5db5-7315-4188-99fd-4a54833e6bf2)  
(961064)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ecf75c70-8489-41ad-9759-3a07e13957be)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ce98ff55-f565-469d-bbd2-32b681faf908)  
(Hoch)
</td>
<td style="border:1px solid black;">
[DNS-Server unter Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b1f81fd2-0099-4450-8543-0459561d22d0)  
(961063)  
(Hoch)  
[WINS-Server unter Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4a393c63-eff5-4c8c-9c3f-33ce45c32428)  
(961064)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=04be3d7e-7dda-4dca-887a-e7a8156ede1c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5ca3c72c-cadb-4b0a-b3a3-fb81d0bfd7b3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[DNS-Server unter Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d3ed7d9a-d652-4bd0-aecc-5a415bec6c59)  
(961063)  
(Hoch)  
[WINS-Server unter Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=37e3a75e-0a5d-4df0-881f-cdb87efa4dcf)  
(961064)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-006**](https://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](https://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](https://go.microsoft.com/fwlink/?linkid=139821)
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
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista und Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4b1aaaba-f355-4265-83c0-50b901856ced)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=21086a04-402a-4940-8358-7fa63508102b)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0fcac480-d6db-4a94-8c7d-b7319282cf56)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c75a2ea9-b42f-457b-be09-5c8fa0339388)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-006**](https://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](https://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](https://go.microsoft.com/fwlink/?linkid=139821)
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
Windows Server 2008 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=38851df2-4fb5-4d28-9d15-181c260cf8cf)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=47b361ce-624b-466c-b5c5-8703f6532615)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[DNS-Server unter Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=92e89882-d656-4b61-a05c-3afb44895f08)\*  
(961063)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ec15acc4-3e0f-4414-9383-61c122ff1382)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5c81ac45-60e6-4121-ab6b-d3b3179aacc4)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[DNS-Server unter Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=be068d06-5939-4ad8-8191-e85931ed610f)\*  
(961063)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=eead6f93-10fd-4492-8137-481d9876a5fe)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bf8f5a86-1757-4f9b-b632-d4aa7005a9f8)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008**

**\*Die Server Core-Installation von Windows Server 2008 ist betroffen.** Für unterstützte Editionen von Windows Server 2008 gilt dieses Update mit der gleichen Bewertung des Schweregrads. Dabei spielt es keine Rolle, ob Windows Server 2008 mit der Server Core-Installationsoption installiert wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Security Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch über [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](https://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](https://office.microsoft.com/de-de/downloads/default.aspx) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) und das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](https://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 für Windows 2000 und neuere Betriebssysteme schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](https://technet.microsoft.com/en-us/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection-Tool für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), die im [Anwendungskompatibilitäts-Toolkit 5.0](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Anwendungskompatibilitäts-Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](https://technet.microsoft.com/en-us/wsus/bb466214.aspx).

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Helmut Buhler ([https://home.arcor.de/clipboarder](https://home.arcor.de/clipboarder/)/) für den Hinweis auf ein in MS09-006 beschriebenes Problem.
-   Thomas Garnier von [SkyRecon](https://www.skyrecon.com/) für den Hinweis auf ein in MS09-006 beschriebenes Problem.
-   [Secretaria da Fazenda do Estado do Rio Grande do Sul](https://www.sefaz.rs.gov.br/) für den Hinweis auf ein in MS09-007 beschriebenes Problem.
-   [Cia de Processamento de Dados do Estado do Rio Grande do Sul](https://www.procergs.rs.gov.br/) für den Hinweis auf ein in MS09-007 beschriebenes Problem.
-   Kevin Day für die Zusammenarbeit mit uns an zwei in MS09-008 beschriebenen Problemen.
-   Dave Dagon von [Georgia Tech Information Security Center](https://www.gtisc.gatech.edu/) für die Zusammenarbeit mit uns an zwei in MS09-008 beschriebenen Problemen.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (10. März 2009): Bulletin Summary veröffentlicht.
-   V1.1 (11. März 2009): Aktualisierung der Finderinformationen für MS09-008.

*Built at 2014-04-18T01:50:00Z-07:00*
