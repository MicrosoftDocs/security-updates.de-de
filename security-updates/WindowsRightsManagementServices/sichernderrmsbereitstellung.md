---
TOCTitle: 'Sichern der RMS-Bereitstellung'
Title: 'Sichern der RMS-Bereitstellung'
ms:assetid: '6de8b636-a824-4844-aefc-f26347abfc14'
ms:contentKeyID: 18118882
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720291(v=WS.10)'
---

Sichern der RMS-Bereitstellung
==============================

Eine RMS-Bereitstellung ist ein Vermögenswert in einem Unternehmen, für den dieselben physischen und netzwerktechnischen Sicherheitsmaßnahmen notwendig sind wie für andere unternehmenswichtige Server in der Infrastruktur. Im Rahmen der Bereitstellung sollten Sie daher die Bedrohungen und die möglichen Gegenmaßnahmen für die RMS-Server ermitteln.

RMS wird als Webdienst implementiert, so dass Sie den Zugriff auf RMS auf dieselbe Weise wie bei anderen Webdiensten steuern können: mittels Zugriffssteuerungslisten und SSL (Secure Sockets Layer).

**Einschränken des Zugriffs auf RMS-Webdienste mit Zugriffssteuerungslisten (ACLs)**

Mithilfe von Zugriffssteuerungslisten (Access Control Lists, ACLs) können Sie den Zugriff auf die RMS-Dienste einschränken. Jedes der virtuellen Stammverzeichnisse, die beim Bereitstellen von RMS auf einer Website erstellt wurden, besitzt eine entsprechende Ordnerstruktur, die gesichert werden kann. Die Ordnerstruktur befindet sich standardmäßig unter &lt;Systemlaufwerk&gt;:\\&lt;*Web\_Stammverzeichnis*&gt;\\\_wmcs. *Web\_Stammverzeichnis* bezeichnet dabei den Ordner, der der Website zugeordnet ist, auf der Sie RMS bereitgestellt haben. Ein Teil der Webdienste, z. B. der Unterregistrierungsdienst, der Zertifizierungsdienst für mobile Geräte sowie der Serverdienst-Zertifizierungsdienst, ist standardmäßig eingeschränkt, und die Benutzer oder Benutzergruppen, die auf einen bestimmten Dienst zugreifen möchten, müssen explizit in die Zugriffssteuerungsliste eingetragen werden.

Der Serverdienst-Zertifizierungsdienst stellt Rechtekontozertifikate (RAC) bereit, die den Zugriff auf RMS-geschützte Inhalte über bestimmte Dienste ermöglichen (z. B. über Webzusammenarbeitsdienste, Mailserver oder Dokumentmanagement-Server) und so die Erweiterung eines RMS-Systems unterstützen:

-   Dokumentzusammenarbeitsserver, auf den die Benutzer ungeschützte Dokumente hochladen können; heruntergeladene Dokumente werden dagegen automatisch mit dem richtigen RMS-Schutz gemäß der Benutzerrechterichtlinien für den jeweiligen Inhaltstyp ausgestattet. Ein Beispiel dafür ist Microsoft Office SharePoint Server 2007.
-   Dokumentmanagement-System, das als allgemeines Repository und Archiv für geschützte und ungeschützte Dokumente fungiert. Es ist möglich, durch Berechtigungen geschützte Dokumente für Suchvorgänge zu indizieren und dabei gleichzeitig die durch den Ersteller der Inhalte definierte Benutzerrechterichtlinie unverändert beizubehalten.
-   Aktivieren Sie den Mailserver, so dass durch Berechtigungen geschützte Inhalte rasch geöffnet und auf Viren und Spam überprüft bzw. im Rahmen von rechtlichen Anforderungen oder von unternehmenseigenen E-Mail-Richtlinien untersucht werden können.

Da für diese Szenarien Lizenzen für die Benutzer erforderlich sind, sollten Sie darauf achten, dass nur die Server im Unternehmen RACs erhalten können, denen diese Funktion zugewiesen ist und die entsprechend gesichert sind.

**Einschränken des Zugriffs auf RMS-Webdienste mit SSL**

Sie sollten Secure Sockets Layer (SSL) aktivieren und die 128-Bit-Verschlüsselung für alle Dateien der RMS-Webdienste anfordern. Diese Dateien besitzen die Dateinamenerweiterung ASMX und befinden sich in den virtuellen Verzeichnissen „Licensing“, „Certification“ und „Admin“. Bei SSL muss auf dem Computer ein gültiges SSL-Zertifikat für die Website installiert sein. Wenn Sie SSL für den Ordner „\_wmcs“ der RMS-Installation anwenden, wird diese Einstellung für alle Unterordner und Dateien übernommen. Weitere Informationen zu Webdienstedateien und virtuellen Verzeichnissen finden Sie in dieser Dokumentationssammlung im Bereich „Technische Referenz für RMS“ unter „Internet Information Services“.

> [!NOTE]
> Beim Öffnen der Verwaltungswebseiten von Windows RMS mit einem Browser, der sich auf einem Remotecomputer befindet, müssen Sie SSL aktivieren. Selbst wenn SSL aktiviert wurde, ist es nicht möglich, die Seite **Globale Verwaltung** von einem Remotecomputer aus zu öffnen. Weitere Informationen zur Remoteverwaltung von RMS erhalten Sie in dieser Dokumentationssammlung im Bereich „Technische Referenz für RMS“ unter „Betreiben von RMS“. 

**Einstellen eines verstärkten privaten Kennwortschlüssels**

Das Kennwort für den privaten Schlüssel wird verwendet, um den privaten Schlüssel zu erstellen und sicher in der RMS-Konfigurationsdatenbank zu speichern. Ein verstärktes Kennwort wird empfohlen, damit maximale Sicherheit gewährleistet ist. Wenn Sie das Kennwort aufschreiben müssen, stellen Sie sicher, dass sie es an einem sicheren Ort aufbewahren.

| ![](images/Cc720291.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                   |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn das Kennwort für den privaten Schlüssel verloren geht oder vergessen wird und der RMS-Server unerwartet offline geht, müssen Sie alle RMS-Dokumente entschlüsseln, die RMS-Umgebung neu erstellen und alle Daten erneut mit einem neuen privaten Schlüssel verschlüsseln. |