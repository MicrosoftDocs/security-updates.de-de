---
TOCTitle: 'MS10-DEC'
Title: Microsoft Security Bulletin Summary für Dezember 2010
ms:assetid: 'ms10-dec'
ms:contentKeyID: 61225081
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms10-dec(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Dezember 2010
=====================================================

Veröffentlicht: Dienstag, 14. Dezember 2010 | Aktualisiert: Mittwoch, 15. Dezember 2010

**Version:** 1.1

In diesem Bulletin Summary sind die im Dezember 2010 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Dezember 2010 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 9. Dezember 2010 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 15. Dezember 2010 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Dezember.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454444&eventcategory=4&culture=en-us&countrycode=us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx)

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
<th style="border:1px solid black;" >Neustartanforderung</th>
<th style="border:1px solid black;" >Betroffene Software</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206495">MS10-090</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2416400)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten und drei öffentlich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=203895">MS10-091</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im OTF-Treiber (OpenType Font) können Remotecodeausführung ermöglichen (2296199)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten im Windows-OTF-Treiber (OpenType Font), die Remotecodeausführung ermöglichen können. Ein Angreifer kann eine speziell gestaltete OpenType-Schriftart auf einer Netzwerkfreigabe hosten. Der betroffene Steuerpfad wird dann ausgelöst, wenn der Benutzer in Windows Explorer auf die Freigabe navigiert, wodurch der speziell gestalteten Schriftart ermöglicht wird, die vollständige Kontrolle über ein betroffenes System zu erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=203463">MS10-092</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Taskplaner kann Erhöhung von Berechtigungen ermöglichen (2305420)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im Windows Taskplaner. Diese Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206698">MS10-093</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Movie Maker kann Remotecodeausführung ermöglichen (2424434)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Windows Movie Maker. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, eine gültige Datei in Windows Movie Maker zu öffnen, die sich im selben Netzwerkverzeichnis befindet wie eine speziell gestaltete Bibliotheksdatei. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von einer anfälligen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206699">MS10-094</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Media Encoder kann Remotecodeausführung ermöglichen (2447961)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Windows Media Encoder. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, eine gültige PRX-Datei (Windows Media Profile) zu öffnen, die sich im selben Netzwerkverzeichnis befindet wie eine speziell gestaltete Bibliotheksdatei. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von einer anfälligen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206683">MS10-095</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Windows kann Remotecodeausführung ermöglichen (2385678)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer einen Dateityp wie „.eml“ und „.rss“ (Windows Live Mail) oder „.wpost“ (Microsoft Live Writer) öffnet, der sich in demselben Netzwerkordner befindet wie eine speziell gestaltete Bibliotheksdatei. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von einer anfälligen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206738">MS10-096</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Adressbuch kann Remotecodeausführung ermöglichen (2423089)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im Windows-Adressbuch. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Windows-Adressbuchdatei öffnet, die sich im selben Netzwerkordner befindet wie eine speziell gestaltete Bibliotheksdatei. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von einer anfälligen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206689">MS10-097</a></td>
<td style="border:1px solid black;"><strong>Nicht sicheres Laden von Bibliotheken im Assistenten zum Anmelden von Internetverbindungen kann Remotecodeausführung ermöglichen (2443105)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im Assistenten zum Anmelden von Internetverbindungen in Microsoft Windows. Dieses Sicherheitsupdate wird für alle unterstützten Editionen von Windows XP und Windows Server 2003 als Hoch eingestuft. Alle unterstützten Editionen von Windows Vista, Windows Server 2008, Windows 7 und Windows Server 2008 R2 sind nicht von der Sicherheitsanfälligkeit betroffen.<br />
<br />
Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine INS- oder ISP-Datei öffnet, die sich im selben Netzwerkordner befindet wie eine speziell gestaltete Bibliotheksdatei. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von einer anfälligen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=204869">MS10-098</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Erhöhung von Berechtigungen ermöglichen (2436673)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich und mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206365">MS10-099</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Routing and Remote Access kann Erhöhung von Berechtigungen ermöglichen (2440591)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Komponente „Routing and Remote Access NDProxy“ von Microsoft Windows. Dieses Sicherheitsupdate wird für alle unterstützten Editionen von Windows XP und Windows Server 2003 als Hoch eingestuft. Alle unterstützten Editionen von Windows Vista, Windows Server 2008, Windows 7 und Windows Server 2008 R2 sind nicht von der Sicherheitsanfälligkeit betroffen.<br />
<br />
Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=204906">MS10-100</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Consent-Benutzeroberfläche kann Erhöhung von Berechtigungen ermöglichen (2442962)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Zustimmungsbenutzeroberfläche. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer eine speziell gestaltete Anwendung auf einem betroffenen System ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und die SeImpersonatePrivilege-Berechtigung und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=201319">MS10-101</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows Netlogon-Dienst kann Denial-of-Service ermöglichen (2207559)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Netlogon RPC-Dienst auf betroffenen Versionen von Windows Server, die als Domänencontroller konfiguriert sind. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer ein speziell gestaltetes RPC-Paket an die Schnittstelle des Netlogon RPC-Dienstes auf einem betroffenen System sendet. Ein Angreifer benötigt zur Ausnutzung dieser Sicherheitsanfälligkeit Administratorrechte auf einem Computer, der mit derselben Domäne verknüpft ist wie der betroffene Domänencontroller.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=205309">MS10-102</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Hyper-V kann Denial-of-Service ermöglichen (2345316)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Server 2008 Hyper-V und Windows Server 2008 R2 Hyper-V. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein authentifizierter Benutzer eine fehlerhafte Sequenz von Computeranweisungen auf einem der virtuellen Gastcomputer ausführt, die vom Hyper-V-Server gehostet wird. Ein Angreifer muss über gültige Anmeldeinformationen verfügen und speziell gestaltete Inhalte von einem virtuellen Gastcomputer senden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=198156">MS10-103</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Publisher können Remotecodeausführung ermöglichen (2292970)</strong><br />
<br />
Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Publisher, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Publisher-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=206469">MS10-104</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Outlook kann Remotecodeausführung ermöglichen (2455005)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft SharePoint. Die Sicherheitsanfälligkeit kann Remotecodeausführung im Sicherheitskontext eines Gastbenutzers ermöglichen, wenn ein Angreifer eine speziell gestaltete SOAP-Anforderung an den Startprogrammdienst für die Dokumentkonvertierung einer SharePoint Server-Umgebung gesendet hat, die den Lastenausgleichsmodul-Dienst für die Dokumentkonvertierung verwendet. Standardmäßig sind der Lastenausgleichsmodul-Dienst für die Dokumentkonvertierung und der Startprogrammdienst für die Dokumentkonvertierung nicht in Microsoft Office SharePoint Server 2007 aktiviert.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft SharePoint</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147425">MS10-105</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office-Grafikfiltern können Remotecodeausführung ermöglichen (968095)</strong><br />
<br />
Dieses Sicherheitsupdate behebt sieben vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Bilddatei mit Microsoft Office anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=204624">MS10-106</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Exchange Server kann Denial-of-Service ermöglichen (2407132)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Exchange Server. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein authentifizierter Angreifer einem Computer, auf dem der Exchange-Dienst ausgeführt wird, eine speziell gestaltete Netzwerknachricht sendet. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Mittel</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Exchange</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach absteigender Bewertung der Ausnutzbarkeit und dann CVE ID aufgeführt. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259.aspx).
  
