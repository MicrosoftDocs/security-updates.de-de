---
TOCTitle: 'MS13-MAR'
Title: Microsoft Security Bulletin Summary für März 2013
ms:assetid: 'ms13-mar'
ms:contentKeyID: 61225122
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms13-mar(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für März 2013
=================================================

Veröffentlicht: Dienstag, 12. März 2013 | Aktualisiert: Freitag, 15. März 2013

**Version:** 1.1

In diesem Bulletin Summary sind die im März 2013 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für März 2013 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 7. März 2013 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, dem 13. März 2013, um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im März](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032538636&culture=en-us). Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032538636&culture=en-us) zur Verfügung.

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=279923">MS13-021</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2809289)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt acht vertraulich gemeldete Sicherheitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=275737">MS13-022</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Silverlight kann Remotecodeausführung ermöglichen (2814124)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Silverlight. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine Website mit einer speziell gestalteten Silverlight-Anwendung hostet, mit der diese Sicherheitsanfälligkeit ausgenutzt werden kann, und dann einen Benutzer zum Anzeigen der Website verleitet. Der Angreifer kann auch beeinträchtigte Websites und Websites nutzen, die von Benutzern bereitgestellte Inhalte oder Anzeigen akzeptieren oder hosten. Solche Websites können speziell gestaltete Inhalte enthalten, mit denen diese Sicherheitsanfälligkeit ausgenutzt werden kann. Ein Angreifer kann Benutzer jedoch nicht zum Besuch einer solchen Website zwingen. Er muss den Benutzer zum Besuch einer Webseite verleiten. Zu diesem Zweck wird der Benutzer normalerweise dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken. Es besteht ebenfalls die Möglichkeit, speziell gestalteten Webinhalt mithilfe von Bannerwerbungen anzuzeigen oder Webinhalt auf andere Weise an betroffene Systeme zu übermitteln.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Kein Neustart erforderlich.</td>
<td style="border:1px solid black;">Microsoft Silverlight</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=276801">MS13-023</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Visio Viewer 2010 kann Remotecodeausführung ermöglichen (2801261)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Visio-Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=271610">MS13-024</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SharePoint können Erhöhung von Berechtigungen ermöglichen (2780176)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft SharePoint und Microsoft SharePoint Foundation. Die schwerwiegendsten dieser Sicherheitsanfälligkeiten können die Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer auf eine speziell gestaltete URL klickt, die den Benutzer zu der betroffenen SharePoint-Website führt.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office, Microsoft Server Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=282355">MS13-025</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft OneNote kann Offenlegung von Informationen ermöglichen (2816264)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft OneNote. Die Sicherheitsanfälligkeit kann die Offenlegung von Informationen ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, eine speziell gestaltete OneNote-Datei zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=280673">MS13-026</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in</strong> <strong>Microsoft Office</strong> <strong>für Mac kann Offenlegung von Information ermöglichen (2813682)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office für Mac. Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer eine speziell gestaltete E-Mail-Nachricht öffnet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Kein Neustart erforderlich.</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=282639">MS13-027</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Kernelmodustreibern können Erhöhung von Berechtigungen ermöglichen (2807986)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Diese Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer Zugang zu einem System erhält.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.
  
