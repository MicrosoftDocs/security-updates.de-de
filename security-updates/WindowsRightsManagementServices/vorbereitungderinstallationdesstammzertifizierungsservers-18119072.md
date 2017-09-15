---
TOCTitle: Vorbereitung der Installation des Stammzertifizierungsservers
Title: Vorbereitung der Installation des Stammzertifizierungsservers
ms:assetid: 'ed51605e-8b17-4155-8d83-f6777f499b7b'
ms:contentKeyID: 18119072
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747726(v=WS.10)'
---

Vorbereitung der Installation des Stammzertifizierungsservers
=============================================================

Im Testinstallationsbeispiel ist nur ein Stammzertifizierungsserver vorhanden. Sie können aber auch zusätzliche Server einrichten, und zwar entweder als Teil des Stammzertifizierungsclusters oder als separaten Lizenzierungsservercluster. Die Infrastruktur ist für alle derartigen Server identisch. Sie müssen also die in diesem Thema bereitgestellte Prozedur auf jedem dieser Server durchführen.

Sie müssen zunächst den Domänencontroller installieren und die Datenbankserver – gemäß den Anweisungen in den vorigen Abschnitten – einrichten. Nachdem Sie alle in der folgenden Tabelle angeführten Schritte abgeschlossen haben, können Sie mit der Installation von RMS beginnen.

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
<th>So bereiten Sie den Server für die RMS-Installation vor</th>
<th>Hinweise für die Bereitstellung in einer Produktionsumgebung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Betriebssystem</p></td>
<td style="border:1px solid black;"><p>Installieren Sie auf einem Computer, der den RMS-Hardwareanforderungen entspricht, aber noch nicht mit einem Netzwerk verbunden ist, das Windows Server 2003-Betriebssystem und verwenden Sie das NTFS-Dateisystem für die Partition.</p></td>
<td style="border:1px solid black;"><p>Sie sollten unbedingt immer die neuesten Service Packs und die neuesten Patches installieren. Verwenden Sie NTFS-formatierte Partitionen.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Internetverbindung</p>
<p>(optional)</p></td>
<td style="border:1px solid black;"><p>Stellen Sie eine Ethernet-Verbindung zu einem Netzwerk her, das Internetkonnektivität bereitstellt, jedoch von der Produktionsumgebung isoliert ist. Wenn Sie zur Registrierung des RMS-Servers die Onlineregistrierung als Teil des Bereitstellungsprozesses verwenden, muss der Server Internetkonnektivität aufweisen.</p></td>
<td style="border:1px solid black;"><p>Im Falle einer Onlineregistrierung müssen Sie sicherstellen, dass die Internetverbindung über eine entsprechende Firewall verfügt.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>IP-Adresse</p></td>
<td style="border:1px solid black;"><p>Weisen Sie diesem Computer eine statische IP-Adresse zu.</p></td>
<td style="border:1px solid black;"><p>Verwenden Sie für Server immer statische IP-Adressen.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Fügen Sie diesen Computer zur Domäne hinzu.</p></td>
<td style="border:1px solid black;"><p>Melden Sie sich als lokaler Administrator am Computer an. Klicken Sie auf <strong>Start</strong>, klicken Sie mit der rechten Maustaste auf <strong>Arbeitsplatz</strong>, klicken Sie auf <strong>Eigenschaften</strong>, klicken Sie auf die Registerkarte <strong>Computername</strong>, und klicken Sie dann auf <strong>Ändern</strong>.</p></td>
<td style="border:1px solid black;"><p>Verwenden Sie dieselbe Domäne für alle Server.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Behalten Sie den Computernamen bei, klicken Sie auf <strong>Domäne</strong>, geben Sie dann den Domänennamen ein, z. B. <strong>Contoso.com</strong>, und klicken Sie dann auf OK. Stellen Sie Benutzeranmeldeinformationen bereit, die Ihnen das Beitreten zu dieser Domäne ermöglichen. Klicken Sie auf <strong>OK</strong>, und starten Sie den Computer neu, wenn Sie dazu aufgefordert werden. Nachdem der Computer neu gestartet wurde und Sie zur Eingabe Ihrer Anmeldeinformationen aufgefordert worden sind, geben Sie die entsprechende Domäne, den Benutzernamen und das Kennwort an.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Benutzer und Anmeldung</p></td>
<td style="border:1px solid black;"><p>Klicken Sie mit der rechten Maustaste auf <strong>Arbeitsplatz</strong>, klicken Sie auf <strong>Verwalten</strong>, und erweitern Sie <strong>Lokale Benutzer und Gruppen</strong>. Klicken Sie auf <strong>Gruppen</strong>, und klicken Sie dann auf <strong>Administratoren</strong>.</p>
<p>Klicken Sie auf <strong>Hinzufügen</strong>, geben Sie den Namen des hinzuzufügenden Benutzerkontos an (z. B. <strong>Michael@contoso.com</strong>), und klicken Sie auf OK. Erteilen Sie dem Benutzerkonto Administratorrechte. Stellen Sie die entsprechenden Anmeldeinformationen bereit, wenn Sie dazu aufgefordert werden, z. B. Contoso\Administrator.</p>
<p>Melden Sie sich am Computer als Domänenbenutzer mit lokalen Administratorrechten an.</p></td>
<td style="border:1px solid black;"><p>Zum Hinzufügen von Komponenten zu diesem Computer sind Administratorrechte erforderlich. Einige Installationsschritte können mithilfe des lokalen Administratorkontos nicht vollständig ausgeführt werden. Auf diesem Server muss es mindestens einen Benutzer geben, der als Administrator fungiert. Darüber hinaus sind bei SQL Server zum Erstellen neuer Datenbanken Systemadministratorrechte erforderlich.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Internetverbindung</p>
<p>(optional)</p></td>
<td style="border:1px solid black;"><p>Wechseln Sie mit einem Internetbrowser zu http://uddi.microsoft.com/, um den Internetzugriff zu überprüfen. Auf Computern mit Windows Server 2003 müssen die Lmhosts- und Hosts-Dateien möglicherweise geändert werden, damit der Domänencontroller mit eingeschlossen wird.</p></td>
<td style="border:1px solid black;"><p>Wechseln Sie zu http://uddi.microsoft.com, um den Internetzugriff zu überprüfen.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Windows-Aktivierung</p></td>
<td style="border:1px solid black;"><p>Sie können die Aktivierung von Windows mithilfe des Aktivierungsassistenten unter Einsatz einer Internetverbindung in die Wege leiten, oder Windows telefonisch über Microsoft aktivieren. Weitere Informationen zur Aktivierung von Windows Server 2003-Produkten finden Sie im Hilfe- und Supportcenter für Windows Server 2003.</p></td>
<td style="border:1px solid black;"><p>Windows Server 2003 muss innerhalb von 14 Tagen nach der Installation aktiviert werden.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Softwareupdates</p></td>
<td style="border:1px solid black;"><p>Stellen Sie sicher, dass die neuesten Software-Aktualisierungen für die auf dem Computer befindliche Software installiert sind.</p></td>
<td style="border:1px solid black;"><p>Installieren Sie die neuesten Software-Aktualisierungen.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Konfigurieren Sie Internet Explorer.</p></td>
<td style="border:1px solid black;"><p>RMS verwendet für die Verwaltung eine Webschnittstelle. Aufgrund der standardmäßigen Sicherheitseinstellungen werden die Seiten möglicherweise nicht einwandfrei angezeigt. Manche Seiten der RMS-Verwaltungswebsite verwenden Popup-Fenster zur Konfiguration von Optionen.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>  
</tbody>  
</table>
  
Nachdem Sie alle nötigen Schritte auf beiden Servern ausgeführt haben, können Sie mit der Installation und Bereitstellung von RMS auf den Servern beginnen.
