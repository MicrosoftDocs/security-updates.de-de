---
TOCTitle: Einrichten eines Domänencontrollers und Datenbankservers
Title: Einrichten eines Domänencontrollers und Datenbankservers
ms:assetid: 'd20f8305-9f9e-4760-bfbf-82824db60d1f'
ms:contentKeyID: 18119036
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747681(v=WS.10)'
---

Einrichten eines Domänencontrollers und Datenbankservers
========================================================

Vor der Installation eines Stammzertifizierungs- oder Lizenzierungsservers müssen Sie sicherstellen, dass Sie die entsprechende Domänen- und Datenbankunterstützung implementiert haben, indem Sie Active Directory und einen Datenbankserver wie etwa SQL Server 2000 mit Service Pack 3 (SP3) oder Microsoft® SQL Server 2000 Desktop Engine (MSDE 2000) Release A verwenden. Selbst wenn die erforderlichen Komponenten in Ihrer Produktionsumgebung bereits ausgeführt werden, sollten Sie Ihre Produktionsumgebung nicht zum Testen einsetzen.

Mithilfe der folgenden Verfahren werden ein Domänencontroller und ein Datenbankserver auf einem einzelnen Computer in einem isolierten Netzwerk zu serverseitigen Testzwecken eingerichtet.

| ![](images/Cc747681.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| In diesem Beispiel wird der Datenbankserver auf dem Domänencontroller ausgeführt. In einer Produktionsumgebung wird im Allgemeinen davon abgeraten, den Domänencontroller als Host für sonstige Komponenten zu verwenden. Active Directory und der Datenbankserver werden in diesem Beispiel auf demselben Computer ausgeführt, um die Installation der vollständigen Infrastruktur auf einer möglichst geringen Anzahl an Computern zu ermöglichen. |

Wenn Sie sich für MSDE 2000 als Datenbankserver entscheiden, sollten Sie berücksichtigen, dass MSDE 2000 keine Netzwerkschnittstellen unterstützt und in den Nutzungsbedingungen für MSDE 2000 angegeben ist, dass SQL Server-Clienttools nicht zur Bearbeitung einer MSDE 2000-Datenbank verwendet werden können. Aufgrund dieser Einschränkung können Sie weder Protokollierungsinformationen anzeigen lassen noch in der Konfigurationsdatenbank gespeicherte Daten ändern. MSDE 2000 sollte deshalb nur zur Unterstützung von RMS-Datenbanken in Testumgebungen verwendet werden.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Infrastrukturkomponente</th>
<th>Schritte zum Einrichten eines Domänencontrollers und Datenbankservers</th>
<th>Hinweise für die Bereitstellung in einer Produktionsumgebung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Betriebssystem</p></td>
<td style="border:1px solid black;"><p>Installieren Sie auf einem Computer, der den RMS-Hardwareanforderungen entspricht, aber noch nicht mit einem Netzwerk verbunden ist, Windows 2000 Server mit SP3 oder später bzw. Windows Server 2003. Verwenden Sie das NTFS-Dateisystem für die Partition.</p></td>
<td style="border:1px solid black;"><p>Sie sollten unbedingt immer die aktuellsten Service Packs und Aktualisierungen installieren. Verwenden Sie NTFS-formatierte Partitionen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Netzwerkverbindung</p></td>
<td style="border:1px solid black;"><p>Stellen Sie eine Verbindung mit dem Netzwerk her, die Internetkonnektivität gewährleistet, jedoch von der Produktionsumgebung isoliert ist.</p></td>
<td style="border:1px solid black;"><p>Die Internetverbindung muss über einen geeigneten Firewall versehen verfügen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>IP-Adresse</p></td>
<td style="border:1px solid black;"><p>Weisen Sie diesem Computer eine statische IP-Adresse zu.</p></td>
<td style="border:1px solid black;"><p>Verwenden Sie für Server immer statische IP-Adressen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Active Directory</p></td>
<td style="border:1px solid black;"><p>Melden Sie sich als lokaler Administrator an.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Klicken Sie auf <strong>Start</strong>, klicken Sie danach auf <strong>Ausführen</strong>, geben Sie in das Feld <code>Öffnen</code> die Codefolge <strong>dcpromo</strong> ein und klicken Sie danach auf <strong>OK</strong>.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Befolgen Sie nach dem Starten des Active Directory-Installationsassistenten die Anleitungen zur Erstellung einer neuen Domäne in einer neuen Gesamtstruktur, und nehmen Sie die Standardoptionen mit Ausnahme der Folgenden an:</p>
<p>Geben Sie den Domänennamen an, z. B. contoso.com.</p>
<p>Überlassen Sie die Konfiguration von DNS auf dem Computer dem Assistenten.</p>
<p>Wählen Sie <strong>Permissions compatible only with Windows 2000 servers (Nur mit Windows 2000-Servern kompatible Berechtigungen)</strong>, wenn alle Domänencontroller unter Windows 2000 oder später ausgeführt werden.</p>
<p>Geben Sie sichere Kennwörter für den lokalen Administrator an.</p></td>
<td style="border:1px solid black;"><p>Wenn für die Implementierung von RMS neue Domänen erforderlich sind, richten Sie diese in Active Directory ein.</p>
<p>Verwenden Sie für alle Konten immer sichere Kennwörter.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Starten Sie den Computer neu, wenn Sie dazu aufgefordert werden.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie die Funktionsebene folgendermaßen: Öffnen Sie das Snap-In <strong>Active Directory-Benutzer und -Computer</strong>, klicken Sie mit der rechten Maustaste auf den Domänennamen, klicken Sie auf <strong>Eigenschaften</strong>, und überprüfen Sie dann die Einstellung im Feld <strong>Betriebsmodus der Domäne</strong>. Klicken Sie auf <strong>Modus wechseln</strong>, damit die Domäne im <strong>einheitlichen Modus</strong> ausgeführt wird, wenn es keine Domänencontroller gibt, die älter als Windows 2000-Domänencontroller sind.</p>
<p>Anmerkungen: In Windows Server 2003 wird die Einstellung <strong>Betriebsmodus der Domäne</strong> durch <strong>Domänen-Funktionsebene</strong> ersetzt.</p></td>
<td style="border:1px solid black;"><p>Zum Zweck optimaler Sicherheit und Verwaltung sollten Sie die gemischte Funktionsebene von Windows 2000 nicht für die RMS-Unterstützung verwenden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Benutzerkonten</p></td>
<td style="border:1px solid black;"><p>Erstellen Sie ein Domänenbenutzerkonto zur Verwendung als RMS-Dienstkonto für RMS, wie etwa ContosoRMS@contoso.com. Legen Sie ein sicheres Kennwort fest. Geben Sie unbedingt eine E-Mail-Adresse für den Benutzer an. Wurde die E-Mail-Adresse nicht in Active Directory angegeben, kann der Benutzer keine Lizenzen und Zertifikate von RMS erhalten.</p>
<p>Anmerkungen: Das RMS-Dienstkonto darf nicht mit dem Domänenkonto identisch sein, das zum Installieren von RMS verwendet wurde.</p></td>
<td style="border:1px solid black;"><p>Sie sollten in Active Directory ein separates Konto erstellen, das vom RMS-Dienstkonto verwendet wird. Schließen Sie eine E-Mail-Adresse ein. Erteilen Sie dem Konto keine besonderen Berechtigungen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SQL Server 2000</p></td>
<td style="border:1px solid black;"><p>Melden Sie sich bei dem Server an, auf dem Sie die Datenbank zu installieren beabsichtigen. Ist dieser Server mit dem Domänencontroller identisch, müssen Sie sich als Domänenadministrator anmelden.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Befolgen Sie die mit der Datenbanksoftware gelieferten Anweisungen zum Installieren der Datenbankserver-Software</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Installieren Sie den Datenbankserver unter Rückgriff auf bewährte Methoden wie etwa:</p>
<ul>
<li>Geben Sie einen Namen für das Systemadministrator-Konto der Datenbank und einen Namen der Organisation, z. B. Contoso an.<br />
<br />
</li>
<li>Geben Sie ein sicheres Systemadministrator-Kennwort an.<br />
<br />
</li>
<li>Setzen Sie integrierte Methoden zur Windows-Authentifizierung ein.<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;"><p>Sie sollten einen integrierten Windows-Authentifizierungsmodus verwenden. Wenn Sie den Datenbankserver nicht in diesem Modus ausführen können, wenden Sie sich an Domänenadministrator und Datenbankserver-Administrator, um festzulegen, welche Änderungen bei der RMS-Einrichtung erforderlich sind.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Stellen Sie sicher, dass der Datenbankdienst beendet wurde.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Installieren Sie Software-Updates für den Datenbankserver. Wenn Sie zur Eingabe eines Kennworts aufgefordert werden, verwenden Sie dasselbe Kennwort, dass Sie bei der Installation festgelegt haben.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Starten Sie den Computer neu. Stellen Sie sicher, dass der Datenbankdienst gestartet wurde.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Stellen Sie sicher, dass Benutzerkonten gültige E-Mail-Adressenattribute in Active Directory aufweisen.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie, ob der Domänenbenutzer, der mit der Verwaltung von RMS und der Bereitstellung der Stammzertifizierungs- und Lizenzierungsserver beauftragt ist, über die erforderlichen Datenbankserver-Berechtigungen verfügt. Wenn SQL Server als Datenbankserver eingesetzt wird, können Sie eine Anmelde-ID für den Benutzer, der das Snap-In für den <strong>SQL Server Enterprise Manager</strong> verwendet, hinzufügen. Erweitern Sie im Snap-In den Server sowie die Servergruppe, und erweitern Sie danach das Element <strong>Sicherheit</strong>. Klicken Sie auf das Element <strong>Anmeldungen</strong>, fügen Sie eine neue Anmeldung für das Domänenkonto des Benutzers hinzu, klicken Sie auf die Registerkarte <strong>Serverrollen</strong> und aktivieren Sie danach das Kontrollkästchen <strong>Server-Administratoren</strong>.</p></td>
<td style="border:1px solid black;"><p>Wichtig: Sämtliche Benutzer und Gruppen, die RMS zum Erwerb von Lizenzen und Veröffentlichen von Inhalt verwenden, müssen im MMC-Snap-In Active Directory-Benutzer und Gruppen auf der Registerkarte <strong>Allgemein</strong> der <strong>Eigenschaften</strong> des Benutzers eine E-Mail-Adresse auf ihrem Konto konfiguriert haben.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Internetverbindung</p>
<p>(optional)</p></td>
<td style="border:1px solid black;"><p>Stellen Sie sicher, dass Browser und Server – einschließlich der erforderlichen Proxyservereinstellungen –, TCP/IP und LMHOSTS/HOSTS ordnungsgemäß konfiguriert sind, damit Sie auf das Internet zugreifen können. Testen Sie den Zugriff, indem Sie zu http://uddi.microsoft.com wechseln. Wenn Sie diese Seite öffnen können, kann RMS eine Verbindung mit dem Microsoft-Registrierungsdienst herstellen.</p></td>
<td style="border:1px solid black;"><p>Wechseln Sie zu http://uddi.microsoft.com, um den Internetzugriff zu überprüfen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Softwareupdates</p></td>
<td style="border:1px solid black;"><p>Laden Sie alle Aktualisierungen für die Software herunter, die auf diesem Computer installiert ist, und installieren Sie sie. Dies umfasst auch die neuesten Windows-Aktualisierungen von www.microsoft.com.</p></td>
<td style="border:1px solid black;"><p>Sie sollten jederzeit die neuesten Aktualisierungen herunterladen und installieren.</p></td>
</tr>
</tbody>
</table>
  
Wenn Sie die vorherigen Schritte ausgeführt haben, sind Sie für die Erstinstallation einschließlich der Installation der vorausgesetzten Software auf dem Computer bereit, auf dem RMS ausgeführt werden soll.
