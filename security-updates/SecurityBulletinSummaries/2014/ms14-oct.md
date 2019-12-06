---
TOCTitle: 'MS14-OKT'
Title: Microsoft Security Bulletin Summary für Oktober 2014
ms:assetid: 'ms14-oct'
ms:contentKeyID: 63172045
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms14-oct(v=Security.10)'
---

Microsoft Security Bulletin Summary für Oktober 2014
====================================================

Veröffentlicht: 14. Oktober 2014

**Version:** 1.0

In diesem Bulletin Summary sind die im Oktober 2014 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Oktober 2014 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 9. Oktober 2014 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, den 15. Oktober 2014 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. Informationen zum Anzeigen des monatlichen Webcasts und Links zu zusätzlichen Security Bulletin-Webcasts finden Sie unter [Microsoft Security Bulletin-Webcast](https://technet.microsoft.com/security/dn756352).

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2987107)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vierzehn vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513095">MS14-057</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in .NET Framework können Remotecodeausführung ermöglichen (3000414))<br />
<br />
</strong>Dieses Sicherheitsupdate behebt drei vertrauliche gemeldete Sicherheitsanfälligkeiten in Microsoft .NET Framework. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete URI-Anforderung mit internationalen Zeichen an eine .NET-Webanwendung sendet. In .NET 4.0-Anwendungen ist die anfällige Funktion (iriParsing) standardmäßig deaktiviert. Damit die Sicherheitsanfälligkeit ausgenutzt werden kann, muss diese Funktion ausdrücklich von einer Anwendung aktiviert werden. In .NET 4.5-Anwendungen ist iriParsing standardmäßig aktiviert und kann nicht deaktiviert werden.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513104">MS14-058</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Kernelmodustreiber kann Remotecodeausführung ermöglichen (3000061)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendere Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, ein speziell gestaltetes Dokument zu öffnen oder eine nicht vertrauenswürdige Website zu besuchen, die integrierte TrueType-Schriftarten enthält. Ein Angreifer kann Endbenutzer jedoch nicht zum Ausführen solcher Aktionen zwingen. Stattdessen muss ein Angreifer einen Benutzer dazu verleiten. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zu klicken.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=507673">MS14-059</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in ASP .NET MVC kann Umgehung der Sicherheitsfunktion ermöglichen (2990942)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in ASP.NET MVC. Die Sicherheitsanfälligkeit kann eine Umgehung der Sicherheitsfunktion ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, auf einen speziell gestalteten Link zu klicken oder eine Webseite zu besuchen, die speziell gestaltete Inhalte enthält, mit denen die Sicherheitsanfälligkeit ausgenutzt werden soll. In einem webbasierten Angriffsszenario kann ein Angreifer eine speziell gestaltete Website hosten, um diese Sicherheitsanfälligkeit durch einen Webbrowser auszunutzen, und dann einen Benutzer zum Besuch der Website verleiten. Der Angreifer kann auch beeinträchtigte Websites und Websites nutzen, die von Benutzern bereitgestellte Inhalte oder Anzeigen akzeptieren oder hosten. Diese Websites können speziell gestaltete Inhalte enthalten, mit denen die Sicherheitsanfälligkeit ausgenutzt werden kann. Ein Angreifer kann Benutzer jedoch nicht zwingen, die vom Angreifer kontrollierten Inhalte anzuzeigen. Stattdessen muss ein Angreifer Benutzer zu Handlungen verleiten. Zu diesem Zweck werden Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder einer Instant Messenger-Nachricht zu klicken, wodurch die Benutzer zur Website des Angreifers gelangen, oder eine Dateianlage zu öffnen, die per E-Mail gesendet wurde.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft-Entwicklertools</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513097">MS14-060</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows OLE kann Remotecodeausführung ermöglichen (3000869)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Microsoft Office-Datei öffnet, die ein speziell gestaltetes OLE-Objekt enthält. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Wenn der aktuelle Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer Programme installieren; Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für jene, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513106">MS14-061</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Word und Office Web Apps können Remotecodeausführung ermöglichen (3000434)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, eine speziell gestaltete Microsoft Word-Datei zu öffnen. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Wenn der aktuelle Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer Programme installieren; Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für jene, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Office-Dienste<br />
Microsoft Office Web Apps</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513107">MS14-062</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Message Queuing-Dienst kann Erhöhung von Berechtigungen ermöglichen 2993254)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer eine speziell gestaltete IOCTL-Anforderung (Input/Output Control; Eingabe/Ausgabe-Steuerung) an den Message Queuing-Dienst sendet. Eine erfolgreiche Ausnutzung dieser Sicherheitsanfälligkeit kann vollständigen Zugriff auf das betroffene System ermöglichen. Standardmäßig wird die Komponente Message Queuing nicht unter betroffenen Betriebssystemversionen installiert und kann nur von einem Benutzer mit Administratorberechtigungen aktiviert werden. Nur Kunden, die die Message Queuing-Komponente manuell aktivieren, können für dieses Problem anfällig sein.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513102">MS14-063</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in FAT32-Festplattenpartitionstreiber kann Erhöhung von Berechtigungen ermöglichen (2998579)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Es liegt eine Sicherheitsanfälligkeit bezüglich der Erhöhung von Berechtigungen vor, die dadurch verursacht wird, wie Windows FASTFAT mit FAT32-Partitionen der Festplatte interagiert. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code mit erhöhten Berechtigungen ausführen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a> <br />
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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4123">CVE-2014-4123</a></td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit bezüglich der Erhöhung von Berechtigungen durch Umgehung der IE-Sandbox.<br />
<br />
Microsoft ist sich begrenzter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4124">CVE-2014-4124</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für eine lokale Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4126">CVE-2014-4126</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4127">CVE-2014-4127</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4128">CVE-2014-4128</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4129">CVE-2014-4129</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4130">CVE-2014-4130</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4132">CVE-2014-4132</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4133">CVE-2014-4133</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4134">CVE-2014-4134</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4137">CVE-2014-4137</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4138">CVE-2014-4138</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Umgehung der Internet Explorer ASLR</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4140">CVE-2014-4140</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit aufgrund der Umgehung von Sicherheitsfunktionen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513092">MS14-056</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4141">CVE-2014-4141</a></td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513095">MS14-057</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET ClickOnce bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4073">CVE-2014-4073</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für eine lokale Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513095">MS14-057</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET Framework bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4121">CVE-2014-4121</a></td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513095">MS14-057</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET ASLR</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4122">CVE-2014-4122</a></td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit aufgrund der Umgehung von Sicherheitsfunktionen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513104">MS14-058</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k.sys bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4113">CVE-2014-4113</a></td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für eine lokale Erhöhung von Berechtigungen ausgenutzt werden.<br />
<br />
Microsoft ist sich begrenzter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513104">MS14-058</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung bei Analyse von True Type-Schriftarten</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4148">CVE-2014 -4148</a></td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Microsoft ist sich begrenzter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=507673">MS14-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MVC durch siteübergreifende Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4075">CVE-2014-4075</a></td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">3 - Ausnutzung unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit aufgrund der Umgehung von Sicherheitsfunktionen.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513097">MS14-060</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows OLE bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4114">CVE-2014-4114</a></td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">0 - Ausnutzung erkannt</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Microsoft ist sich begrenzter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513106">MS14-061</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Microsoft Word-Dateiformat </td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4117">CVE-2014-4117</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513107">MS14-062</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MQAC bezüglich Erhöhung von Berechtigungen durch beliebiges Schreiben</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4971">CVE-2014-4971</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">1 - Ausnutzung wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für eine lokale Erhöhung von Berechtigungen ausgenutzt werden.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=513102">MS14-063</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Windows-Festplattenpartitionstreiber bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4115">CVE-2014-4115</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">2 - Ausnutzung weniger wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für eine lokale Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
</tbody>
</table>
  
 
  
