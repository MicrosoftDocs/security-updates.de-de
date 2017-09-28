---
TOCTitle: Migration einer Pilotbereitstellung von RMS auf eine Produktionsbereitstellung
Title: Migration einer Pilotbereitstellung von RMS auf eine Produktionsbereitstellung
ms:assetid: 'ea151946-22fb-4cba-a3ef-fd7a4bf0d292'
ms:contentKeyID: 18119084
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747789(v=WS.10)'
---

Migration einer Pilotbereitstellung von RMS auf eine Produktionsbereitstellung
==============================================================================

Viele Organisationen entscheiden sich für die Bereitstellung von RMS in einer Testumgebung, bevor sie die Technologie auf die gesamte Organisation anwenden. Das Pilotprogramm umfasst in der Regel eine eingeschränkte Anzahl von Benutzern. Der Server wird üblicherweise lokal von einem Administrator verwaltet und ist nicht Teil eines von einer IT-Gruppe verwalteten Datenzentrums. Wenn die Organisation im Datenzentrum nach Abschluss des Pilotprogramms RMS für alle Clients umsetzt, werden neue Server zur Unterstützung einer größeren Anzahl möglicher Benutzer bereitgestellt.

RMS-geschützter Inhalt ist jedoch an den zur Erstellung des Inhalts verwendeten RMS-Server gebunden. Wenn also ein Server entfernt oder ersetzt wird, müssen Sie sicherstellen, dass der mit den RMS-Servern des Pilotprogramms verschlüsselte Inhalt mit den RMS-Servern der Produktionsumgebung entschlüsselt und lizenziert werden kann.

Wenn Sie RMS als Pilotprogramm bereitgestellt haben und den RMS-Server in der Produktionsumgebung Ihrer Organisation einsetzen und zudem die Integrität der mithilfe des Testservers von RMS geschützten Inhalte aufrechterhalten möchten, sollten Sie einen Migrationsplan aufstellen, durch den im Falle einer erforderlichen Wiederherstellung von Daten ein reibungsloser Übergang unter Rückgriff auf das Pilotprogramm sichergestellt werden soll.

