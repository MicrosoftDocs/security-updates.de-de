---
TOCTitle: Bereitstellen von Sperrlisten
Title: Bereitstellen von Sperrlisten
ms:assetid: 'e331338b-66d4-45e4-8d3f-acccf2302ac4'
ms:contentKeyID: 18119049
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747702(v=WS.10)'
---

Bereitstellen von Sperrlisten
=============================

Zum Implementieren der Sperrung müssen Sie Sperrlisten bereitstellen. Sperrlisten geben die Inhalte, Anwendungen, Benutzer oder anderen Prinzipale an, die gesperrt wurden. Sie können sowohl Sperrlisten einer Organisation als auch Sperrlisten von Microsoft bereitstellen.

Bereitstellen von Sperrlisten einer Organisation
------------------------------------------------

Sie müssen Clientcomputern in der Organisation die Sperrliste zur Verfügung stellen, um eine Vorlage für Benutzerrechterichtlinien zu verwenden. Weitere Informationen zum Erstellen von Sperrlisten finden Sie oben unter „Implementieren der Sperrung“.

Sie können eine Sperrliste einer Organisation mithilfe der folgenden Schritten bereitstellen:

1.  Kopieren Sie die Sperrlistendatei auf einen Webserver mit öffentlichem Zugriff. Da Benutzer die geschützten Inhalte möglicherweise außerhalb der Organisation abrufen, müssen alle Benutzer sowohl innerhalb als auch außerhalb des Netzwerks Zugriff auf den angegebenen Speicherort haben.
    Das Verteilen der Sperrlistendatei an Clientcomputer ist u. U. relativ zeitaufwändig. Daher ist es möglich, dass Benutzern die Sperrliste nicht auf dem Computer zur Verfügung stehen, wenn sie versuchen, ein Dokument zu öffnen, für das eine Sperrliste erforderlich ist. Fehlt die Sperrliste auf dem Clientcomputer, kann die RMS-fähige Anwendung sie von dem in der Nutzungslizenz angegebenen Speicherort downloaden.
    Es empfiehlt sich, ein Skript zu erstellen, das die Sperrliste automatisch signiert und täglich auf die Website kopiert. Damit können Sie sicherstellen, dass das Abrufen von Inhalten nicht verhindert wird, weil die Sperrliste der Benutzer abgelaufen ist. Ein Beispielskript hierzu finden Sie oben unter „Verwenden des Tools zum Signieren von Sperrlisten“.
2.  Geben Sie in der Vorlage für Benutzerrechterichtlinien für die Sperrliste einer Organisation ein Aktualisierungsintervall an, das größer als Null ist. Damit wird sichergestellt, dass die Sperrliste nicht optional ist. Wenn Sie die Liste nur selten aktualisieren, z. B. im Fall einer Sicherheitsverletzung, können Sie für die Aktualisierungsbedingung ein langes Intervall festlegen. Sie können dann den Skript- oder Richtlinieneinstellungen das Verteilen der Sperrliste an die Clientcomputer bei Bedarf überlassen. Weitere Informationen zum Festlegen von Aktualisierungsintervallen finden Sie oben unter „Definieren von Sperrrichtlinien“. Weitere Informationen zum Konfigurieren von Vorlagen für Benutzerrechterichtlinien finden Sie nachstehend unter „Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien“.
3.  Geben Sie in der Vorlage für Benutzerrechterichtlinien den URL an, an dem die Sperrliste verfügbar ist.
4.  Stellen Sie die Sperrliste wahlweise mithilfe einer automatisierten Methode, wie Gruppenrichtlinie oder Systems Management Server (SMS), auf Clientcomputern bereit.

Bereitstellen von Sperrlisten von Microsoft
-------------------------------------------

Damit der RMS-Client (Rights Management oder Rechteverwaltung) eine Sperrliste von Microsoft verwendet, müssen Sie die Liste auf den Clientcomputern bereitstellen. In diesem Thema wird die Bereitstellung einer Sperrliste von Microsoft in den folgenden Szenarien beschrieben:

-   Eine Organisation möchte eine eigene Sperrliste und die Sperrliste von Microsoft bereitstellen.
-   Eine Organisation möchte nur die Sperrliste von Microsoft bereitstellen.

Wenn eine Sperrliste von Microsoft veröffentlicht wird, können Sie sie von folgenden Speicherorten downloaden:

-   Server mit RMS können die Sperrliste mithilfe von Windows Update downloaden.
-   Die Sperrliste von Microsoft kann zudem vom Microsoft Download Center gedownloadet werden, wenn vom Server mit RMS keine Internet-Verbindung hergestellt werden kann.