| Kennung des Bulletins                                     | Titel der Sicherheitsanfälligkeit                                                       | CVE-ID                                                                           | Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen                                             | Bewertung der Ausnutzbarkeit für ältere Softwareversionen                                               | Bewertung der Ausnutzbarkeit durch Denial-of-Service | Wichtige Hinweise                                                                              |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|------------------------------------------------------|------------------------------------------------------------------------------------------------|  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer OnResize                    | [CVE-2013-0087](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0087) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer saveHistory                 | [CVE-2013-0088](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0088) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CMarkupBehaviorContext      | [CVE-2013-0089](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0089) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CCaret                      | [CVE-2013-0090](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0090) | [2](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wäre schwer zu erstellen | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CElement                    | [CVE-2013-0091](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0091) | Nicht betroffen                                                                                         | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer GetMarkupPtr                | [CVE-2013-0092](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0092) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer onBeforeCopy                | [CVE-2013-0093](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0093) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer removeChild                 | [CVE-2013-0094](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0094) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-021](https://go.microsoft.com/fwlink/?linkid=279923) | Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CTreeNode                   | [CVE-2013-1288](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1288) | Nicht betroffen                                                                                         | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | Diese Sicherheitsanfälligkeit wurde veröffentlicht.                                            |  
| [MS13-022](https://go.microsoft.com/fwlink/?linkid=275737) | Sicherheitsanfälligkeit in Silverlight aufgrund doppelter Dereferenz                    | [CVE-2013-0074](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0074) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                                                                         | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-023](https://go.microsoft.com/fwlink/?linkid=276801) | Sicherheitsanfälligkeit bezüglich Objekttypverwechslung in Visio Viewer Strukturansicht | [CVE-2013-0079](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0079) | Nicht betroffen                                                                                         | [2](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wäre schwer zu erstellen | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-024](https://go.microsoft.com/fwlink/?linkid=271610) | Sicherheitsanfälligkeit in der Rückruffunktion                                          | [CVE-2013-0080](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0080) | Nicht betroffen                                                                                         | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-024](https://go.microsoft.com/fwlink/?linkid=271610) | Sicherheitsanfälligkeit in SharePoint XSS                                               | [CVE-2013-0083](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0083) | Nicht betroffen                                                                                         | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-024](https://go.microsoft.com/fwlink/?linkid=271610) | Sicherheitsanfälligkeit in SharePoint durch Verzeichnisüberquerung                      | [CVE-2013-0084](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0084) | Nicht betroffen                                                                                         | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Nicht anwendbar                                      | (Keine)                                                                                        |  
| [MS13-024](https://go.microsoft.com/fwlink/?linkid=271610) | Sicherheitsanfälligkeit durch Pufferüberlauf                                            | [CVE-2013-0085](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0085) | Nicht betroffen                                                                                         | [3](https://technet.microsoft.com/de-de/security/cc998259) – Angreifercode unwahrscheinlich              | Vorläufig                                            | Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.         |  
| [MS13-025](https://go.microsoft.com/fwlink/?linkid=282355) | Sicherheitsanfälligkeit beim Überprüfen der Puffergröße                                 | [CVE-2013-0086](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0086) | Nicht betroffen                                                                                         | [3](https://technet.microsoft.com/de-de/security/cc998259) – Angreifercode unwahrscheinlich              | Nicht anwendbar                                      | Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht. |  
| [MS13-026](https://go.microsoft.com/fwlink/?linkid=280673) | Sicherheitsanfälligkeit durch unbeabsichtigtes Laden von Inhalten                       | [CVE-2013-0095](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0095) | [3](https://technet.microsoft.com/de-de/security/cc998259) – Angreifercode unwahrscheinlich              | [3](https://technet.microsoft.com/de-de/security/cc998259) – Angreifercode unwahrscheinlich              | Nicht anwendbar                                      | Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht. |  
| [MS13-027](https://go.microsoft.com/fwlink/?linkid=282639) | Sicherheitsanfälligkeit in Windows USB-Beschreibung                                     | [CVE-2013-1285](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1285) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Dauerhaft                                            | (Keine)                                                                                        |  
| [MS13-027](https://go.microsoft.com/fwlink/?linkid=282639) | Sicherheitsanfälligkeit in Windows USB-Beschreibung                                     | [CVE-2013-1286](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1286) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Dauerhaft                                            | (Keine)                                                                                        |  
| [MS13-027](https://go.microsoft.com/fwlink/?linkid=282639) | Sicherheitsanfälligkeit in Windows USB-Beschreibung                                     | [CVE-2013-1287](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1287) | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | [1](https://technet.microsoft.com/de-de/security/cc998259.aspx) – Angreifercode wahrscheinlich           | Dauerhaft                                            | (Keine)                                                                                        |
  
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
<th colspan="3" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=ace6994d-7482-40de-84ad-a87853a35860)  
(2809289)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=50c59794-4ec7-404a-b316-dae314521ebb)  
(2809289)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7e5d96a7-d9f5-4832-b4f9-b6e0148c655b)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=ba528d03-b0a6-40a5-a6bd-13c062a8a877)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=795cef4e-9c01-447f-916c-e52e69eca4a3)  
(2809289)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=16993a2c-1fe1-4c1e-bcd9-db1a7dd4a058)  
(2809289)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=66a08524-883d-4d67-82cc-2c0f55c56b31)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4f8a48d4-b1bb-465c-a232-d29fe94d1429)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=e3c911b3-7fdd-4105-a20a-eef65b0908e3)  
(2809289)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=0f58d63e-0d2c-41d2-9792-edbb2f4a539d)  
(2809289)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e6b63da9-a414-40ee-b877-4fb0d62bacba)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=835651b7-79fb-4d50-b48e-f02173062253)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=eaf2c568-089a-4c2f-bca6-da83f7332de9)  
(2809289)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=5a18b139-2773-44c8-85f9-8dce24249e71)  
(2809289)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d6feba92-f014-4521-b6c4-7f5f358a3ce3)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9d5f1ed1-f33b-4c90-9b29-ee8ac587d31b)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=088fd3ec-62e1-4737-8132-6b51219ed37f)  
(2809289)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=799748d8-056d-4139-86e1-9bd0cb0151b4)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=28d441e7-abcf-4cc9-84e0-572e5b79aab7)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=0bf77905-1199-4219-a67d-1e9ad3f63757)  
(2809289)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=76e328f8-4f86-4e50-b7e0-22db0385ab01)  
(2809289)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c26f74fc-e224-4533-a4e3-b52125dca5cd)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b8472bc7-9e20-4238-adcf-a1e1a91687a1)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=7b652bb4-7a0a-437b-bcc5-ebbbb820c559)  
(2809289)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=67b09398-ceb6-403c-bba4-261d9d9dea98)  
(2809289)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=3f1795a5-4376-4929-8748-743840ec2154)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e412c54a-a93d-4c5b-9b13-40b59d1dff35)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=0303fcb1-34d5-47da-b6ee-18222fe3235a)  
(2809289)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=337068a5-9281-4db6-9ff1-5282cdfa0763)  
(2809289)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c672c196-5072-468c-8d88-34534fa219fd)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f1ca4fe0-3ee3-4162-a9fa-48c54fc8b08e)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=f22b9327-1430-44cb-a609-ea1bb9b7b8f8)  
(2809289)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=0496cbfe-77d2-4de6-b78d-937225dc8974)  
(2809289)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=5c40f237-b4c8-41eb-a649-baad46dfa13c)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8b61f3e5-0cf9-4eab-8a59-829957135dd6)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=09e4832c-b95e-4581-a73b-49cb6a60c1df)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=af2e8e83-fb8f-4ba5-83ec-8bd4347a5fe6)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=b07b63d5-925d-4c4f-ae19-18a9b141eaa0)  
(2809289)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=54c619b7-e156-4f07-a90e-56ed9a618085)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=c72f78be-e6a8-43b4-9303-7c93dd11d502)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=b07b63d5-925d-4c4f-ae19-18a9b141eaa0)  
(2809289)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=54c619b7-e156-4f07-a90e-56ed9a618085)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c72f78be-e6a8-43b4-9303-7c93dd11d502)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=610da6c6-e8a9-4726-ae54-11f01fb5ab2d)  
(2809289)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=86f2a369-d71d-4a36-95ed-d5be89cbbbae)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=6a8a22d6-0e6e-4d3b-afd0-d4841274ade0)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=610da6c6-e8a9-4726-ae54-11f01fb5ab2d)  
(2809289)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=86f2a369-d71d-4a36-95ed-d5be89cbbbae)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6a8a22d6-0e6e-4d3b-afd0-d4841274ade0)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=cf5f65e1-93ae-4ec3-84d2-eb017efdc9d6)  
(2809289)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c5018865-7162-4d8d-86fc-aacd6d5f0a37)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=84ba3686-14ed-4aac-8db1-4438aa9e0a2e)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=cf5f65e1-93ae-4ec3-84d2-eb017efdc9d6)  
(2809289)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c5018865-7162-4d8d-86fc-aacd6d5f0a37)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=84ba3686-14ed-4aac-8db1-4438aa9e0a2e)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=3436d1d1-bf20-40cc-8c51-f093da67c8a9)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=01498cd0-e27e-4256-8f21-7a6eeedfb77c)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=3436d1d1-bf20-40cc-8c51-f093da67c8a9)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=01498cd0-e27e-4256-8f21-7a6eeedfb77c)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows 8
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=7c348fe3-f4f0-4f22-8a7f-8563705c1f64)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=de4ec125-c337-4615-b39b-8456658dae22)  
(2807986)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=0c503b83-5b13-41da-a5ff-7519bc244521)  
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=c1539e94-0635-4f51-8172-a96a737d81d3)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2012
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=f9b299f1-8a73-40b2-9942-e6419496bb39)  
(2809289)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=959c78e1-29d9-40a3-9eb3-1206c09e3752)  
(2807986)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows RT
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
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
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10<sup>[1]</sup>
(2809289)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Server Core-Installationsoption
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-021**](https://go.microsoft.com/fwlink/?linkid=279923)
</td>
<td style="border:1px solid black;">
[**MS13-027**](https://go.microsoft.com/fwlink/?linkid=282639)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f1ca4fe0-3ee3-4162-a9fa-48c54fc8b08e) (Server Core-Installation)  
(2807986)  
(Hoch)
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
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8b61f3e5-0cf9-4eab-8a59-829957135dd6) (Server Core-Installation)  
(2807986)  
(Hoch)
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
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=84ba3686-14ed-4aac-8db1-4438aa9e0a2e) (Server Core-Installation)  
(2807986)  
(Hoch)
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
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=84ba3686-14ed-4aac-8db1-4438aa9e0a2e) (Server Core-Installation)  
(2807986)  
(Hoch)
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
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=959c78e1-29d9-40a3-9eb3-1206c09e3752) (Server Core-Installation)  
(2807986)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-021**

