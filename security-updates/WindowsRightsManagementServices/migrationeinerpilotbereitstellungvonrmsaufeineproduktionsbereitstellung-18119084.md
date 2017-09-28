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
<td style="border:1px solid black;">Pilotprogramm</td>
<td style="border:1px solid black;">Sichern Sie die RMS-Konfigurationsdatenbank.</td>
<td style="border:1px solid black;">Dies ermöglicht Ihnen erforderlichenfalls die Wiederherstellung des Testservers.
In der Konfigurationsdatenbank ist der private Schlüssel von RMS enthalten.
Stellen Sie sicher, dass Sie das Kennwort für den privaten Schlüssel kennen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pilotprogramm</td>
<td style="border:1px solid black;">Wenn Sie zum Schutz des privaten Schlüssels von RMS ein Hardwaresicherheitsmodul (HSM) verwendet haben, sichern Sie die Konfiguration des HSM gemäß den Anweisungen des Herstellers.</td>
<td style="border:1px solid black;">Das HSM wird auf dem neuen Server wiederhergestellt.
Stellen Sie sicher, dass Ihnen sämtliche notwendigen Komponenten zur Installation und Konfiguration des HSM zur Verfügung stehen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Pilotprogramm</td>
<td style="border:1px solid black;">Exportieren Sie die Datei für die vertrauenswürdige Veröffentlichungsdomäne.</td>
<td style="border:1px solid black;">Dadurch kann ein anderer RMS-Server die auf diesem Server erstellten Veröffentlichungslizenzen entschlüsseln und Nutzungslizenzen für den geschützten Inhalt ausstellen.
Die vertrauenswürdige Veröffentlichungsdomäne enthält das Server-Lizenzgeberzertifikat, den privaten Schlüssel für RMS sowie alle Benutzerrechterichtlinien, die auf dem Server erstellt wurden.
Bei der Datei für die vertrauenswürdige Veröffentlichungsdomäne handelt es sich um eine XML-Datei, die durch ein sicheres Kennwort verschlüsselt wird, das beim Erstellen der Datei festgelegt wird. Sie müssen also dieses Kennwort wissen, um die Datei für die vertrauenswürdige Veröffentlichungsdomäne importieren zu können.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pilotprogramm</td>
<td style="border:1px solid black;">Exportieren Sie vertrauenswürdige Benutzerdomänen.</td>
<td style="border:1px solid black;">Dadurch kann ein anderer RMS-Server Nutzungslizenzen an Benutzer gewähren, die Rechtekontozertifikate (RACs) vom Testserver erhalten haben.
Die vertrauenswürdige Benutzerdomäne wird erstellt, indem das Server-Lizenzgeberzertifikat dieses Servers auf den anderen RMS-Server importiert wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Bereiten Sie den neuen Server als Stammzertifizierungsserver vor.</td>
<td style="border:1px solid black;">Stellen Sie sicher, dass der Zugriff auf den Datenbankserver ermöglicht wird und dass IIS und Message Queuing installiert sind.
Verwenden Sie, falls möglich, denselben Servernamen für diesen Server.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Wenn Sie ein HSM verwenden, installieren Sie das HSM und stellen Sie die Konfiguration aus der auf dem Pilotserver erstellten Sicherung wieder her.</td>
<td style="border:1px solid black;">Richtet die für die Verschlüsselung des privaten Schlüssels für RMS erforderlichen Anmeldeinformationen ein.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Installieren Sie RMS.</td>
<td style="border:1px solid black;">RMS überprüft, ob alle vorausgesetzten Dienste ordnungsgemäß installiert und konfiguriert sind.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Stellen Sie RMS mit einem neuen privaten Schlüssel bereit. Wenn Sie die Onlineregistrierung verwenden, wird der Server während des Bereitstellungsprozesses über eine Internetverbindung mit dem Microsoft-Registrierungsdienst registriert. Wenn Sie keine Internetverbindung auf diesem Server herstellen können, müssen Sie die Offlineregistrierung verwenden.</td>
<td style="border:1px solid black;">Unterscheidet sich dieser Servername vom Namen des Testservers, können Sie die Cluster-URL-Einstellung dahingehend ändern, dass Sie mit dem URL des Testservers identisch ist.
Falls dies nicht erfolgt, müssen Sie eine URL-Umleitung vom vorherigen Cluster-URL auf den neuen URL vornehmen, um Benutzern mit bereits bestehendem Inhalt den Erwerb von Nutzungslizenzen zu ermöglichen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Wenn Sie die Offlineregistrierung vornehmen, dann schließen Sie zunächst die manuelle Registrierung des neuen RMS-Servers ab. Weitere Informationen erhalten Sie unter „So registrieren Sie einen Stammzertifizierungsserver manuell“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.</td>
<td style="border:1px solid black;">Der RMS-Server kann erst nach seiner Registrierung verwendet werden.
Außerdem können Sie erst nach erfolgter Registrierung des Servers auf die RMS-Verwaltungsseiten zugreifen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Importieren Sie die Datei für die vertrauenswürdige Veröffentlichungsdomäne, die Sie in Schritt 3 exportiert haben.</td>
<td style="border:1px solid black;">Zum erfolgreichen Import der Datei muss das RMS-Dienstkonto Lesezugriff auf den Speicherort der Datei aufweisen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Signieren Sie die einzelnen Vorlagen erneut, die mit der vertrauenswürdigen Veröffentlichungsdomäne importiert wurden.</td>
<td style="border:1px solid black;">Die Vorlagen werden mit dem privaten Schlüssel für den Server signiert. Aufgrund des neuen privaten Schlüssels für den Server müssen die Vorlagen erneut signiert werden, damit sie gültig sind. Weitere Informationen finden Sie unter „So signieren Sie eine Vorlage für Benutzerrechterichtlinien erneut“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Verteilen Sie die Vorlagen erneut an die Clientcomputer, die am Pilotprojekt beteiligt waren.</td>
<td style="border:1px solid black;">Die alten Vorlagen müssen entfernt und durch die von diesem Server signierten Vorlagen ersetzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Produktion</td>
<td style="border:1px solid black;">Importieren Sie die Datei für die vertrauenswürdige Benutzerdomäne, die Sie in Schritt 4 exportiert haben.</td>
<td style="border:1px solid black;">Dadurch können auch alte Client-Lizenzgeberzertifikate und Rechtekontozertifikate verwendet werden.
Wenn Benutzerkonten als Teil dieser Migration innerhalb der Gesamtstrukturen verschoben werden, bedenken Sie bitte, dass die Konten entsprechende SMTP-Proxys aufweisen müssen.</td>
</tr>
</tbody>
</table>
 

Nach erfolgreicher Einrichtung des Produktionsservers überprüfen Sie, ob die Testbenutzer weiterhin zuvor geschützte Nachrichten lesen, sowie neue erstellen können. Sie können dann beliebig viele RMS-Server zum Cluster hinzufügen, um die Anzahl der Benutzer in Ihrer Organisation zu unterstützen.