Betroffene Software  
-------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.
  
**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
**Keine**
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(2987107)  
(Mittel)  
Internet Explorer 7  
(2987107)  
(Mittel)  
Internet Explorer 8  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2972105)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979574)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2993254)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(2987107)  
(Mittel)  
Internet Explorer 7  
(2987107)  
(Mittel)  
Internet Explorer 8  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2972105)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979574)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2993254)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(2987107)  
(Mittel)  
Internet Explorer 7  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2972105)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979574)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2993254)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2998579)  
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
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
(2987107)  
(Kritisch)  
Internet Explorer 8  
(2987107)  
(Kritisch)  
Internet Explorer 9  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2968292)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2972098)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979568)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2987107)  
(Kritisch)  
Internet Explorer 8  
(2987107)  
(Kritisch)  
Internet Explorer 9  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2968292)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2972098)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979568)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
(2987107)  
(Mittel)  
Internet Explorer 8  
(2987107)  
(Mittel)  
Internet Explorer 9  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2968292)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2972098)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979568)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2987107)  
(Mittel)  
Internet Explorer 8  
(2987107)  
(Mittel)  
Internet Explorer 9  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2968292)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2972098)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979568)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2968292)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2972098)  
(Kritisch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2979568)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2987107)  
(Kritisch)  
Internet Explorer 9  
(2987107)  
(Kritisch)  
Internet Explorer 10  
(2987107)  
(Kritisch)  
Internet Explorer 11  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2968294)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2972100)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(2979570)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2987107)  
(Kritisch)  
Internet Explorer 9  
(2987107)  
(Kritisch)  
Internet Explorer 10  
(2987107)  
(Kritisch)  
Internet Explorer 11  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2968294)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2972100)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(2979570)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2987107)  
(Mittel)  
Internet Explorer 9  
(2987107)  
(Mittel)  
Internet Explorer 10  
(2987107)  
(Mittel)  
Internet Explorer 11  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2968294)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2972100)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(2979570)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2968294)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2972100)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(2979570)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="7">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968295)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972101)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979571)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978042)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979577)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968295)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972101)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979571)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978042)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979577)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968296)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972103)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979573)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978041)  
(Kritisch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2979576)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968296)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972103)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979573)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978041)  
(Kritisch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2979576)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
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
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968295)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972101)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979571)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978042)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979577)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(2987107)  
(Mittel)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968296)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972103)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979573)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978041)  
(Kritisch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2979576)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
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
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978042)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979577)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(2987107)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.1/4.5.2  
(2978041)  
(Kritisch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2979576)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3000869)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
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
[**MS14-056**](https://go.microsoft.com/fwlink/?linkid=513092)
</td>
<td style="border:1px solid black;">
[**MS14-057**](https://go.microsoft.com/fwlink/?linkid=513095)
</td>
<td style="border:1px solid black;">
[**MS14-058**](https://go.microsoft.com/fwlink/?linkid=513104)
</td>
<td style="border:1px solid black;">
[**MS14-060**](https://go.microsoft.com/fwlink/?linkid=513097)
</td>
<td style="border:1px solid black;">
[**MS14-062**](https://go.microsoft.com/fwlink/?linkid=513107)
</td>
<td style="border:1px solid black;">
[**MS14-063**](https://go.microsoft.com/fwlink/?linkid=513102)
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
**Keine**
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(2998579)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2968294)  
(Hoch)  
Microsoft .NET Framework 3.5.1  
(2972100)  
(Kritisch)  
Microsoft .NET Framework 3.5.1  
(2979570)  
(Hoch)  
Microsoft .NET Framework 4  
(2972106)  
(Kritisch)  
Microsoft .NET Framework 4  
(2979575)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2972107)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979578)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968295)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972101)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979571)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978042)  
(Kritisch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2979577)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2968296)  
(Hoch)  
Microsoft .NET Framework 3.5  
(2972103)  
(Kritisch)  
Microsoft .NET Framework 3.5  
(2979573)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978041)  
(Kritisch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2979576)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3000061)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
</table>
 
 

### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**ASP.NET MVC**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-059**](https://go.microsoft.com/fwlink/?linkid=507673)
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
ASP.NET MVC 2.0
</td>
<td style="border:1px solid black;">
ASP.NET MVC 2.0  
(2993939)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
ASP.NET MVC 3.0
</td>
<td style="border:1px solid black;">
ASP.NET MVC 3.0  
(2993937)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
ASP.NET MVC 4.0
</td>
<td style="border:1px solid black;">
ASP.NET MVC 4.0  
(2993928)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
ASP.NET MVC 5.0
</td>
<td style="border:1px solid black;">
ASP.NET MVC 5.0  
(2992080)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
ASP.NET MVC 5.1
</td>
<td style="border:1px solid black;">
ASP.NET MVC 5.1  
(2994397)  
(Hoch)
</td>
</tr>
</table>
 
 

### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-061**](https://go.microsoft.com/fwlink/?linkid=513106)
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
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(2883031)  
(Hoch)  
Microsoft Word 2007 Service Pack 3  
(2883032)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office 2010**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-061**](https://go.microsoft.com/fwlink/?linkid=513106)
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
Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)  
(2883008)  
(Hoch)  
Microsoft Word 2010 Service Pack 1 (32-Bit-Editionen)  
(2883013)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)  
(2883008)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(2883013)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (64-Bit-Editionen)  
(2883008)  
(Hoch)  
Microsoft Word 2010 Service Pack 1 (64-Bit-Editionen)  
(2883013)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)  
(2883008)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(2883013)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Microsoft Office für Mac**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-061**](https://go.microsoft.com/fwlink/?linkid=513106)
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
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011  
(3004865)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="2">
**Weitere Office-Software**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-061**](https://go.microsoft.com/fwlink/?linkid=513106)
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
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2883031)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS14-061**

