---
TOCTitle: 'Sperren von Server-Lizenzgeberzertifikaten'
Title: 'Sperren von Server-Lizenzgeberzertifikaten'
ms:assetid: '8020861d-d196-4431-8282-044675ef5616'
ms:contentKeyID: 18118919
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747578(v=WS.10)'
---

Sperren von Server-Lizenzgeberzertifikaten
==========================================

Eine Organisation muss ein Server-Lizenzgeberzertifikat möglicherweise aufgrund unvorhersehbarer Umstände sperren, die den RMS-Server gefährden können. Bei einem privaten Schlüssel, der nicht in einem Hardwaresicherheitsmodul gespeichert wurde, besteht ein höheres Diebstahlrisiko. Ein Server-Lizenzgeberzertifikat und ein Schlüssel können in einer Organisation von einem Eindringling, der die Kontrolle über den Server übernommen hat, oder von einem verärgerten Mitarbeiter, der das Zertifikat oder den Schlüssel kopiert oder entfernt hat, gefährdet werden. Die Sperrung ist eine Möglichkeit, den verursachten Schaden und den Missbrauch durch einen unberechtigten Benutzer in Grenzen zu halten.

Standardmäßig können Lizenzen oder Zertifikate von dem ausstellenden Prinzipal gesperrt werden. Da RMS-Server die den geschützten Inhalten zugeordneten Lizenzen und Zertifikate ausstellen, können Sie diese bei Bedarf jederzeit sperren. Wenn ein Lizenzierungsserver gefährdet wird, können Sie sein Server-Lizenzgeberzertifikat sperren. Dabei werden alle von diesem Server ausgestellten Zertifikate und Lizenzen ungültig. Anweisungen zum Sperren von Lizenzen und Zertifikaten finden Sie nachstehend unter [Implementieren der Sperrung](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a).

Der Stammzertifizierungscluster stellt allerdings einen Sonderfall dar. Das Server-Lizenzgeberzertifikat des Stammzertifizierungsclusters wird vom Microsoft-Registrierungsdienst ausgestellt, und standardmäßig kann nur der Microsoft-Registrierungsdienst dieses Server-Lizenzgeberzertifikat sperren.

Microsoft kann das Server-Lizenzgeberzertifikat eines Stammzertifizierungsservers nur aufgrund einer gerichtlichen Anordnung sperren. Der öffentliche Schlüssel des Servers muss dem Gericht zur Verfügung gestellt werden. Nachdem das Gericht Microsoft über den Antrag auf Sperrung benachrichtigt hat, gibt Microsoft das Server-Lizenzgeberzertifikat über den öffentlichen Schlüssel in seiner Sperrliste an. Diese Liste wird veröffentlicht. Sie können einen Antrag auf Sperrung bei Gericht nur anfordern, wenn eine der folgenden Bedingungen für den Server gilt, dessen Lizenz gesperrt werden soll:

-   Der Server befindet sich in Ihrem Besitz, und der private Schlüssel ist gefährdet.
-   Die veröffentlichten Inhalte befinden sich in Ihrem Besitz, und diese Inhalte werden unter Verletzung Ihres Copyrights veröffentlicht.

Befolgen Sie die zuvor in diesem Abschnitt unter [Bereitstellen von Sperrlisten](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4) von Microsoft beschriebenen Schritte zum Erwerben und Verteilen einer Microsoft-Sperrliste, die das gesperrte Server-Lizenzgeberzertifikat eines Stammzertifizierungsservers einschließt.

Beim Bereistellen des Stammzertifizierungsservers können Sie einen öffentlichen Schlüssel angeben, der zum Sperren des Server-Lizenzgeberzertifikats des Stammzertifizierungsclusters autorisiert ist. Dieser öffentliche Schlüssel kann im Besitz der Organisation oder eines Drittanbieters sein. Eine mit dem zugehörigen privaten Schlüssel signierte Sperrliste kann das Server-Lizenzgeberzertifikat sperren.

Zum Sperren des Server-Lizenzgeberzertifikats des Stammzertifizierungsservers können Sie eine Sperrliste erstellen, die dieses Server-Lizenzgeberzertifikat angibt. Dann können Sie es mit dem privaten Schlüssel Ihrer Organisation oder des Drittanbieters signieren und die Sperrliste an alle Benutzer verteilen. Weitere Informationen hierzu finden Sie oben unter [Bereitstellen von Sperrlisten](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4) im Abschnitt „Bereitstellen von Sperrlisten einer Organisation“.

