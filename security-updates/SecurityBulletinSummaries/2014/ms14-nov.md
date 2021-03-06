---
TOCTitle: 'MS14-NOV'
Title: Microsoft Security Bulletin Summary für November 2014
ms:assetid: 'ms14-nov'
ms:contentKeyID: 63355193
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms14-nov(v=Security.10)'
---

Microsoft Security Bulletin Summary für November 2014
=====================================================

Veröffentlicht: 11. November 2014 | Aktualisiert: 18. Dezember 2014

**Version:** 2.1

In diesem Bulletin Summary sind die im November 2014 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für November 2014 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 6. November 2014 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://technet.microsoft.com/de-de/security/gg309152.aspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-064">MS14-064</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows OLE kann Remotecodeausführung ermöglichen (3011443)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows OLE (Object Linking and Embedding). Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code im Kontext des aktuellen Benutzers ausführen. Wenn der aktuelle Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer Programme installieren; Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für jene, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch </a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-065">MS14-065</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (3003057)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt siebzehn vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch </a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-066">MS14-066</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in SChannel kann Remotecodeausführung ermöglichen (2992611)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft Secure Channel (Schannel)-Sicherheitspaket in Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine Reihe speziell gestalteter Pakete an einen betroffenen Windows-Server sendet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch </a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-067">MS14-067</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in XML Core Services kann Remotecodeausführung ermöglichen (2993958)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Remotecodeausführung ermöglichen, wenn ein angemeldeter Benutzer eine speziell gestaltete Website besucht, die dafür ausgelegt ist, Microsoft XML Core Services (MSXML) über Internet Explorer aufzurufen. Ein Angreifer kann Endbenutzer jedoch nicht zum Besuch solcher Websites zwingen. Er muss den Benutzer zu einem Besuch einer Webseite verleiten. Zu diesem Zweck wird der Benutzer normalerweise dazu gebracht, in einer E-Mail oder einer Instant Messenger-Anfrage auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch </a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-068">MS14-068</a></td>
<td style="border:1px solid black;"><strong>Sicherheitslücke in Kerberos kann Erhöhung von Berechtigungen ermöglichen (3011780)<br />
</strong><br />
Dieses Sicherheitsupdate dient zum Schließen einer privat gemeldeten Sicherheitslücke im Microsoft Windows Kerberos-Schlüsselverteilungscenter (KDC), über die ein Angreifer die Berechtigungen eines Domänenbenutzerkontos ohne Berechtigungen in die des Domänenadministratorkontos hochstufen kann. Ein Angreifer kann mit diesen erhöhten Berechtigungen beliebige Computer in der Domäne, einschließlich Domänencontrollern, gefährden. Ein Angreifer muss über gültige Anmeldeinformationen verfügen, um diese Sicherheitslücke ausnutzen zu können. Die betroffene Komponente ist für Benutzer mit standardmäßigen Benutzerkonten mit Anmeldeinformationen für die Domäne remote verfügbar. Dies ist nicht der Fall für Benutzer mit ausschließlich Anmeldeinformationen für das lokale Konto. Als dieses Security Bulletin veröffentlicht wurde, war sich Microsoft begrenzter, gezielter Angriffe bewusst, bei denen versucht wird, diese Sicherheitslücke auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch </a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-069">MS14-069</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (3009710)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Diese Sicherheitsanfälligkeiten können die Codeausführung von Remotestandorten aus ermöglichen, wenn eine speziell gestaltete Datei in einer betroffenen Version von Microsoft Office 2007 geöffnet wird. Wenn ein Angreifer diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann er die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-070">MS14-070</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in TCP/IP kann Erhöhung von Berechtigungen ermöglichen (2989935)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in TCP/IP, die während der Verarbeitung der Eingabe/Ausgabe-Steuerung (IOCTL) auftritt. Diese Sicherheitsanfälligkeit kann Rechteerweiterungen ermöglichen, wenn sich ein Angreifer bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code im Kontext eines anderen Prozesses ausführen. Wenn dieser Prozess mit Administratorrechten ausgeführt wird, kann ein Angreifer Programme installieren; Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-071">MS14-071</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows-Audiodienst kann Rechteerweiterungen ermöglichen (3005607)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Rechteerweiterungen ermöglichen, wenn eine Anwendung den Microsoft Windows-Audiodienst verwendet. Für sich genommen ermöglicht diese Sicherheitsanfälligkeit nicht das Ausführen beliebigen Codes. Diese Sicherheitsanfälligkeit muss in Verbindung mit einer anderen Sicherheitsanfälligkeit ausgenutzt werden, die wiederum Remotecodeausführung ermöglicht.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-072">MS14-072</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework kann Erhöhung von Berechtigungen ermöglichen (3005210)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft .NET Framework. Die Sicherheitsanfälligkeit kann Rechteerweiterungen ermöglichen, wenn ein authentifizierter Angreifer speziell gestaltete Daten an eine betroffene Arbeitsstation oder einen Server sendet, die bzw. der .NET Remoting verwendet. Nur benutzerdefinierte Anwendungen, die speziell für die Verwendung von .NET Remoting entwickelt wurden, können ein System anfällig für diese Sicherheitsanfälligkeit machen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-073">MS14-073</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft SharePoint Foundation kann Erhöhung von Berechtigungen ermöglichen (3000431)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft SharePoint Server. Ein authentifizierter Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code im Kontext des Benutzers auf der aktuellen SharePoint-Website ausführen. In einem webbasierten Angriffsszenario kann ein Angreifer eine speziell gestaltete Website hosten, mit der diese Sicherheitsanfälligkeiten ausgenutzt werden sollen, und dann einen Benutzer zum Besuch der Website verleiten. Der Angreifer kann auch beeinträchtigte Websites und Websites nutzen, die von Benutzern bereitgestellte Inhalte oder Anzeigen akzeptieren oder hosten. Diese Websites können speziell gestalteten Inhalt enthalten, mit dem diese Sicherheitsanfälligkeiten ausgenutzt werden können. Ein Angreifer kann Benutzer jedoch nicht zwingen, die vom Angreifer kontrollierten Inhalte anzuzeigen. Stattdessen muss ein Angreifer Benutzer zu Handlungen verleiten. Zu diesem Zweck werden Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder einer Instant Messenger-Nachricht zu klicken, wodurch die Benutzer zur Website des Angreifers gelangen, oder eine Dateianlage zu öffnen, die per E-Mail gesendet wurde.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Server-Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-074">MS14-074</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Remotedesktopprotokoll kann Umgehung der Sicherheitsfunktion ermöglichen (3003743)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Umgehung der Sicherheitsfunktion ermöglichen, wenn das Remotedesktopprotokoll (RDP) Überwachungsereignisse nicht ordnungsgemäß protokollieren kann. Standardmäßig ist RDP auf keinem Windows-Betriebssystem aktiviert. Systeme, auf denen RDP nicht aktiviert ist, sind nicht gefährdet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-076">MS14-076</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Internetinformationsdiensten (IIS) kann Umgehung der Sicherheitsfunktion ermöglichen (2982998)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft-Internetinformationsdiensten (IIS), das zur Umgehung der Sicherheitsfunktion &quot;Einschränkungen für IP-Adressen und Domänen&quot; führen kann. Bei erfolgreicher Ausnutzung dieser Sicherheitsanfälligkeit können Clients von eingeschränkten oder blockierten Domänen Zugriff auf eingeschränkte Ressourcen erlangen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-077">MS14-077</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory-Verbunddiensten kann Offenlegung von Information ermöglichen (3003381)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Active Directory-Verbunddiensten (AD FS). Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer den Webbrowser geöffnet lässt, nachdem er sich von einer Anwendung abgemeldet hat, und ein Angreifer die Anwendung unmittelbar nach der Abmeldung des Benutzers im Webbrowser erneut öffnet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Wichtig</a> <br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-078">MS14-078</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in IME (Japanisch) kann Rechteerweiterungen ermöglichen (2992719)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Input Method Editor (IME) (Japanisch). Die Sicherheitsanfälligkeit kann auf Basis der Sandkastenanwendungsrichtlinie Sandkastenflucht auf einem System ermöglichen, auf dem eine betroffene Version von Microsoft IME (Japanisch) installiert ist. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann dem Sandkasten einer gefährdeten Anwendung entkommen und mit den Rechten des angemeldeten Benutzers Zugriff auf das betroffene System erlangen. Wenn das betroffene System mit administrativen Berechtigungen angemeldet ist, kann ein Angreifer Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Mittel</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/security/ms14-079">MS14-079</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Kernelmodustreiber kann Denial of Service ermöglichen (3002885)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Denial-of-Service-Angriffe ermöglichen, wenn Angreifer eine speziell manipulierte TrueType-Schriftartdatei auf einer Netzwerkfreigabe platziert und ein Benutzer danach in Windows-Explorer dorthin navigiert. In einem webbasierten Angriffsszenario kann ein Angreifer eine Website mit einer Webseite einrichten, die diese Sicherheitsanfälligkeit ausnutzt. Außerdem können manipulierte Websites und Websites, die von Endbenutzern bereitgestellte Inhalte oder Werbemitteilungen akzeptieren oder hosten, speziell gestaltete Inhalte enthalten, über die diese Sicherheitsanfälligkeit ausgenutzt werden kann. Ein Angreifer kann Endbenutzer jedoch nicht zum Besuch solcher Websites zwingen. Er muss den Benutzer zum Besuch dieser Website verleiten. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Mittel</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
 
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Im Ausnutzbarkeitsindex sind nur Sicherheitsanfälligkeiten enthalten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde.
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
In den nachfolgenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
**Titel der Sicherheitsanfälligkeit**
</td>
<td style="border:1px solid black;">
**CVE-ID**
</td>
<td style="border:1px solid black;" colspan="2">
**Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen**
</td>
<td style="border:1px solid black;" colspan="2">
**Bewertung der Ausnutzbarkeit für ältere Softwareversionen**
</td>
<td style="border:1px solid black;">
**Bewertung der Ausnutzbarkeit durch Denial-of-Service**
</td>
<td style="border:1px solid black;">
**Wichtige Hinweise**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-064](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows OLE-Automatisierung kann Remotecodeausführung in Array ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6332](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6332)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-064](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows OLE bezüglich Remotecodeausführung
</td>
<td style="border:1px solid black;">
[CVE-2014-6352](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6352)
</td>
<td style="border:1px solid black;" colspan="2">
0 - Ausnutzung erkannt
</td>
<td style="border:1px solid black;" colspan="2">
0 - Ausnutzung erkannt
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft ist sich begrenzter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.  
Diese Sicherheitsanfälligkeit wurde erstmals in der Microsoft-Sicherheitsempfehlung [3010060](https://technet.microsoft.com/de-de/library/security/3010060.aspx) beschrieben.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-4143](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4143)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer kann Offenlegung von Informationen der Zwischenablage ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6323](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6323)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6337](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6337)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit durch Umgehung der Internet Explorer ASLR
</td>
<td style="border:1px solid black;">
[CVE-2014-6339](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6339)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer durch domänenübergreifende Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
[CVE-2014-6340](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6340)
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6341](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6341)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6342](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6342)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6343](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6343)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6344](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6344)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer durch domänenübergreifende Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
[CVE-2014-6345](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6345)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer durch domänenübergreifende Offenlegung von Informationen
</td>
<td style="border:1px solid black;">
[CVE-2014-6346](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6346)
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6347](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6347)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6348](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6348)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;">
[CVE-2014-6349](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6349)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich der Erhöhung von Berechtigungen
</td>
<td style="border:1px solid black;">
[CVE-2014-6350](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6350)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6351](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6351)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-065](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung
</td>
<td style="border:1px solid black;">
[CVE-2014-6353](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6353)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-066](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Schannel kann Remotecodeausführung ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6321](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6321)
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-067](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in MSXML kann Remotecodeausführung ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-4118](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4118)
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-068](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
Kerberos-Prüfsumme für die Sicherheitslücke
</td>
<td style="border:1px solid black;" colspan="2">
[CVE-2014-6324](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6324)
</td>
<td style="border:1px solid black;">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
0 - Ausnutzung erkannt
</td>
<td style="border:1px solid black;" colspan="2">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.  
Microsoft ist sich begrenzter, gezielter Angriffe bewusst, bei denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-069](https://technet.microsoft.com/de-de/library/security/ms14-069)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bei doppeltem Löschvorgang in Microsoft Office kann Remotecodeausführung ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6333](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6333)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-069](https://technet.microsoft.com/de-de/library/security/ms14-069)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit bei ungültigem Index in Microsoft Office kann Remotecodeausführung ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6334](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6334)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-069](https://technet.microsoft.com/de-de/library/security/ms14-069)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft Office kann durch einen fehlerhaften Objektzeiger Remotecodeausführung ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6335](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6335)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
1 - Ausnutzung wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
(Keine)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-070](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in TCP/IP kann Erhöhung von Berechtigungen ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-4076](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4076)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-071](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit im Windows-Audiodienst
</td>
<td style="border:1px solid black;">
[CVE-2014-6322](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6322)
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-072](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in TypeFilterLevel
</td>
<td style="border:1px solid black;">
[CVE-2014-4149](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4149)
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-073](https://technet.microsoft.com/de-de/library/security/ms14-073)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in SharePoint kann Rechteerweiterungen ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-4116](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4116)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
2 - Ausnutzung weniger wahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-074](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Remotedesktopprotokoll (RDP) bei Überwachungsfehler
</td>
<td style="border:1px solid black;">
[CVE-2014-6318](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6318)
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-076](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in IIS kann Umgebung der Sicherheitsfunktion ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-4078](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4078)
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die eine Umgehung von Sicherheitsfunktionen ermöglicht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-077](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Active Directory-Verbunddiensten kann Offenlegung von Information ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6331](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6331)
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-078](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Microsoft IME (Japanisch) kann Rechteerweiterungen ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-4077](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-4077)
</td>
<td style="border:1px solid black;" colspan="2">
Nicht betroffen
</td>
<td style="border:1px solid black;" colspan="2">
0 - Ausnutzung erkannt
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Diese Sicherheitsanfälligkeit kann für Rechteerweiterungen ausgenutzt werden.
</td>
</tr>
<tr>
<td style="border:1px solid black;">
[MS14-079](https://technet.microsoft.com/de-de/library/security/ms14-079)
</td>
<td style="border:1px solid black;">
Sicherheitsanfälligkeit in Windows-Kernelmodustreibern kann Denial of Service ermöglichen
</td>
<td style="border:1px solid black;">
[CVE-2014-6317](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2014-6317)
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;" colspan="2">
3 - Ausnutzung unwahrscheinlich
</td>
<td style="border:1px solid black;">
Dauerhaft
</td>
<td style="border:1px solid black;">
Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.
</td>
</tr>
</table>
 
 

Betroffene Software
-------------------

In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.

In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.

**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.

### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows Server 2003**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2003 Service Pack 2  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3003057)  
(Mittel)  
Internet Explorer 7  
(3003057)  
(Mittel)  
Internet Explorer 8  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2989935)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1 Service Pack 1  
(2978114)  
(Hoch)  
Microsoft .NET Framework 2.0 Service Pack 2  
(2978124)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)
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
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3003057)  
(Mittel)  
Internet Explorer 7  
(3003057)  
(Mittel)  
Internet Explorer 8  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2989935)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2978124)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)
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
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(3003057)  
(Mittel)  
Internet Explorer 7  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2989935)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2978124)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)
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
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows Vista**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3006226)  
(Kritisch)  
Windows Vista Service Pack 2  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3003057)  
(Kritisch)  
Internet Explorer 8  
(3003057)  
(Kritisch)  
Internet Explorer 9  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2978116)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3006226)  
(Kritisch)  
Windows Vista x64 Edition Service Pack 2  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3003057)  
(Kritisch)  
Internet Explorer 8  
(3003057)  
(Kritisch)  
Internet Explorer 9  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2978116)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows Server 2008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3006226)  
(Kritisch)  
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3003057)  
(Mittel)  
Internet Explorer 8  
(3003057)  
(Mittel)  
Internet Explorer 9  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2978116)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.0  
(3003381)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3006226)  
(Kritisch)  
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3003057)  
(Mittel)  
Internet Explorer 8  
(3003057)  
(Mittel)  
Internet Explorer 9  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2978116)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.0  
(3003381)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3006226)  
(Kritisch)  
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0 Service Pack 2  
(2978116)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows 7**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(3006226)  
(Kritisch)  
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3003057)  
(Kritisch)  
Internet Explorer 9  
(3003057)  
(Kritisch)  
Internet Explorer 10  
(3003057)  
(Kritisch)  
Internet Explorer 11  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2978120)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für 32-Bit-Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme  
(3006226)  
(Kritisch)  
Windows 7 Service Pack 1 für x64-basierte Systeme  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3003057)  
(Kritisch)  
Internet Explorer 9  
(3003057)  
(Kritisch)  
Internet Explorer 10  
(3003057)  
(Kritisch)  
Internet Explorer 11  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2978120)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows 7 Service Pack 1 für x64-basierte Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows Server 2008 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(3006226)  
(Kritisch)  
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3003057)  
(Mittel)  
Internet Explorer 9  
(3003057)  
(Mittel)  
Internet Explorer 10  
(3003057)  
(Mittel)  
Internet Explorer 11  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2978120)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.0  
(3003381)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 Service Pack 1 für x64-basierte Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3006226)  
(Kritisch)  
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2978120)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows 8 und Windows 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3006226)  
(Kritisch)  
Windows 8 für 32-Bit-Systeme  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978121)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978127)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Internetinformationsdienste 8.0 (Internet Information Services, IIS)  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3006226)  
(Kritisch)  
Windows 8 für x64-basierte Systeme  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978121)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978127)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Internetinformationsdienste 8.0 (Internet Information Services, IIS)  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8 für x64-basierte Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3006226)  
(Kritisch)  
Windows 8.1 für 32-Bit-Systeme  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978122)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978126)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Internetinformationsdienste 8.5 (Internet Information Services, IIS)  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8.1 für 32-Bit-Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3006226)  
(Kritisch)  
Windows 8.1 für x64-basierte Systeme  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3011780)  
(Keine Bewertung des Schweregrads) <sup>[1]</sup>
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978122)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978126)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Internetinformationsdienste 8.5 (Internet Information Services, IIS)  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows 8.1 für x64-basierte Systeme  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows Server 2012 und Windows Server 2012 R2**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3006226)  
(Kritisch)  
Windows Server 2012  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978121)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978127)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Internetinformationsdienste 8.0 (Internet Information Services, IIS)  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.1  
(3003381)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3006226)  
(Kritisch)  
Windows Server 2012 R2  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3003057)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978122)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978126)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Internetinformationsdienste 8.5 (Internet Information Services, IIS)  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 3.0  
(3003381)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Windows RT und Windows RT 8.1**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Windows RT  
(3006226)  
(Kritisch)  
Windows RT  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows RT  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978127)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT  
(3003743)  
(Hoch)
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
<td style="border:1px solid black;">
Windows RT  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows RT 8.1
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3006226)  
(Kritisch)  
Windows RT 8.1  
(3010788)  
(Hoch)
</td>
<td style="border:1px solid black;">
Internet Explorer 11  
(3003057)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(2993958)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3005607)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 4.5.1/4.5.2  
(2978126)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT 8.1  
(3003743)  
(Hoch)
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
<td style="border:1px solid black;">
Windows RT 8.1  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="14">
**Server Core-Installationsoption**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-064**](https://technet.microsoft.com/de-de/library/security/ms14-064)
</td>
<td style="border:1px solid black;">
[**MS14-065**](https://technet.microsoft.com/de-de/library/security/ms14-065)
</td>
<td style="border:1px solid black;">
[**MS14-066**](https://technet.microsoft.com/de-de/library/security/ms14-066)
</td>
<td style="border:1px solid black;">
[**MS14-067**](https://technet.microsoft.com/de-de/library/security/ms14-067)
</td>
<td style="border:1px solid black;">
[**MS14-068**](https://technet.microsoft.com/de-de/library/security/ms14-068)
</td>
<td style="border:1px solid black;">
[**MS14-070**](https://technet.microsoft.com/de-de/library/security/ms14-070)
</td>
<td style="border:1px solid black;">
[**MS14-071**](https://technet.microsoft.com/de-de/library/security/ms14-071)
</td>
<td style="border:1px solid black;">
[**MS14-072**](https://technet.microsoft.com/de-de/library/security/ms14-072)
</td>
<td style="border:1px solid black;">
[**MS14-074**](https://technet.microsoft.com/de-de/library/security/ms14-074)
</td>
<td style="border:1px solid black;">
[**MS14-076**](https://technet.microsoft.com/de-de/library/security/ms14-076)
</td>
<td style="border:1px solid black;">
[**MS14-077**](https://technet.microsoft.com/de-de/library/security/ms14-077)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
<td style="border:1px solid black;">
[**MS14-079**](https://technet.microsoft.com/de-de/library/security/ms14-079)
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
**Keine**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3011780)  
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
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation) (2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation) (2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3011780)  
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
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5.1  
(2978120)  
(Hoch)  
Microsoft .NET Framework 4  
(2978125)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978128)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2991963)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation) (2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978121)  
(Hoch)  
Microsoft .NET Framework 4.5/4.5.1/4.5.2  
(2978127)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation) (3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation) (3002885)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3006226)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(2992611)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(2993958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3011780)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Microsoft .NET Framework 3.5  
(2978122)  
(Hoch)  
Microsoft .NET Framework 4.5.1/4.5.2  
(2978126)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3003743)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation  
(2982998)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 3.0  
(3003381)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
<td style="border:1px solid black;">
Windows Server 2012 R2 (Server Core-Installation)  
(3002885)  
(Mittel)
</td>
</tr>
</table>
 
**Hinweis für MS14-064, MS14-065 und MS14-067**

Windows Technical Preview und Windows Server Technical Preview sind betroffen. Benutzer mit diesen Betriebssystemen werden aufgefordert, das Update anzuwenden, das über [Windows Update](https://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) verfügbar ist. 

**Hinweis für MS14-068**

Windows Technical Preview und Windows Server Technical Preview sind betroffen. Benutzer mit diesen Betriebssystemen werden aufgefordert, das Update anzuwenden, das über [Windows Update](https://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) verfügbar ist. 

<sup>[1]</sup>Bewertungen des Schweregrads treffen nicht auf dieses Betriebssystem zu, da die in diesem Bulletin angesprochene Sicherheitslücke nicht vorhanden ist. Dieses Update bietet eine zusätzliche [Verstärkung der Sicherheit](https://technet.microsoft.com/de-de/library/security/dn848375.aspx), durch die keine bekannten Sicherheitslücken geschlossen werden.

**Hinweis für MS14-078**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

 

### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<td style="border:1px solid black;" colspan="3">
**Microsoft Office 2007**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-069**](https://technet.microsoft.com/de-de/library/security/ms14-069)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Word 2007 Service Pack 3  
(2899527)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 IME (Japanisch)  
(2889913)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;" colspan="3">
**Andere Microsoft Office-Software**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS14-069**](https://technet.microsoft.com/de-de/library/security/ms14-069)
</td>
<td style="border:1px solid black;">
[**MS14-078**](https://technet.microsoft.com/de-de/library/security/ms14-078)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(2899553)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2899526)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht zutreffend
</td>
</tr>
</table>
 
**Hinweis für MS14-078**

Dieses Bulletin umfasst mehr als eine Softwarekategorie. Zusätzliche betroffene Software finden Sie in den anderen Tabellen in diesem Abschnitt. 

 

### Microsoft Server-Software

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
[**MS14-073**](https://technet.microsoft.com/de-de/library/security/ms14-073)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 Service Pack 2  
(2889838)  
(Hoch)
</td>
</tr>
</table>
 
 

Tools und Hinweise zur Erkennung und Bereitstellung von Sicherheitsupdates
--------------------------------------------------------------------------

Es stehen mehrere Ressourcen zur Verfügung, um Administratoren bei der Bereitstellung von Sicherheitsupdates zu helfen.

Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren, lokale und Remotesysteme auf fehlende Sicherheitsupdates und auf häufige Fehlkonfigurationen der Sicherheit zu überprüfen.

Windows Server Update Services (WSUS), Systems Management Server (SMS) und System Center Configuration Manager erleichtern Administratoren die Verteilung von Sicherheitsupdates.

Die im Anwendungskompatibilitäts-Toolkit enthaltenen Komponenten zur Updatekompatibilitätsbewertung helfen dabei, die Vereinbarkeit von Windows-Updates mit installierten Anwendungen zu testen und zu überprüfen.

Weitere Informationen zu diesen und weiteren verfügbaren Tools finden Sie unter [Sicherheitstools](https://technet.microsoft.com/de-de/security/cc297183).

Danksagung
----------

Microsoft erkennt die Bemühungen der Mitglieder der Sicherheitscommunity an, die uns durch die verantwortungsvolle Offenlegung.von Sicherheitsanfälligkeiten helfen, unsere Kunden zu schützen. Weitere Informationen finden Sie unter [Danksagung](https://technet.microsoft.com/de-de/library/security/dn820091.aspx).

Weitere Informationen:
----------------------

### Microsoft Windows-Tool zum Entfernen bösartiger Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://technet.microsoft.com/de-de/security/dn467918) aufgeführt sind.

### Sicherheitsstrategien und Community

**Updateverwaltungsstrategien**

Auf der Seite [Patchmanagement](https://technet.microsoft.com/de-de/library/bb466251.aspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://update.microsoft.com/microsoftupdate/v6/vistadefault.aspx?ln=de-de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

### Support

Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://go.microsoft.com/fwlink/?linkid=21742), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.

Sicherheitslösungen für IT-Experten: [TechNet Security – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)

Hilfe beim Schützen des Computers, auf dem Windows ausgeführt wird, vor Viren und Schadsoftware: [Safety and Security Center](https://www.microsoft.com/de-de/security/default.aspx)

Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx?ln=de)

### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

### Revisionen

-   V1.0 (11. November 2014): Bulletin Summary veröffentlicht.
-   V2.0 (18. November 2014): Das Bulletin Summary wurde mit der Dokumentation der außerplanmäßigen Veröffentlichung von MS14-068 und für MS14-066 mit der Ankündigung des erneuten Angebots von Update 2992611 für Systeme mit Windows Server 2008 R2 und Windows Server 2012 überarbeitet.
-   V2.1 (19. Dezember 2014): Das Bulletin wurde überarbeitet, um der Tabelle „Betroffene Software“ für MS14-076 einen Eintrag bezüglich der Windows 2012 Server Core-Installation und der Windows 2012 R2 Server Core-Installation hinzuzufügen.

*Seite generiert am 19.12.2014 13:20Z-08:00.*