<sup>[1]</sup>Sicherheitsupdates für Windows RT werden über [Windows Update](https://update.microsoft.com/windowsupdate/) bereitgestellt.

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="4" style="border:1px solid black;">
Microsoft Office Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-023**](https://go.microsoft.com/fwlink/?linkid=276801)
</td>
<td style="border:1px solid black;">
[**MS13-025**](https://go.microsoft.com/fwlink/?linkid=282355)
</td>
<td style="border:1px solid black;">
[**MS13-026**](https://go.microsoft.com/fwlink/?linkid=280673)
</td>
</tr>
<tr class="alternateRow">
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 Service Pack 1 (32-Bit-Edition)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 Service Pack 1 (32-Bit-Edition)](https://www.microsoft.com/download/details.aspx?familyid=b01b4410-1107-472f-bf96-234304e91e77)  
(2687505)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 Service Pack 1 (64-Bit-Edition)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 Service Pack 1 (64-Bit-Edition)](https://www.microsoft.com/download/details.aspx?familyid=24065dd5-251b-4a3c-bb44-8d552a1f265e)  
(2687505)  
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
Microsoft Visio 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2010 Service Pack 1 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=7a1a21e7-3137-4201-a005-cc66379fc1c5)  
(2760762)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio 2010 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2010 Service Pack 1 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=7b7d39f0-a341-4d48-8177-329cccb5a7f1)  
(2760762)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
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
Microsoft Office 2010 Filter Pack Service Pack 1 (32-Bit-Version)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Filter Pack Service Pack 1 (32-Bit-Version)](https://www.microsoft.com/download/details.aspx?familyid=f10db48f-a980-47bf-83a5-c0da4e615114)  
(2553501)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 Filter Pack Service Pack 1 (64-Bit-Version)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Filter Pack Service Pack 1 (64-Bit-Version)](https://www.microsoft.com/download/details.aspx?familyid=70d3372b-74a8-4b68-b6c4-18863835915d)  
(2553501)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
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
Microsoft OneNote 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft OneNote 2010 Service Pack 1 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=da4bfd31-65b9-496b-aa98-4fa8b729dcf3)  
(2760600)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft OneNote 2010 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft OneNote 2010 Service Pack 1 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=10fc7350-e1d4-40b6-a5d1-8670263faf05)  
(2760600)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=d7aef20a-922b-4495-b473-1afa4a7ac514)  
(2817449)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office für Mac 2011](https://www.microsoft.com/download/details.aspx?familyid=4960674b-1cb4-499a-999e-7aa4d4c49e5e)  
(2817452)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-023**

<sup>[1]</sup>In diesem Update gibt es für die angegebene Software keine Bewertung des Schweregrads, da die bekannten Angriffsmethoden für die Sicherheitsanfälligkeit blockiert sind.

#### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-022**](https://go.microsoft.com/fwlink/?linkid=275737)
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
Microsoft Silverlight 5 bei Installation auf dem Mac
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 5](https://www.microsoft.com/download/details.aspx?familyid=75eef049-1f39-47b4-9a1e-839974fc89b9) bei Installation auf dem Mac  
(2814124)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 5 Developer Runtime bei Installation auf dem Mac
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 5 Developer Runtime](https://www.microsoft.com/download/details.aspx?familyid=75eef049-1f39-47b4-9a1e-839974fc89b9) bei Installation auf dem Mac  
(2814124)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 5](https://www.microsoft.com/download/details.aspx?familyid=75eef049-1f39-47b4-9a1e-839974fc89b9) bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(2814124)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 5 Developer Runtime](https://www.microsoft.com/download/details.aspx?familyid=75eef049-1f39-47b4-9a1e-839974fc89b9) bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(2814124)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 5 bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 5](https://www.microsoft.com/download/details.aspx?familyid=75eef049-1f39-47b4-9a1e-839974fc89b9) bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(2814124)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 5 Developer Runtime bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 5 Developer Runtime](https://www.microsoft.com/download/details.aspx?familyid=75eef049-1f39-47b4-9a1e-839974fc89b9) bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern  
(2814124)  
(Kritisch)
</td>
</tr>
</table>
 

#### Microsoft Server Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-024**](https://go.microsoft.com/fwlink/?linkid=271610)
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
Microsoft SharePoint Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Server 2010 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=a9e8acbd-90e5-4acd-aa8f-b743a352787b)<sup>[1]</sup>
(wasrv)  
(2553407)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Foundation
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-024**](https://go.microsoft.com/fwlink/?linkid=271610)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Foundation 2010 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=293666ec-3290-4c6f-a7f6-b44c9b7fa0a6)  
(2687418)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-024**

<sup>[1]</sup>Bei unterstützten Editionen von Microsoft SharePoint Server 2010 müssen Endbenutzer zusätzlich zu dem Sicherheitsupdatepaket für Microsoft SharePoint 2010 (2553407) auch das Sicherheitsupdate für Microsoft SharePoint Foundation 2010 (2687418) installieren, um vor den Sicherheitsanfälligkeiten geschützt zu sein, die in diesem Bulletin beschrieben sind.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/bb245732). Im [TechNet Sicherheitscenter](https://technet.microsoft.com/de-de/security/default.aspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Endbenutzer können das [Microsoft-Sicherheitscenter](https://www.microsoft.com/de-de/security/default.aspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. und können am einfachsten durch eine Suche nach dem Begriff „Sicherheitsupdate“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS13-001“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

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

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://technet.microsoft.com/en-us/library/cc917507.aspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/de-de/download/details.aspx?id=1846) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc749197), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

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

**MS13-021**

-   Arseniy Akuney von [TELUS Security Labs](https://telussecuritylabs.com/) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer OnResize (CVE-2013-0087).
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer saveHistory (CVE-2013-0088).
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CMarkupBehaviorContext (CVE-2013-0089).
-   Stephen Fewer von [Harmony Security](https://www.harmonysecurity.com) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CCaret (CVE-2013-0090).
-   SkyLined in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CCaret (CVE-2013-0090).
-   Jose A. Vazquez von Yenteasy – Security Research in Zusammenarbeit mit [Exodus Intelligence](https://www.exodusintel.com/) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CElement (CVE-2013-0091).
-   [Aniway.Aniway@gmail.com](mailto:aniway.aniway@gmail.com) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer GetMarkupPtr (CVE-2013-0092).
-   [Aniway.Aniway@gmail.com](mailto:aniway.aniway@gmail.com) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer onBeforeCopy (CVE-2013-0093).
-   Simon Zuckerbraun in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer removeChild (CVE-2013-0094).
-   Gen Chen von [Venustech](https://www.venustech.com.cn/) ADLab für die Zusammenarbeit mit uns an der Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CTreeNode (CVE-2013-1288).
-   [Qihoo 360 Security Center](https://www.360.cn/) für die Zusammenarbeit mit uns an der Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CTreeNode (CVE-2013-1288).

**MS13-022**

-   James Forshaw von [Context Information Security](https://www.contextis.com/) für den Hinweis auf die Sicherheitsanfälligkeit aufgrund doppelter Dereferenz (CVE-2013-0074).

**MS13-023**

-   [Aniway.Anyway@gmail.com](mailto:aniway.anyway@gmail.com) in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Objekttypverwechslung in Visio Viewer Strukturansicht (CVE-2013-0079).

**MS13-024**

-   Emanuel Bronshtein von [BugSec](https://www.bugsec.com/) für den Hinweis auf die Sicherheitsanfälligkeit in der Rückruffunktion (CVE-2013-0080).
-   Sunil Yadav von INR Labs ([Network Intelligence India](https://niiconsulting.com/)) für den Hinweis auf die Sicherheitsanfälligkeit in SharePoint durch siteübergreifende Skripterstellung (CVE-2013-0083).
-   Moritz Jodeit von [n.runs AG](https://www.nruns.com/) für den Hinweis auf die Sicherheitsanfälligkeit in SharePoint durch Verzeichnisüberquerung (CVE-2013-0084).

**MS13-025**

-   Christopher Gabriel von der für den Hinweis auf die Sicherheitsanfälligkeit beim Überprüfen der Puffergröße (CVE-2013-0086).

**MS13-026**

-   [Nick Semenkovich](https://technet.microsoft.com/de-DE/mailto:semenko@alum.mit.edu) für den Hinweis auf die Sicherheitsanfälligkeit durch unbeabsichtigtes Laden von Inhalten (CVE- 2013-0095).

**MS13-027**

-   Andy Davis von der NCC Group für den Hinweis auf die Sicherheitsanfälligkeit in Windows USB-Beschreibung (CVE-2013-1285).
-   Andy Davis von der NCC Group für den Hinweis auf die Sicherheitsanfälligkeit in Windows USB-Beschreibung (CVE-2013-1286).
-   Andy Davis von der NCC Group für den Hinweis auf die Sicherheitsanfälligkeit in Windows USB-Beschreibung (CVE-2013-1287).

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617.aspx)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (12. März 2013): Bulletin Summary veröffentlicht.
-   V1.1 (15. März 2013) Für MS13-026 wurde der Titel des Bulletins im Abschnitt **Kurzzusammenfassungen** korrigiert.

*Built at 2014-04-18T01:50:00Z-07:00*