Diese Bulletins umfassen mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

### Microsoft Office-Dienste und Web Apps

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
[**MS14-061**](https://go.microsoft.com/fwlink/?linkid=513106)
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
Microsoft SharePoint Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Word-Automatisierungsdienste  
(2883098)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Word-Automatisierungsdienste  
(2883098)  
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
[**MS14-061**](https://go.microsoft.com/fwlink/?linkid=513106)
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
Microsoft Office Web Apps 2010
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2010  
(2889827)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2010 Service Pack 1  
(2889827)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2010 Service Pack 2  
(2889827)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS14-061**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt.

 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter.

Windows-Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager helfen Administratoren beim Verteilen von Sicherheitsupdates.

Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](https://technet.microsoft.com/de-de/security/cc297183). 

Danksagungen
------------

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

**MS14-056**

-   James Forshaw von [Context Information Security](https://www.contextis.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen (CVE-2014-4123).
-   James Forshaw von [Context Information Security](https://www.contextis.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen (CVE-2014-4124).
-   Rohit Mothe in Zusammenarbeit mit den [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4126).
-   Bo Qu von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4127).
-   Omair in Zusammenarbeit mit den [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4128).
-   Jason Kratzer für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4128).
-   [Adlab von Venustech](https://www.venustech.com.cn/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4129).
-   Sky in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4130).
-   Zhibin Hu von [Qihoo 360](https://www.360.cn/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4132).
-   José A. Vázquez von Yenteasy – Security Research in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4132).
-   Zhibin Hu von [Qihoo 360](https://www.360.cn/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4133).
-   Zhibin Hu von [Qihoo 360](https://www.360.cn/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4134).
-   Liu Long von [Qihoo 360](https://www.360.cn/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4137).
-   SkyLined in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4138).
-   John Villamil (@day6reak) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4140).
-   Peter ‘corelanc0d3 r‘ Van Eeckhoutte von [Corelan](https://www.corelangcv.com/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2014-4141).

**MS14-057**

-   James Forshaw von [Context Information Security](https://www.contextis.com/) für den Hinweis auf die Sicherheitsanfälligkeit in .NET ClickOnce bezüglich der Erhöhung von Berechtigungen (CVE-2014-4073).

**MS14-058**

-   [CrowdStrike Intelligence Team](https://www.crowdstrike.com/) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in Win32k.sys bezüglich der Erhöhung von Berechtigungen (CVE-2014-4113).
-   [FireEye, Inc.](https://www.fireeye.com/) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in Win32k.sys bezüglich der Erhöhung von Berechtigungen (CVE-2014-4113).
-   [FireEye, Inc.](https://www.fireeye.com/) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in TrueType.sys bezüglich der Erhöhung von Berechtigungen (CVE-2014-4148).

**MS14-060**

-   [iSIGHT Partners](https://www.isightpartners.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Windows OLE bezüglich Remotecodeausführung (CVE-2014-4114).

**MS14-061**

-   3S Labs in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit im Microsoft Word-Dateiformat (CVE-2014-4117).

**MS14-063**

-   Marcin 'Icewall' Noga von [Cisco Talos](https://www.sourcefire.com/solutions/research) für den Hinweis auf die Sicherheitsanfälligkeit in Windows-Festplattenpartitionstreiber bezüglich Erhöhung von Berechtigungen (CVE-2014-4115).

Weitere Informationen:
----------------------

### Windows-Tool zum Entfernen schädlicher Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

### Support

Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.

Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)

So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)

Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (14. Oktober 2014): Bulletin Summary veröffentlicht.

*Seite generiert am 13.10.2014 um 14:39Z-07:00.*