Das auf einen Server mit RMS gedownloadete Sperrlistenpaket wird im Ordner %systemdrive%\\Program Files\\Windows Rights Management Services Revocation List gespeichert. Wenn Sie das Sperrlistenpaket auf einen anderen Computertyp downloaden, können Sie den Downloadpfad auswählen. Das Paket enthält die ausführbare Datei CRL\_Update.exe, die Sie zum Installieren der Clientsperrlisten im Clientlizenzspeicher ausführen können. Außerdem enthält es die Sperrlistendatei Msrl.xml, die Sie auf eine Website oder in einen freigegebenen Ordner kopieren können.

**So stellen Sie die Sperrliste Ihrer Organisation und die Sperrliste von Microsoft bereit**
1.  Folgen Sie den oben angeführten Anweisungen unter [Bereitstellen von Sperrlisten](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4), wenn Sie die Sperrliste einer Organisation bereitstellen möchten.

2.  Downloaden Sie das Microsoft-Sperrlistenpaket, und stellen Sie es mithilfe einer Methode, wie Gruppenrichtlinie oder Systems Management Server (SMS), auf allen Clientcomputern in der Organisation bereit. Sie können stattdessen auch Einträge in der Microsoft-Sperrliste in die Sperrliste einer Organisation kopieren und nur die Sperrliste der Organisation bereitstellen.

| ![](images/Cc747702.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft ist ein Prinzipal in einer Vertrauenskette aller von RMS ausgestellten Zertifikate und Lizenzen. Daher tritt eine von Microsoft ausgestellte Sperrliste für alle Bindungsanforderungen in Kraft, für die die Nutzungslizenz basierend auf einer Vorlage für Benutzerrechterichtlinien erworben wird, die die Sperrliste einer Organisation erfordert. Darüber hinaus wird die Microsoft-Sperrliste auf dem Clientcomputer registriert. |

**So stellen Sie nur eine Microsoft-Sperrliste bereit**
1.  Downloaden Sie das Microsoft-Sperrlistenpaket.

2.  Ändern Sie vorhandene Vorlagen für Benutzerrechterichtlinien so, dass die Sperrung erforderlich ist. Gibt es keine Vorlagen für Benutzerrechterichtlinien, erstellen Sie stattdessen eine Vorlage, für die die Sperrung erforderlich ist. Verwenden Sie beim Angeben der Sperrbedingung den öffentlichen Schlüssel von Microsoft.

3.  Legen Sie für das Aktualisierungsintervall einen sehr hohen Wert fest, z. B. 50.000. Dieser hohe Wert stellt sicher, dass die von Microsoft veröffentlichte Sperrliste nie abläuft. Aus diesem Grund ist für die von Ihnen verteilten Nutzungslizenzen keine neue Version der Microsoft-Sperrliste erforderlich, wenn ein solche möglicherweise nicht verfügbar ist.

4.  Kopieren Sie die Sperrlistendatei auf einen Webserver mit öffentlichem Zugriff. Da Benutzer die geschützten Inhalte möglicherweise außerhalb der Organisation abrufen, müssen alle Benutzer auf den angegebenen Speicherort Zugriff haben, d. h. sowohl innerhalb als auch außerhalb des Netzwerks.

5.  Sie müssen die Sperrliste zur Verfügung stellen, da das Verteilen der Sperrlistendatei an Clientcomputer u. U. ziemlich zeitaufwändig ist. Aus diesem Grund ist es möglich, dass einem Benutzer die Sperrliste nicht lokal auf seinem Computer zur Verfügung steht, wenn er versucht, ein Dokument mit einer Veröffentlichungslizenz zu öffnen, für die die Sperrung erforderlich ist. Fehlt die Sperrliste auf dem Clientcomputer, kann die RMS-fähige Anwendung sie von einem angegebenen Speicherort downloaden.

6.  Geben Sie in der Vorlage für Benutzerrechterichtlinien den URL an, an dem die Sperrliste verfügbar ist. Weitere Informationen zum Konfigurieren von Vorlagen für Benutzerrechterichtlinien finden Sie unter [Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).

7.  Stellen Sie das Sperrlistenpaket wahlweise mithilfe einer Methode, wie Gruppenrichtlinie oder Systems Management Server (SMS), auf Clientcomputern bereit. Benutzer können RMS-geschützte Inhalte, für die Sperrlisten erforderlich sind, in diesem Fall auch dann öffnen, wenn keine Verbindung zum Netzwerk besteht.