Die folgenden Schritte dienen als Beispiel für einige der Punkte, die in Ihrem Migrationsplan nicht fehlen sollten. Zudem erfordert Ihre Bereitstellung möglicherweise noch zusätzliche Elemente.

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
<th>Server</th>
<th>Schritt</th>
<th>Anmerkungen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Pilotprogramm</p></td>
<td style="border:1px solid black;"><p>Sichern Sie die RMS-Konfigurationsdatenbank.</p></td>
<td style="border:1px solid black;"><p>Dies ermöglicht Ihnen erforderlichenfalls die Wiederherstellung des Testservers.</p>
<p>In der Konfigurationsdatenbank ist der private Schlüssel von RMS enthalten.</p>
<p>Stellen Sie sicher, dass Sie das Kennwort für den privaten Schlüssel kennen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Pilotprogramm</p></td>
<td style="border:1px solid black;"><p>Wenn Sie zum Schutz des privaten Schlüssels von RMS ein Hardwaresicherheitsmodul (HSM) verwendet haben, sichern Sie die Konfiguration des HSM gemäß den Anweisungen des Herstellers.</p></td>
<td style="border:1px solid black;"><p>Das HSM wird auf dem neuen Server wiederhergestellt.</p>
<p>Stellen Sie sicher, dass Ihnen sämtliche notwendigen Komponenten zur Installation und Konfiguration des HSM zur Verfügung stehen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Pilotprogramm</p></td>
<td style="border:1px solid black;"><p>Exportieren Sie die Datei für die vertrauenswürdige Veröffentlichungsdomäne.</p></td>
<td style="border:1px solid black;"><p>Dadurch kann ein anderer RMS-Server die auf diesem Server erstellten Veröffentlichungslizenzen entschlüsseln und Nutzungslizenzen für den geschützten Inhalt ausstellen.</p>
<p>Die vertrauenswürdige Veröffentlichungsdomäne enthält das Server-Lizenzgeberzertifikat, den privaten Schlüssel für RMS sowie alle Benutzerrechterichtlinien, die auf dem Server erstellt wurden.</p>
<p>Bei der Datei für die vertrauenswürdige Veröffentlichungsdomäne handelt es sich um eine XML-Datei, die durch ein sicheres Kennwort verschlüsselt wird, das beim Erstellen der Datei festgelegt wird. Sie müssen also dieses Kennwort wissen, um die Datei für die vertrauenswürdige Veröffentlichungsdomäne importieren zu können.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Pilotprogramm</p></td>
<td style="border:1px solid black;"><p>Exportieren Sie vertrauenswürdige Benutzerdomänen.</p></td>
<td style="border:1px solid black;"><p>Dadurch kann ein anderer RMS-Server Nutzungslizenzen an Benutzer gewähren, die Rechtekontozertifikate (RACs) vom Testserver erhalten haben.</p>
<p>Die vertrauenswürdige Benutzerdomäne wird erstellt, indem das Server-Lizenzgeberzertifikat dieses Servers auf den anderen RMS-Server importiert wird.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Bereiten Sie den neuen Server als Stammzertifizierungsserver vor.</p></td>
<td style="border:1px solid black;"><p>Stellen Sie sicher, dass der Zugriff auf den Datenbankserver ermöglicht wird und dass IIS und Message Queuing installiert sind.</p>
<p>Verwenden Sie, falls möglich, denselben Servernamen für diesen Server.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Wenn Sie ein HSM verwenden, installieren Sie das HSM und stellen Sie die Konfiguration aus der auf dem Pilotserver erstellten Sicherung wieder her.</p></td>
<td style="border:1px solid black;"><p>Richtet die für die Verschlüsselung des privaten Schlüssels für RMS erforderlichen Anmeldeinformationen ein.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Installieren Sie RMS.</p></td>
<td style="border:1px solid black;"><p>RMS überprüft, ob alle vorausgesetzten Dienste ordnungsgemäß installiert und konfiguriert sind.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Stellen Sie RMS mit einem neuen privaten Schlüssel bereit. Wenn Sie die Onlineregistrierung verwenden, wird der Server während des Bereitstellungsprozesses über eine Internetverbindung mit dem Microsoft-Registrierungsdienst registriert. Wenn Sie keine Internetverbindung auf diesem Server herstellen können, müssen Sie die Offlineregistrierung verwenden.</p></td>
<td style="border:1px solid black;"><p>Unterscheidet sich dieser Servername vom Namen des Testservers, können Sie die Cluster-URL-Einstellung dahingehend ändern, dass Sie mit dem URL des Testservers identisch ist.</p>
<p>Falls dies nicht erfolgt, müssen Sie eine URL-Umleitung vom vorherigen Cluster-URL auf den neuen URL vornehmen, um Benutzern mit bereits bestehendem Inhalt den Erwerb von Nutzungslizenzen zu ermöglichen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Wenn Sie die Offlineregistrierung vornehmen, dann schließen Sie zunächst die manuelle Registrierung des neuen RMS-Servers ab. Weitere Informationen erhalten Sie unter „So registrieren Sie einen Stammzertifizierungsserver manuell“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.</p></td>
<td style="border:1px solid black;"><p>Der RMS-Server kann erst nach seiner Registrierung verwendet werden.</p>
<p>Außerdem können Sie erst nach erfolgter Registrierung des Servers auf die RMS-Verwaltungsseiten zugreifen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Importieren Sie die Datei für die vertrauenswürdige Veröffentlichungsdomäne, die Sie in Schritt 3 exportiert haben.</p></td>
<td style="border:1px solid black;"><p>Zum erfolgreichen Import der Datei muss das RMS-Dienstkonto Lesezugriff auf den Speicherort der Datei aufweisen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Signieren Sie die einzelnen Vorlagen erneut, die mit der vertrauenswürdigen Veröffentlichungsdomäne importiert wurden.</p></td>
<td style="border:1px solid black;"><p>Die Vorlagen werden mit dem privaten Schlüssel für den Server signiert. Aufgrund des neuen privaten Schlüssels für den Server müssen die Vorlagen erneut signiert werden, damit sie gültig sind. Weitere Informationen finden Sie unter „So signieren Sie eine Vorlage für Benutzerrechterichtlinien erneut“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Verteilen Sie die Vorlagen erneut an die Clientcomputer, die am Pilotprojekt beteiligt waren.</p></td>
<td style="border:1px solid black;"><p>Die alten Vorlagen müssen entfernt und durch die von diesem Server signierten Vorlagen ersetzt werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Produktion</p></td>
<td style="border:1px solid black;"><p>Importieren Sie die Datei für die vertrauenswürdige Benutzerdomäne, die Sie in Schritt 4 exportiert haben.</p></td>
<td style="border:1px solid black;"><p>Dadurch können auch alte Client-Lizenzgeberzertifikate und Rechtekontozertifikate verwendet werden.</p>
<p>Wenn Benutzerkonten als Teil dieser Migration innerhalb der Gesamtstrukturen verschoben werden, bedenken Sie bitte, dass die Konten entsprechende SMTP-Proxys aufweisen müssen.</p></td>
</tr>
</tbody>
</table>
<p> </p>

Nach erfolgreicher Einrichtung des Produktionsservers überprüfen Sie, ob die Testbenutzer weiterhin zuvor geschützte Nachrichten lesen, sowie neue erstellen können. Sie können dann beliebig viele RMS-Server zum Cluster hinzufügen, um die Anzahl der Benutzer in Ihrer Organisation zu unterstützen.