| Kennung des Bulletins                                     | Titel der Sicherheitsanfälligkeit                                                                                            | CVE-ID                                                                           | Ausnutzbarkeitsindex - Bewertung                                                                                     | Wichtige Hinweise                                                                    |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|  
| [MS10-103](https://go.microsoft.com/fwlink/?linkid=198156) | Sicherheitsanfälligkeit bzgl. Heap-Beschädigung durch Größenwert in pubconv.dll                                              | [CVE-2010-2569](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2569) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-103](https://go.microsoft.com/fwlink/?linkid=198156) | Sicherheitsanfälligkeit in pubconv.dll durch Heapüberlauf                                                                    | [CVE-2010-2570](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2570) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-097](https://go.microsoft.com/fwlink/?linkid=206689) | Sicherheitsanfälligkeit aufgrund nicht sicheren Ladens von Bibliotheken im Assistenten zum Anmelden von Internetverbindungen | [CVE-2010-3144](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3144) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.**                         |  
| [MS10-096](https://go.microsoft.com/fwlink/?linkid=206738) | Sicherheitsanfälligkeit aufgrund nicht sicheren Ladens von Bibliotheken                                                      | [CVE-2010-3147](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3147) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.**                         |  
| [MS10-092](https://go.microsoft.com/fwlink/?linkid=203463) | Sicherheitsanfälligkeit im Taskplaner                                                                                        | [CVE-2010-3338](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3338) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt**    |  
| [MS10-090](https://go.microsoft.com/fwlink/?linkid=206495) | Sicherheitsanfälligkeit durch Speicherbeschädigung bei HTML-Objekten                                                         | [CVE-2010-3340](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3340) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-090](https://go.microsoft.com/fwlink/?linkid=206495) | Sicherheitsanfälligkeit durch Speicherbeschädigung bei HTML-Objekten                                                         | [CVE-2010-3343](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3343) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-090](https://go.microsoft.com/fwlink/?linkid=206495) | Sicherheitsanfälligkeit durch Speicherbeschädigung bei HTML-Elementen                                                        | [CVE-2010-3345](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3345) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-090](https://go.microsoft.com/fwlink/?linkid=206495) | Sicherheitsanfälligkeit durch Speicherbeschädigung bei HTML-Elementen                                                        | [CVE-2010-3346](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3346) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-098](https://go.microsoft.com/fwlink/?linkid=204869) | Sicherheitsanfälligkeit in Win32k durch Pufferüberlauf                                                                       | [CVE-2010-3939](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3939) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.**                         |  
| [MS10-098](https://go.microsoft.com/fwlink/?linkid=204869) | Sicherheitsanfälligkeit in Win32k durch doppelte Freigabe des PFE-Zeigers                                                    | [CVE-2010-3940](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3940) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-098](https://go.microsoft.com/fwlink/?linkid=204869) | Sicherheitsanfälligkeit in Win32k bei der Cursorverknüpfung                                                                  | [CVE-2010-3943](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3943) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-098](https://go.microsoft.com/fwlink/?linkid=204869) | Sicherheitsanfälligkeit in Win32k bezüglich Speicherbeschädigung                                                             | [CVE-2010-3944](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3944) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-105](https://go.microsoft.com/fwlink/?linkid=147425) | Sicherheitsanfälligkeit in FlashPix-Bildkonverter durch Pufferüberlauf                                                       | [CVE-2010-3951](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3951) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-091](https://go.microsoft.com/fwlink/?linkid=203895) | Sicherheitsanfälligkeit durch doppelte Freigabe bei OpenType-Schriftarten                                                    | [CVE-2010-3957](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3957) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-091](https://go.microsoft.com/fwlink/?linkid=203895) | Sicherheitsanfälligkeit in der OpenType-CMAP-Tabelle                                                                         | [CVE-2010-3959](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3959) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-100](https://go.microsoft.com/fwlink/?linkid=204906) | Sicherheitsanfälligkeit durch Nachahmung der Zustimmungsbenutzeroberfläche                                                   | [CVE-2010-3961](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3961) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-090](https://go.microsoft.com/fwlink/?linkid=206495) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung aufgrund von Nichtinitialisierung                                     | [CVE-2010-3962](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3962) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt**    |  
| [MS10-099](https://go.microsoft.com/fwlink/?linkid=206365) | Sicherheitsanfälligkeit in NDProxy im Kernel durch Pufferüberlauf                                                            | [CVE-2010-3963](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3963) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-104](https://go.microsoft.com/fwlink/?linkid=206469) | Sicherheitsanfälligkeit bezüglich fehlerhafter Anforderung zur Codeausführung                                                | [CVE-2010-3964](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3964) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-094](https://go.microsoft.com/fwlink/?linkid=206699) | Sicherheitsanfälligkeit aufgrund nicht sicheren Ladens von Bibliotheken                                                      | [CVE-2010-3965](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3965) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.**                         |  
| [MS10-095](https://go.microsoft.com/fwlink/?linkid=206683) | Sicherheitsanfälligkeit durch nicht sichereres Laden von Bibliotheken in BranchCache                                         | [CVE-2010-3966](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3966) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | (Keine)                                                                              |  
| [MS10-093](https://go.microsoft.com/fwlink/?linkid=206698) | Sicherheitsanfälligkeit aufgrund nicht sicheren Ladens von Bibliotheken                                                      | [CVE-2010-3967](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3967) | [**1**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Konsistenter Angreifercode wahrscheinlich       | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.**                         |  
| [MS10-103](https://go.microsoft.com/fwlink/?linkid=198156) | Sicherheitsanfälligkeit in Pubconv.dll durch Speicherbeschädigung aufgrund ungültigen Indexes in Array                       | [CVE-2010-2571](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2571) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-098](https://go.microsoft.com/fwlink/?linkid=204869) | Sicherheitsanfälligkeit in Win32k durch doppelte Freigabe                                                                    | [CVE-2010-3941](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3941) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-098](https://go.microsoft.com/fwlink/?linkid=204869) | Sicherheitsanfälligkeit in Win32k bei WriteAV                                                                                | [CVE-2010-3942](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3942) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-105](https://go.microsoft.com/fwlink/?linkid=147425) | Sicherheitsanfälligkeit in CGM-Bildkonverter durch Pufferüberlauf                                                            | [CVE-2010-3945](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3945) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-105](https://go.microsoft.com/fwlink/?linkid=147425) | Sicherheitsanfälligkeit in PICT-Bildkonverter durch Ganzzahlüberlauf                                                         | [CVE-2010-3946](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3946) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-105](https://go.microsoft.com/fwlink/?linkid=147425) | Sicherheitsanfälligkeit in TIFF-Bildkonverter durch Heapüberlauf                                                             | [CVE-2010-3947](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3947) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-105](https://go.microsoft.com/fwlink/?linkid=147425) | Sicherheitsanfälligkeit in TIFF-Bildkonverter durch Pufferüberlauf                                                           | [CVE-2010-3949](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3949) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-105](https://go.microsoft.com/fwlink/?linkid=147425) | Sicherheitsanfälligkeit in TIFF-Bildkonverter durch Speicherbeschädigung                                                     | [CVE-2010-3950](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3950) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-105](https://go.microsoft.com/fwlink/?linkid=147425) | Sicherheitsanfälligkeit in FlashPix-Bildkonverter durch Heap-Beschädigung                                                    | [CVE-2010-3952](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3952) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-103](https://go.microsoft.com/fwlink/?linkid=198156) | Sicherheitsanfälligkeit bezüglich Speicherbeschädigung bei Arrayindizierung                                                  | [CVE-2010-3955](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3955) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-091](https://go.microsoft.com/fwlink/?linkid=203895) | Sicherheitsanfälligkeit beim Indizieren von OpenType-Schriftarten                                                            | [CVE-2010-3956](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3956) | [**2** -](https://technet.microsoft.com/de-de/security/cc998259.aspx) Inkonsistenter Angreifercode wahrscheinlich     | (Keine)                                                                              |  
| [MS10-101](https://go.microsoft.com/fwlink/?linkid=201319) | DoS-Sicherheitsanfälligkeit aufgrund einer Null-Dereferenzierung in Netlogon RPC                                             | [CVE-2010-2742](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2742) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Funktionierender Angreifercode unwahrscheinlich | Diese Sicherheitsanfälligkeit bezieht sich lediglich auf Denial-of-Service-Angriffe. |  
| [MS10-106](https://go.microsoft.com/fwlink/?linkid=204624) | Sicherheitsanfälligkeit in Exchange Server bezüglich Endlosschleife                                                          | [CVE-2010-3937](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3937) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Funktionierender Angreifercode unwahrscheinlich | Diese Sicherheitsanfälligkeit bezieht sich lediglich auf Denial-of-Service-Angriffe. |  
| [MS10-103](https://go.microsoft.com/fwlink/?linkid=198156) | Sicherheitsanfälligkeit in Microsoft Publisher bzgl. Speicherbeschädigung                                                    | [CVE-2010-3954](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3954) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Funktionierender Angreifercode unwahrscheinlich | (Keine)                                                                              |  
| [MS10-102](https://go.microsoft.com/fwlink/?linkid=205309) | Sicherheitsanfälligkeit im VMBus von Hyper-V                                                                                 | [CVE-2010-3960](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3960) | [**3**](https://technet.microsoft.com/de-de/security/cc998259.aspx) - Funktionierender Angreifercode unwahrscheinlich | Diese Sicherheitsanfälligkeit bezieht sich lediglich auf Denial-of-Service-Angriffe. |
  
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
<th colspan="14" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-090**](https://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](https://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](https://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](https://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](https://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](https://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](https://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](https://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](https://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](https://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](https://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](https://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](https://go.microsoft.com/fwlink/?linkid=205309)
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
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=6031d98a-cd0f-4dd8-80b6-70a7167e9e55)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=922a0835-7f69-4e37-a9f7-c64e976e3513)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=a55b8029-9499-4219-99b7-65c30b0b864a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=cdef3358-ad3e-40a6-9ba5-3be220a56a65)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=ef0ada2c-965f-438f-a1d3-bd45db8460c1)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=46baa431-126c-4fa5-9a7b-525008e2817d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=fa9a1aac-b9c5-4d4e-9083-a080ad4ccc6f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=bb9d1657-5beb-4372-b74c-a612a6fff5a8)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=4d0ae558-a4f2-4048-b5fd-ba072ca35e48)  
(Hoch)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=5d3a5678-77f8-4ebc-8775-aedd25ef0eb8)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a7c826b0-4aac-41ce-b297-6b6e11105c14)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d5207bf5-7e58-4001-aa8f-f9a4b2c037d8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=070fef8e-ba09-40f4-abaa-9cebf08983c3)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=dc777e61-e1e3-43bf-a84d-22c4a69c135d)  
(Hoch)  
[Windows Media Encoder 9 x64](https://www.microsoft.com/download/details.aspx?familyid=550957c2-ce66-439f-95ea-681237513f75)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b9ce9d62-2eaa-48d8-bb6d-ea137e63d077)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6dabc306-c858-46b1-815c-cd8d011ff62e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1f277ae4-4f85-4c8a-bfc5-dcdc8afed133)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=238bb885-eae6-464a-bb3d-679025f1cb50)  
(Hoch)
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
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-090**](https://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](https://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](https://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](https://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](https://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](https://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](https://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](https://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](https://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](https://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](https://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](https://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](https://go.microsoft.com/fwlink/?linkid=205309)
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
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=4f1f41fb-368a-42e6-8d17-fca83b64f57b)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a3b57d26-5551-4785-86cf-41b532d78979)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4f5a3677-0990-4702-bf08-af64cf12cb6c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9b70334c-490d-446c-988a-a88a75595fd4)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=ef0ada2c-965f-438f-a1d3-bd45db8460c1)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e0b2837c-019b-419b-954d-5bdc71a3a332)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8fa2cfa4-a01d-4910-b69f-736aeb585bab)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4aa39f59-2177-459f-9b8a-9543330d48ec)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c87af292-a068-4089-aab8-115c18b4b024)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ad843b97-2f6e-4406-a17a-627b7db8a926)  
(Hoch)
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=6a9f56a0-230a-4dde-94da-f051ebf51f47)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=8b0d2a3a-7fed-4d48-9ec5-8558000e51bb)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=1e134e5d-84fb-432b-99b1-593b1be5d5a4)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=08328e82-b012-4ea5-bf89-becb4881084f)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=dc777e61-e1e3-43bf-a84d-22c4a69c135d)  
(Hoch)  
[Windows Media Encoder 9 x64](https://www.microsoft.com/download/details.aspx?familyid=550957c2-ce66-439f-95ea-681237513f75)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4c5cb600-9a39-40a0-be42-1593b1e0b97d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=17b0b340-73b2-42a7-9d86-1297c63dcc2b)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=bca61d61-d5cf-49a4-ab99-b61e50e8f619)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e17b8878-d065-49cc-bdba-0f24cdf35ea3)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0b0a06e7-0ae5-41f4-9ff5-d524fc0afbfa)  
(Hoch)
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=7c1cf126-604c-4f70-bbe8-aa4d145eb68f)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=96884bfa-00c8-4263-9936-d7c054919dd3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=15588d6a-f576-4e3d-95e8-d422af8a94de)  
(Hoch)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9abc8270-f3ac-474d-9ebc-410aaa6262cc)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=04a178cc-1afd-4e47-8cab-05e402e5a568)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=4fce129d-2b4e-4a66-af27-bbbde1e65ba1)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ad896d80-167f-4e8f-a448-cac93516f4d0)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=7c0c2850-e81d-4347-aeb3-47036caa7c1b)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-090**](https://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](https://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](https://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](https://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](https://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](https://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](https://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](https://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](https://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](https://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](https://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](https://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](https://go.microsoft.com/fwlink/?linkid=205309)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=897351de-9697-4954-aa7e-169e980b932c)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=bebf0df0-5ebe-44b4-9ace-b3085a993e58)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2ddb8a06-c9cc-4d33-b6d1-22dbda2d871f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=48f10251-34d8-4149-b4b2-bf3ec28f5846)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.6](https://www.microsoft.com/download/details.aspx?familyid=55141a02-3ad3-4691-98b9-80dd8ecb14c5)<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=e8a57950-43cd-486f-bd97-70b0ad360a0b)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a1c7f1b5-e054-4cd6-857d-2ab0a2fe9f62)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b824d3b9-2ce1-4abc-ae06-68aef1250be9)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=85265a23-5094-4007-8d33-f402cabd1664)  
(Hoch)
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
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=171c02f9-f7d2-42f2-ba31-4c819a43784a)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=837b6056-af04-4aed-8afe-cc392770a590)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9a245f3c-ffb6-4ccd-956c-e7d1231fca30)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=099ccc5f-b92f-4d06-bcb5-92e35c49f613)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.6](https://www.microsoft.com/download/details.aspx?familyid=5b078136-a492-4a2e-939d-82799f774d82)<sup>[1]</sup>
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=f98c3b96-acb5-49f1-be42-3dd44d316408)  
(Hoch)  
[Windows Media Encoder 9 x64](https://www.microsoft.com/download/details.aspx?familyid=e1054088-f484-4f44-ba0e-5cbd21773c0c)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=73624b68-a69d-4517-b971-f0b7d2ccc9d6)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f4c42cfe-b7f2-4436-919e-4bd305a3439a)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=63c7257a-16bf-4108-80b9-9dfe53528348)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-090**](https://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](https://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](https://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](https://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](https://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](https://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](https://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](https://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](https://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](https://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](https://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](https://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](https://go.microsoft.com/fwlink/?linkid=205309)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=f3785f3b-64c6-46a4-8e3a-9b9448124a8f)\*\*  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=98183a76-5642-4e19-b488-029eb7ed3942)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=87149ec2-74a8-4dea-b7e3-873558e0103e)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=bdc9564a-4091-4cde-963a-239513db6c17)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=a4ea028f-edfc-4237-8325-7ece11fcf437)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=118f528f-bd05-49c2-a4a4-78314cd00992)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6e2f572a-4169-47f2-a872-5466997122ed)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=14e079a8-01a4-47c9-bd47-f5c9a6ca070a)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6793f75b-cdf4-42ef-a53e-a1acb5b662d1)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=4b81aae5-6034-4c83-b5d2-e7e472435284)\*\*  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d47b457d-e995-4a7e-9bfa-eebab9b3a729)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=523a47d3-771d-471a-889b-16311c276a00)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dff39bfe-0799-4912-ae22-392562178ae6)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](https://www.microsoft.com/download/details.aspx?familyid=f468d2b5-f02c-4691-9fb5-a7f69752f126)\*\*  
(Hoch)  
[Windows Media Encoder 9 x64](https://www.microsoft.com/download/details.aspx?familyid=533d91d8-0291-421e-9701-3bd86d18bc45)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=77e288fb-b51f-4f57-baac-1443d8fbd37b)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=09a4b646-989d-43ef-a3e8-64af8b380a14)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6baf92b7-a336-45f2-a1ba-c00c34dfb76f)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=85add876-ca5a-4a92-984e-188a72e349fc)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b8c06bbc-6e84-4cf1-89f0-c0d34cfffaed)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=8ddafaaf-84a0-4325-b06f-4aac7cd61274)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=959146ee-0e70-4e56-9012-72ed59aeb24b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=cf341a35-32ea-4ff7-aca9-1a4683c100ee)  
(Hoch)
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
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=82f71194-6f1f-4f43-8752-4bf5e5f94a93)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=46522323-837e-4a74-9cf0-45f69343e776)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7a4b23d4-f68e-4d5b-8814-d9247145f164)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-090**](https://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](https://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](https://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](https://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](https://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](https://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](https://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](https://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](https://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](https://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](https://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](https://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](https://go.microsoft.com/fwlink/?linkid=205309)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
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
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c288fe87-b113-4615-9b02-5e388bcb5241)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=ff590db8-4264-42ba-9e07-88d100e1c4f5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=cf85cdb6-58c7-4144-82f6-f01a6a4f9c3a)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=75591d37-2cb8-4cdf-acbb-89cd0d1a9290)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=4e8ad5cd-af27-4f00-9378-ad778b8ee7b3)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=aa7de2e4-ba48-4d58-b034-05349f0eb920)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=f7c7d57a-d031-46a3-9613-eae2b9cb6401)  
(Hoch)
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
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=2cf4ac70-88b4-4840-9895-2bcf119312a7)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=4ea4e339-9db2-4b99-b567-80ee55ecdf92)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=0597018d-39f5-4ca9-b437-63d9e68f264d)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=3a0c4dd0-98b4-4e7a-99ed-22b9d9f76cd1)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=35a3e821-b463-411c-858b-d01eb5aed42b)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=b21db627-91c2-4ebf-b7c0-38ac58ae5b6c)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=e52c36f5-637b-4928-83d0-27514c6cc384)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-090**](https://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](https://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](https://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](https://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](https://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](https://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](https://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](https://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](https://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](https://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](https://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](https://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](https://go.microsoft.com/fwlink/?linkid=205309)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
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
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=99a91ba7-035b-4717-ada5-c1ad6645db64)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=e52f7869-474a-44c8-a102-e766c576fc01)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=28c832fb-4937-4652-8799-eab6c76d05fb)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=f58a765f-cea9-456d-b0ab-bfc70b109cbf)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9e2c95f6-9381-4484-b11b-814ab9138118)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=d417ebce-7841-4bbb-8abc-b15ef5f4b733)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=b823a7aa-0eb9-42dd-bf56-8907d94b314a)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=d7307afd-84a0-434e-9658-bf9f8ae4b938)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=39b7abc7-65a4-4dfd-92ba-c638e3de1118)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c26de145-94b8-404a-b946-744988fab83b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=a21d061a-794a-4012-b3cd-c67445c074f5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=3ad64d5c-2d81-4ac8-934e-8917b2fcf961)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=13a9f838-ac07-43dc-9aee-a77207998e1e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=cb4211f3-1082-4245-8f03-7cbac90e9a31)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=7eeac1bb-9f86-4ea5-b30f-980d52be5044)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=66b2506d-80e0-4e32-86e6-0908ef56ae90)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS10-093**

