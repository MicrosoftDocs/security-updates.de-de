---
TOCTitle: So fügen Sie einen Server zu einem Cluster hinzu
Title: So fügen Sie einen Server zu einem Cluster hinzu
ms:assetid: 'db635238-5528-4bec-9cc6-8244e2b3d733'
ms:contentKeyID: 18119048
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747690(v=WS.10)'
---

So fügen Sie einen Server zu einem Cluster hinzu
================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Auf jedem Server können Sie RMS nur auf einer einzelnen Website bereitstellen. Wenn Sie RMS nicht auf der Standardwebsite bereitstellen möchten, fügen Sie die gewünschte Website mithilfe von IIS-Manager hinzu, bevor Sie diesen Bereitstellungsprozess starten. Wenn die Website, die Sie bereitstellen möchten, nicht in der Liste der Websites angezeigt wird, schließen Sie die Seite **Globale Verwaltung**, fügen Sie die Website hinzu, und starten Sie dann den Bereitstellungsprozess erneut.

Wenn Sie RMS in einer Umgebung bereitstellen, in der die Active Directory-Infrastruktur für die Verwendung des „Native Mode“ (einheitlicher Modus) von Windows 2000 eingestellt ist, kann RMS möglicherweise nicht das Attribut **memberOf** von Active Directory-Objekten lesen, wenn die Gruppenmitgliedschaft erweitert werden soll. Das RMS-Dienstkonto muss ein Konto auf Domänenebene verwenden, das ein Mitglied der vordefinierten Gruppe Prä-Windows 2000-kompatibler Zugriff in Ihrer Gesamtstruktur ist, um RMS das Lesen des Attributs **memberOf** zu ermöglichen.

Hinzufügen eines Servers zu einem Cluster
-----------------------------------------

#### So fügen Sie einen Server zu einem Cluster hinzu

1.  Nachdem Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) auf einem Server installiert haben, den Sie zu einem Stammzertifizierungs- oder Lizenzierungscluster hinzufügen möchten, öffnen Sie die Seite **Globale Verwaltung**.

2.  Klicken Sie neben der Website, auf der Sie RMS bereitstellen möchten, auf **Diesen Server zu einem Cluster hinzufügen**. Sie können die Standardwebsite oder eine andere Website auswählen, die Sie unter „Internetinformationsdienste“ (Internet Information Services oder IIS) zu diesem Zweck erstellt haben.

    | ![](images/Cc747690.Warning(WS.10).gif)Warnung                                                                                                                                                                                                                           |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Das Ausführen zusätzlicher Websites oder Dienste auf dem Server mit RMS wird nicht unterstützt. Dies könnte dazu führen, dass mehrere Anwendungen und Dienste unter demselben Konto wie RMS ausgeführt werden. Hierdurch würden die privaten Schlüssel in nicht vorgesehenen Operationen dargestellt. |

3.  Geben Sie im Bereich **RMS-Dienstkonto** den Kontonamen im Format Domänenname\\Benutzername sowie das Kennwort des RMS-Dienstkontos ein, das zur Ausführung von RMS-Standardoperationen verwendet wird. Hierbei muss es sich um ein Domänenkonto handeln. All Server in einem Cluster sollten unter demselben RMS-Dienstkonto ausgeführt werden.

    | ![](images/Cc747690.Important(WS.10).gif)Wichtig                                                                                                                                                                                           |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Sie sollten ein spezielles Domänenbenutzerkonto als RMS-Dienstkonto erstellen, dem keine besonderen Berechtigungen erteilt werden. Das RMS-Dienstkonto darf nicht mit dem Domänenkonto identisch sein, das zum Installieren von RMS mit Service Pack 1 verwendet wurde. |

4.  Geben Sie im Bereich **Konfigurationsdatenbank** den Namen des Datenbankservers und den Namen der Konfigurationsdatenbank für diesen Cluster an. Die Datenbank, die Sie auswählen, bestimmt den Cluster, zu dem dieser Server hinzugefügt wird.

5.  Wählen Sie im Bereich **Schutz durch privaten Schlüssel** den Mechanismus aus, der von diesem Cluster zum Schutz für den privaten Schlüssel verwendet wird. Stellen Sie für den standardmäßigen softwarebasierten Schutz des privaten Schlüssels das Kennwort zur Verfügung, das zum Verschlüsseln des privaten Schlüssels bei der Bereitstellung des ersten Servers in diesem Cluster verwendet wurde.

6.  Klicken Sie auf **Absenden**.

    Schließen Sie die Seite nicht, wenn Fehlermeldungen angezeigt werden. Beheben Sie stattdessen die Fehler, verwenden Sie **IISReset** aus der Befehlszeile, um IIS zu beenden und erneut zu starten, gehen Sie zurück zur vorherigen Seite, geben Sie die Bereitstellungsinformationen erneut ein, und klicken Sie dann erneut auf Absenden. Wenn Sie die Fehlermeldung „Zeitüberschreitung der Anforderung“ erhalten, schließen Sie das Fenster, überprüfen Sie, ob das System die Hardwareanforderungen erfüllt, und versuchen Sie, den Server erneut bereitzustellen.