Sie können ein Server-Lizenzgeberzertifikat in einer Sperrliste mithilfe der folgenden Parameter sperren:

-   **GUID**. Ein Server-Lizenzgeberzertifikat kann von seiner GUID (Globally Unique Identifier) gesperrt werden. Weitere Informationen zum Verwenden dieses Parameters in einer Sperrliste finden Sie oben unter [Erstellen von Sperrlisten](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a) im Abschnitt „Sperren von Zertifikaten und Lizenzen mithilfe der GUID“.
-   **Hashwert**. Ein Server-Lizenzgeberzertifikat kann basierend auf einem SHA-1-Hash der im Körper des Zertifikats enthaltenen Unicode-Zeichen gesperrt werden. Weitere Informationen zum Verwenden dieses Parameters in einer Sperrliste finden Sie oben unter [Erstellen von Sperrlisten](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a) im Abschnitt „Sperren von Zertifikaten und Lizenzen mithilfe des Hashwerts“.

Sie müssen die RMS-Konfigurationsdatenbank abfragen, um das Server-Lizenzgeberzertifikat einer RMS-Installation zu erhalten. Die folgenden Schritte beschreiben, wie Sie diese Informationen von einer SQL-Konfigurationsdatenbank erhalten und sie in einer Datei speichern, die mit einem Browser gelesen werden kann:

1.  Öffnen Sie SQL Query Analyzer, und stellen Sie dann eine Verbindung zur Konfigurationsdatenbank des Stammzertifizierungsservers her.
2.  Klicken Sie im Menü **Abfrage** auf **Ergebnisse in Text**.
3.  Klicken Sie im Menü **Extras** auf **Optionen**, um das Dialogfeld **Optionen** zu öffnen. Klicken Sie auf die Registerkarte **Ergebnisse**, und legen Sie dann für **Maximale Zeichenanzahl pro Spalte** den Wert **8192** fest.
        ```
1.  Kopieren Sie die Ergebnisse aus dem Fenster **Ergebnisse**, und fügen Sie diese Ergebnisse in einen Text-Editor ein, wie z. B. Editor. Speichern Sie die Ergebnisse in einer Datei mit der Dateinamenerweiterung \*.xml.

Weitere Informationen zum Verwenden dieser Informationen in einer Sperrliste finden Sie oben unter [Erstellen von Sperrlisten](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a).

Sobald Sie die Informationen zum Server-Lizenzgeberzertifikat als XML-Datei gespeichert haben, kann der öffentliche Schlüssel mithilfe der folgenden Schritte extrahiert werden:

1.  Öffnen Sie die XM-Datei für das Server-Lizenzgeberzertifikat in einem XML- oder Text-Editor.
2.  Kopieren Sie das Element &lt;PUBLICKEY&gt; in den Abschnitt &lt;ISSUEDPRINCIPALS&gt;.
3.  Speichern Sie diese Informationen in einer Datei, die Sie dem Gericht zusenden können, oder speichern Sie die Informationen in einer Organisationssperrliste.

Nachdem das Server-Lizenzgeberzertifikat des Stammzertifizierungsclusters gesperrt wurde, werden alle von der RMS-Installation ausgestellten Zertifikate und Lizenzen für die Inhalte ungültig, die eine Sperrliste erfordern. Die Inhalte sind nicht mehr verfügbar. Der Prozess ist unabhängig vom Typ der Benutzerlizenz. Sie müssen vor dem Implementieren der Sperrliste eine der folgenden Aktionen ausführen, um Inhalte beizubehalten, die vom Server veröffentlicht wurden, dessen Lizenz gesperrt wurde:

-   Speichern der Inhalte ohne RMS-Schutz.
-   Erneutes Veröffentlichen des Inhalts ohne eine Sperrlistenanforderung.

In beiden Szenarien – Sperrung durch Microsoft oder Sperrung durch einen Drittanbieter – tritt die Sperrliste für alle Bindungsanforderungen in Kraft, da sie vom privaten Schlüssel eines Prinzipals in der Vertrauenskette der Nutzungslizenz signiert wurde. Daher schlagen alle Bindungsanforderungen fehl, bei denen Lizenzen verwendet werden, die mithilfe des gesperrten Server-Lizenzgeberzertifikats von der RMS-Installation ausgestellt wurden.

| ![](images/Cc747578.note(WS.10).gif)Hinweis            |
|-------------------------------------------------------------------------------------|
| Microsoft sperrt ein Server-Lizenzgeberzertifikat nur auf Anordnung eines Gerichts. |