<sup>[1]</sup> Windows Movie Maker 2.6 ist ein optionaler Download, der unter den angegebenen Betriebssystemen installiert werden kann.

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS10-103**](https://go.microsoft.com/fwlink/?linkid=198156)
</td>
<td style="border:1px solid black;">
[**MS10-105**](https://go.microsoft.com/fwlink/?linkid=147425)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f540692c-e404-4383-8937-4d6a36475da5)  
(KB2284692)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=724d0ad6-ba5f-4dbf-b280-3fb36335d33b)<sup>[1]</sup>
(KB2289162)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e600de65-3e9d-4e37-8906-8b7091ff523e)  
(KB2284695)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=976857e9-77fc-4667-88ca-7637e57536cd)<sup>[1]</sup>
(KB2289163)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=79275011-bdc1-446a-8ea6-56fc31bd9c35)  
(KB2284697)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=676eeed6-f2b7-4265-afc7-a82ffdbeb290)  
(KB2288931)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=99e18990-75e9-497e-9b4f-5d7ef8656ab2)  
(KB2409055)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=6d644494-b530-4b37-bc37-8a8a7edefe53)  
(KB2289078)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2010 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=9b27ee11-e563-4152-9691-25eec1ee9966)  
(KB2409055)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=58e54779-aa8f-41b3-9993-8cec12c49082)  
(KB2289078)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-103**](https://go.microsoft.com/fwlink/?linkid=198156)
</td>
<td style="border:1px solid black;">
[**MS10-105**](https://go.microsoft.com/fwlink/?linkid=147425)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Converter Pack
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Converter Pack](https://www.microsoft.com/download/details.aspx?familyid=dcded2ee-0673-4afe-abe6-04941a2ad306)  
(KB2456849)  
(Hoch)
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
[Microsoft Works 9](https://www.microsoft.com/download/details.aspx?familyid=10f6f330-05d8-4b60-9ebb-822a7321ac0f)  
(KB2431831)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für MS10-105**

<sup>[1]</sup>Benutzer, die die angezeigte Software verwenden, müssen auch das in MS10-087 bereitgestellte Microsoft Office Update installieren, um vor den in MS10-105 beschriebenen Sicherheitsanfälligkeiten geschützt zu sein.

<sup>[2]</sup>Bewertungen des Schweregrads treffen nicht auf dieses Update zu, da diese Software nicht von der Sicherheitsanfälligkeit betroffen ist, die in diesem Bulletin erörtert wird. Als Tiefenverteidigungsmaßnahme zum Schutz vor möglicherweise in der Zukunft entdeckten Sicherheitsanfälligkeiten empfiehlt Microsoft jedoch den Benutzern dieser Software, dieses Sicherheitsupdate zu installieren.

#### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-104**](https://go.microsoft.com/fwlink/?linkid=206469)
</td>
<td style="border:1px solid black;">
[**MS10-106**](https://go.microsoft.com/fwlink/?linkid=204624)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Office SharePoint Server 2007 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=3c8fb9f9-7920-43ea-b618-e26dc3360c60)  
(KB2433089)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=3db09280-24bd-42e0-9ae3-02c9bf3e8ee3)  
(KB2433089)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS10-104**](https://go.microsoft.com/fwlink/?linkid=206469)
</td>
<td style="border:1px solid black;">
[**MS10-106**](https://go.microsoft.com/fwlink/?linkid=204624)
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007 Service Pack 2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2007 Service Pack 2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=7b983156-9e9f-4d29-9e9b-2369747e3b62)  
(KB2407132)  
(Mittel)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**SystemCenter Configuration Manager 2007**

Configuration Manager 2007-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit Configuration Manager 2007 können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in Configuration Manager 2007 erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in Configuration Manager 2007 ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen dazu, wie Administratoren mithilfe von Configuration Manager 2007 Updates bereitstellen können, finden Sie in [Softwareupdateverwaltung](https://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Weitere Informationen zu Configuration Manager finden Sie auf der Website [System Center Configuration Manager](https://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](https://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe den früheren Abschnitt, **SystemCenter Configuration Manager 2007**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](https://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/download/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24da89e9-b581-47b0-b45e-492dd6da2971&amp;displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Aniway von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS10-090 beschriebenes Problem
-   Nicolas Joly vom [VUPEN Vulnerability Research Team](https://www.vupen.com/) für den Hinweis auf ein in MS10-090 beschriebenes Problem
-   Steven Fewer in Zusammenarbeit mit [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) für den Hinweis auf ein in MS10-090 beschriebenes Problem
-   [Peter Vreugdenhil](https://vreugdenhilresearch.nl/) in Zusammenarbeit mit [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) für den Hinweis auf ein in MS10-090 beschriebenes Problem
-   Masatoshi Sato von [AZIA CO., LTD.](https://www.azia.jp) für den Hinweis auf ein in MS10-090 beschriebenes Problem
-   [Yosuke Hasegawa](https://utf-8.jp/) für die Zusammenarbeit mit uns an einem in MS10-090 beschriebenen Problem
-   Jose Antonio Vazquez Gonzalez von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS10-090 beschriebenes Problem
-   Marc Schoenefeld vom [Red Hat Security Response Team](https://www.redhat.com/security/team/), in Zusammenarbeit dem [Opera Security Team](https://www.opera.com/security/), für den Hinweis auf ein in MS10-091 beschriebenes Problem
-   Marc Schoenefeld vom [Red Hat Security Response Team](https://www.redhat.com/security/team/) für den Hinweis auf ein in MS10-091 beschriebenes Problem
-   Paul-Kenji Cahier Furuya für den Hinweis auf ein in MS10-091 beschriebenes Problem
-   Sergey Golovanov, Alexander Gostev, Maxime Golovkin und Alexey Monastyrsky von [Kaspersky Lab](https://usa.kaspersky.com/) und Vitaly Kiktenko und Alexander Saprykin von [Design and Test Lab](https://www.dnt-lab.com/) für den Hinweis auf ein in MS10-092 beschriebenes Problem.
-   Liam O Murchu von [Symantec](https://www.symantec.com/index.jsp) für den Hinweis auf ein in MS10-092 beschriebenes Problem
-   Alexandr Matrosov, Eugene Rodionov, Juraj Malcho und David Harley von [ESET](https://www.eset.com/) für den Hinweis auf ein in MS10-092 beschriebenes Problem
-   Haifei Li von [Fortinets FortiGuard Labs](https://www.fortiguard.com/) für den Hinweis auf ein in MS10-095 beschriebenes Problem
-   Simon Raner von [ACROS Security](https://www.acrossecurity.com/) für den Hinweis auf ein in MS10-096 beschriebenes Problem
-   HD Moore von [Rapid7](https://www.rapid7.com/) für den Hinweis auf ein in MS10-096 beschriebenes Problem
-   Muhaimin Dzulfakar von [NGS Software](https://www.ngssoftware.com/) für den Hinweis auf ein in MS10-096 beschriebenes Problem
-   Muhaimin Dzulfakar von [NGS Software](https://www.ngssoftware.com/) für den Hinweis auf ein in MS10-097 beschriebenes Problem
-   Tarjei Mandt von [Norman](https://www.norman.com/) für den Hinweis auf vier in MS10-098 beschriebene Probleme
-   Stéfan Le Berre von [Sysdream](https://www.sysdream.com/) für den Hinweis auf ein in MS10-098 beschriebenes Problem
-   Honggang Ren von [Fortinets FortiGuard Labs](https://www.fortiguard.com/) für den Hinweis auf ein in MS10-099 beschriebenes Problem
-   Cesar Cerrudo von [Argeniss](https://www.argeniss.com/) für den Hinweis auf ein in MS10-100 beschriebenes Problem
-   Matthias Dieter Wallnöfer und Andrew Bartlett von „The Samba Team“ für den Hinweis auf ein in MS10-101 beschriebenes Problem
-   [HP](https://www.hp.com/) und [techit](https://www.techit.de/) für den Hinweis auf ein in MS10-102 beschriebenes Problem
-   Chaouki Bekrar vom [VUPEN Vulnerability Research Team](https://www.vupen.com/) für den Hinweis auf fünf in MS10-103 beschriebene Probleme
-   Oleksandr Mirosh in Zusammenarbeit mit [TippingPoints](https://www.tippingpoint.com/)[Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS10-104 beschriebenes Problem
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf zwei in MS10-105 beschriebene Probleme
-   Alin Rad Pop von [Secunia Research](https://secunia.com/) für den Hinweis auf ein in MS10-105 beschriebenes Problem
-   Carsten Eiram von [Secunia Research](https://secunia.com/) für den Hinweis auf drei in MS10-105 beschriebene Probleme
-   Dyon Balding von [Secunia Research](https://secunia.com/) für den Hinweis auf zwei in MS10-105 beschriebene Probleme
-   Oleksandr Mirosh in Zusammenarbeit mit [TippingPoints](https://www.tippingpoint.com/)[Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS10-106 beschriebenes Problem

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (14. Dezember 2010): Bulletin Summary veröffentlicht.
-   V1.1 (15. Dezember 2010): Es wird verdeutlicht, dass Benutzer von Microsoft Office XP und Microsoft Office 2003 das Update in MS10-087 installieren müssen, um vor den in MS10-105 beschriebenen Sicherheitsanfälligkeiten geschützt zu sein.

*Built at 2014-04-18T01:50:00Z-07:00*
