---
TOCTitle: Ermitteln der Zugriffsanforderungen
Title: Ermitteln der Zugriffsanforderungen
ms:assetid: 'eb2ce9a5-0430-4811-bd40-4a94a84426a8'
ms:contentKeyID: 18119086
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747790(v=WS.10)'
---

Ermitteln der Zugriffsanforderungen
===================================

In diesem Stadium der Planungsphase sollten Sie den Umfang Ihrer RMS-Implementierung bereits bestimmt haben. Wenn Sie die Sicherheit Ihres RMS-Systems bewerten, sollten Sie Methoden in Betracht ziehen, mit denen Sie den Umfang auf genau diese Teilnehmer einschränken und dabei sicherstellen können, dass die Daten, die die Teilnehmer mit RMS schützen, auch mithilfe bewährter Datensicherheitsverfahren geschützt werden. Des Weiteren sollten Sie sicherstellen, dass der Zugriff auf den RMS-Server zu Verwaltungs- und Konfigurationszwecken ausschließlich den vertrauenswürdigen Administratoren vorbehalten bleibt. Bei RMS stehen die folgenden Methoden für die Zugriffssicherheit zur Auswahl:

-   **Zugriffssteuerungslisten (Access Control Lists, ACLs)**. Alle RMS-Webdienste sowie die Verwaltungswebsite können mithilfe von ACLs geschützt werden. Um sicherzustellen, dass nur entsprechend befugte Benutzer den RMS-Dienst verwenden, können Sie Zugriffssteuerungslisten einsetzen und damit die Möglichkeiten der Benutzer zum Aufbauen einer Verbindung zu den RMS-Zertifizierungs- und -Lizenzierungsdiensten einschränken. Diese Vorgehensweise eignet sich insbesondere dann, wenn nur bestimmte Gruppen geschützte Inhalte erstellen oder eine Lizenz für geschützte Inhalte erhalten sollen.
-   **Clientauthentifizierung**. Sie können festlegen, dass Smartcards oder andere Formen der Clientauthentifizierung notwendig sein sollen, wenn ein Benutzer versucht, eine Nutzungslizenz oder ein Zertifikat abzurufen. So wird das Risiko verringert, dass ein unbefugter Benutzer Inhalte in der Sitzung eines befugten Benutzers öffnet.
-   **SSL (Secure Sockets Layer)**. Als zusätzlichen Schutz können Sie angeben, dass eine SSL-Verbindung zwischen den RMS-Clients und dem RMS-Server erforderlich ist. Sie sollten SSL aktivieren und die 128-Bit-Verschlüsselung für alle Dateien der RMS-Webdienste anfordern. Diese Dateien besitzen die Dateinamenerweiterung ASMX und befinden sich in den virtuellen Verzeichnissen „Licensing“, „Certification“ und „Admin“. Um die **RMS-Verwaltungswebseiten** über einen Browser auf einem Remotecomputer öffnen zu können, müssen Sie SSL aktivieren. Selbst wenn SSL aktiviert wurde, ist es nicht möglich, die Seite **Globale Verwaltung** von einem Remotecomputer aus zu öffnen.
    Weitere Informationen zum Konfigurieren von SSL auf Servern finden Sie in der Hilfe zu IIS.

Einige Unternehmen benötigen ein Abteilungslizenzierungssystem, das abgesichert und von anderen Abteilungen vollkommen getrennt ist. In einem solchen Szenario können Sie die Informationsrechte-Verwaltungsrichtlinien mit einem RMS-Server einrichten. Falls in einer Abteilung oder einem anderen Teilbereich Ihres Unternehmens äußerst vertrauliche Daten anfallen, sollten Sie das Einrichten eines separaten Lizenzierungsservers oder Lizenzierungsclusters in Erwägung ziehen, um so die Lizenzierung und Veröffentlichung der Inhalte vom Rest des Unternehmens getrennt zu halten. Hierzu wird ein Lizenzierungsserver beim Stammzertifizierungsserver (oder -cluster) unterregistriert, der die Zertifizierung und andere Dienste für die einzelnen Lizenzierungsserver übernimmt. Lizenzierungsserver stellen jedoch ihre eigenen Lizenzierungs- und Veröffentlichungsdienste bereit.

Benutzerkonten, Zugriffssteuerungslisten und die physische Sicherheit sind kritische Aspekte der Bereitstellung. Bevor Sie RMS in einer Produktionsumgebung implementieren, sollten Sie zunächst alle geeigneten Sicherheitsverfahren sowie Ihr derzeitiges Sicherheitsmodell untersuchen und implementieren.
