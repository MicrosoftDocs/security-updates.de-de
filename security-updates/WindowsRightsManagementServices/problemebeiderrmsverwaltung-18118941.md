---
TOCTitle: 'Probleme bei der RMS-Verwaltung'
Title: 'Probleme bei der RMS-Verwaltung'
ms:assetid: '97013c08-d3fa-4ea0-8914-995b6c97f900'
ms:contentKeyID: 18118941
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747605(v=WS.10)'
---

Probleme bei der RMS-Verwaltung
===============================

Nach der erfolgreichen Bereitstellung von RMS auf Ihrem Server treten möglicherweise Probleme bei der täglichen Verwaltung von RMS auf. Die Informationen in den folgenden Abschnitten können zur Lösung dieser Probleme beitragen.

Bei dem Versuch, die RMS-Verwaltungswebsite zu öffnen, wird die Meldung angezeigt, dass SQL Server nicht vorhanden ist oder der Zugriff darauf verweigert wird („SQL Server does not exist or access denied“).
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Wenn Sie RMS mit einer neuen Installation von SQL Server 2005 als Datenbankserver installiert haben, wurde der SQL Server-Dienst eventuell nicht gestartet. In SQL Server 2005 ist der Dienst MSSQLSERVER nicht so konfiguriert, dass er automatischen gestartet wird, sobald der Server gestartet wird. Wenn Sie SQL Server seit der Installation von RMS erneut gestartet und diesen Dienst nicht für einen automatischen Neustart konfiguriert haben, kann RMS nicht funktionieren, und Sie können nur auf die RMS-Seite „Globale Verwaltung“ zugreifen.

Nachdem Sie den Dienst MSSQLSERVER gestartet haben, müssen Sie auch die Internetinformationsdienste (Internet Information Services oder IIS) auf dem RMS-Server neu starten, um die RMS-Funktionalität wiederherzustellen.

Offlineregistrierungsvorgang kann nicht abgeschlossen werden
------------------------------------------------------------

Wenn die Registrierungsanforderungsdatei nicht vollständig ist oder geändert wurde, bevor sie der Website des Registrierungsdienstes übergeben wird, können Sie die Offlineregistrierung nicht abschließen. Die Registrierungsanforderungsdatei wurde eventuell durch ein bösartiges Programm, einen Benutzerfehler oder einen Systemfehler beschädigt.

Je nachdem, welche Informationen fehlen, kann die Website des Registrierungsdienstes entweder die Datei dennoch akzeptieren und ein Server Lizenzgeberzertifikat zurückgeben oder die Datei zurückweisen und eine Fehlermeldung ausgeben.

Wenn ein Server-Lizenzgeberzertifikat zurückgegeben wird, werden darin Beschädigungen oder fehlende Informationen in der Registrierungsanforderungsdatei angegeben, und RMS zeigt eine Fehlermeldung an, wenn Sie versuchen, das Zertifikat zu importieren.

Wenn Sie den Registrierungsprozess nicht abschließen können, überprüfen Sie, ob der Computer mit der Internetverbindung frei von Viren ist, exportieren Sie die Registrierungsanforderungsdatei erneut vom RMS-Server, und verwenden Sie dann andere Datenträger, um sie auf den Computer mit der Internetverbindung zu übertragen. Wenn der Fehler erneut auftritt, sollten Sie sich an Microsoft Product Support Services wenden.

Protokolldateien werden nicht erstellt
--------------------------------------

Für den RMS-Protokollierungsdienst ist sowohl Message Queuing (auch MSMQ genannt) als auch Zugriff auf die Protokollierungsdatenbank erforderlich. Wenn keine Protokolldateien erstellt werden, kann dies bedeuten, dass die Komponenten nicht korrekt konfiguriert wurden oder dass die Kommunikation zwischen den Computern unterbrochen wurde.

Führen Sie einen Test durch, um sicherzustellen, dass die Netzwerkverbindung zwischen dem RMS-Server und dem Datenbankserver vorhanden ist und funktioniert. Wenn dies der Fall ist, führen Sie folgende Schritte aus, um die Voraussetzungen für den RMS-Protokollierungsdienst zu überprüfen und sicherzustellen, das alle Softwareabhängigkeiten korrekt konfiguriert wurden.

Schritt 1: Stellen Sie sicher, dass Message Queuing ordnungsgemäß konfiguriert ist. Message Queuing muss mit aktivierter Active Directory-Integration installiert werden.

**So stellen Sie sicher, dass Message Queuing ordnungsgemäß installiert und konfiguriert wurde**
1.  Klicken Sie in der **Systemsteuerung** auf **Software** und anschließend auf **Windows-Komponenten hinzufügen/entfernen**, um den **Assistenten für Windows-Komponenten** zu öffnen.

2.  Aktivieren Sie im **Assistenten für Windows-Komponenten** das Kontrollkästchen **Anwendungsserver**, und klicken Sie anschließend auf **Details**.

3.  Aktivieren Sie das Kontrollkästchen **Message Queuing**, und klicken Sie anschließend auf **Details**.

4.  Wenn das Kontrollkästchen **Integration des Active Directory** bereits aktiviert ist, fahren Sie mit dem nächsten Test fort, und überprüfen Sie, ob Message Queuing ausgeführt wird. Wenn das Kontrollkästchen nicht aktiviert ist, fahren Sie mit den Schritten 5 bis 9 fort.

5.  Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Webseite „Globale Verwaltung“ zu öffnen.

6.  Klicken Sie neben der Website, auf der RMS bereitgestellt wird, auf **RMS von dieser Website entfernen**, und klicken Sie dann auf **OK**.

7.  Klicken Sie in der **Systemsteuerung** auf **Software**, dann auf **Windows-Komponenten hinzufügen/entfernen**, dann auf **Anwendungsserver** und schließlich auf **Message Queuing**.

8.  Aktivieren Sie die **Active Directory-Integration**, indem Sie auf **Details** klicken, das Kontrollkästchen **Integration des Active Directory** aktivieren und anschließend auf **OK** klicken.

9.  Öffnen Sie die Seite **Globale Verwaltung**. Klicken Sie neben dem Namen der Website, auf der Sie RMS bereitstellen möchten, auf **RMS auf dieser Website bereitstellen**.

Schritt 2: Stellen Sie sicher, dass Message Queuing auf Ihrem Server ausgeführt wird.

**So stellen Sie sicher, dass Message Queuing auf Ihrem Server ausgeführt wird**
1.  Klicken Sie in der **Systemsteuerung** auf **Verwaltung** und anschließend auf **Dienste**.

2.  Blättern Sie in der Liste, bis Sie den Dienst **Message Queuing** finden.

3.  In der Spalte **Status** muss für den Dienst die Angabe **Gestartet** stehen. Wenn dies nicht der Fall ist, klicken Sie mit der rechten Maustaste auf den Dienst, und klicken Sie anschließend auf **Starten**.

Schritt 3: Stellen Sie sicher, dass der Protokollierungsdienst die Berechtigung hat, Ereignisse in die Protokollierungsdatenbank zu schreiben. Der RMS-Protokollierungsdienst wird über das RMS-Dienstkonto ausgeführt. Stellen Sie sicher, dass das RMS-Dienstkonto eine gültige Anmeldung für den Datenbankserver hat und über die erforderlichen Berechtigungen verfügt, um Datenbanken zu erstellen und Informationen in die Dateien zu schreiben.

Wenn all diese Voraussetzungen erfüllt sind, stoppen Sie den RMS-Protokollierungsdienst, und starten Sie ihn erneut über das Snap-In für Dienste. Nach dem erneuten Start des RMS-Protokollierungsdienstes sollten Protokolldateien auf dem Datenbankserver erstellt werden. Wenn Sie SQL Server als Datenbankserver verwenden, können Sie mit Hilfe folgender Schritte überprüfen, ob Protokolldateien erstellt werden.

**So stellen Sie sicher, dass in SQL Server Protokolldateien erstellt werden**
1.  Wechseln Sie in SQL Server Enterprise Manager zur Protokollierungsdatenbank, erweitern Sie **Datenbanken**, und erweitern Sie dann die Datenbank, die die RMS-Protokollierungsdatenbank enthält.

2.  Klicken Sie auf die Protokollierungsdatenbank und dann auf **Tabellen**, klicken Sie mit der rechten Maustaste auf **DRMS\_log\_master**, und klicken Sie anschließend auf **Tabelle öffnen – Alle Zeilen zurückgeben**. Wenn Protokolldateien erstellt werden, werden eine oder mehrere Protokolldateien angezeigt.

Wiederherstellen der Konfigurationsdatenbank
--------------------------------------------

RMS kann ohne funktionierende Konfigurationsdatenbank nicht ausgeführt werden. Wenn Sie Probleme mit der Konfigurationsdatenbank haben, wie z. B. Datenbankbeschädigung oder Festplattenfehler auf dem Datenbankserver, können Sie die RMS-Funktionalität wiederherstellen, indem Sie die Sicherung der Konfigurationsdatenbank wiederherstellen. Um die RMS-Konfigurationsdatenbank aus einer Sicherung wiederherstellen zu können, benötigen Sie folgende Informationen:

-   Den Namen der letzten Sicherung der Datenbank.
-   Den Namen des Computers, auf dem die Sicherung der Datenbank wiederhergestellt werden soll.
-   Den Namen und das Kennwort des Kontos, das ursprünglich zum Bereitstellen von RMS verwendet wurde.
-   Das Kennwort, das ursprünglich zum Schutz des privaten Softwareschlüssels (falls zutreffend) verwendet wurde.

Für die Wiederherstellung einer gesicherten Datenbank ist weder ein neues Server-Lizenzgeberzertifikat noch ein neuer privater Schlüssel erforderlich, da RMS alle Einstellungen (die aus der gesicherten Konfigurationsdatenbank abgerufen werden) beibehält.

Führen Sie folgende Schritte aus, um eine gesicherte Datenbank wiederherzustellen.

**So stellen Sie eine gesicherte Datenbank wieder her**
1.  Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Webseite **Globale Verwaltung** zu öffnen.

2.  Klicken Sie neben der Website, auf der RMS bereitgestellt wird, auf **RMS von dieser Website entfernen**, und klicken Sie dann auf **OK**.

3.  Stellen Sie die gesicherten Datenbankdateien für die Konfigurationsdatenbank wieder her. Wenn Sie die Protokollierungsdatenbank im Zuge des Sicherungsverfahrens ebenfalls gesichert haben und Sie die Kontinuität der Daten bewahren möchten, stellen Sie die Protokollierungsdatenbank ebenfalls wieder her.

    -   Sollte dieses System im Anschluss an einen vollständigen Systemausfall wiederhergestellt werden, stellen Sie zunächst die Registrierung mit Hilfe der Systemstatussicherung wieder her, bevor Sie die Datenbankdateien wiederherstellen.

4.  Wenn die Datenbank, die wiederhergestellt wird, einem einzelnen Stammzertifizierungsserver dient, ändern Sie folgenden Registrierungsschlüssel, bevor Sie den Dienst erneut bereitstellen:

    -   Auf Computern mit der 32-Bit-Version von Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0\`
    -   Auf Computern mit der 64-Bit-Version von Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0\`

    Fügen Sie folgenden Eintrag als Zeichenfolgenwert hinzu, und lassen Sie den Wert leer:

    `GicURL`

    Dadurch wird die Active Directory-Suche nach dem Stammzertifizierungsserver außer Kraft gesetzt und der Zugriff auf die Bereitstellungsseiten des Stammzertifizierungsservers ermöglicht.

5.  Wenn Sie zum Sichern des privaten RMS-Schlüssels ein Hardwaresicherheitsmodul (Hardware Security Module oder HSM) verwendet haben, stellen Sie die gesicherte Sicherheitsumgebung wieder her, damit die Schlüssel abgerufen werden können.

6.  Führen Sie dazu einen der folgenden Schritte aus:

    -   Klicken Sie neben der Website, auf der RMS bereitgestellt werden soll, auf „RMS auf dieser Website bereitstellen“, um die Datenbank für einen einzelnen Server statt für einen Cluster wiederherzustellen.
        – Oder –
    -   Klicken Sie neben der Website, auf der RMS bereitgestellt werden soll, auf „Diesen Server zu einem Cluster hinzufügen“, um die Datenbank für einen Cluster wiederherzustellen.

7.  Geben Sie das RMS-Dienstkonto an, das ursprünglich zum Bereitstellen des Servers verwendet wurde.

8.  Geben Sie die gesicherte Konfigurationsdatenbank an (einschließlich des Namens der Datenbank und des Computers, auf dem sich die Datenbank befindet), die Sie verwenden möchten.

9.  Geben Sie das gleiche Kennwort an, das Sie ursprünglich zum Bereitstellen des Servers verwendet haben.

10. Klicken Sie auf **Absenden**.

Der Bereitstellungsprozess wird gestartet, und RMS wird erneut auf dem Server bereitgestellt.

Weitere Informationen dazu finden Sie unter „Planen der Wiederherstellung des Systems“ und „Sichern und Wiederherstellen des RMS-Systems“ im Abschnitt „Planen einer RMS-Bereitstellung“ in dieser Dokumentationssammlung.

Abgelaufenes Kennwort für das RMS-Dienstkonto
---------------------------------------------

Wenn RMS den Betrieb einstellt, kann dies daran liegen, dass das Kennwort für das RMS-Dienstkonto abgelaufen ist. Sehen Sie in IIS-Manager (Internet Information Services oder Internetinformationsdienste) nach. Wenn die RMS-Anwendungspools gestoppt wurden und Sie sie nicht erneut starten können, ist eventuell das Kennwort für das RMS-Dienstkonto abgelaufen.

Wenn Ihr Kennwort für das RMS-Dienstkonto abläuft, muss das Kennwort auf jedem RMS-Server geändert werden, auf dem das Konto mit dem abgelaufenen Kennwort verwendet wird. Starten Sie IIS anschließend erneut. Weitere Informationen hierzu finden Sie unter „Ändern des Kennworts für das RMS-Dienstkonto“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.

Wiederherstellen einer vorherigen RMS-Installation
--------------------------------------------------

Wenn in der Hardware oder Software des RMS-Servers ein Fehler auftritt, können Sie den RMS-Server wiederherstellen, indem Sie die zuvor installierte Konfigurationsdatenbank zum Bereitstellen einer neuen Serverinstanz verwenden.

| ![](images/Cc747605.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Diese Vorgehensweise gilt nur für den Fall, dass auf dem Server, auf dem RMS ausgeführt wird, ein Fehler auftritt. Wenn auf dem Server, auf dem die Konfigurationsdatenbank ausgeführt wird, ein Fehler auftritt, folgen Sie den Anweisungen unter „Wiederherstellen der Konfigurationsdatenbank“ weiter oben in diesem Thema. Wenn der RMS-Server auch der Datenbankserver ist, muss der gesamte Server aus einer Sicherungskopie wiederhergestellt werden. |

Führen Sie folgende Schritte aus, um auf dieselbe Konfigurationsdatenbank zu verweisen, die für die ursprüngliche Installation verwendet wurde.

**So stellen Sie eine vorherige RMS-Installation wieder her**
1.  Melden Sie sich bei dem Computer, den Sie als RMS-Server konfigurieren möchten, über ein Konto mit Administratorberechtigungen an. Stellen Sie sicher, dass der Computer die Mindestsystemanforderungen für RMS erfüllt. Weitere Informationen zu den Systemanforderungen für RMS finden Sie unter „Hardwareanforderungen“ im Abschnitt „Planen einer RMS-Bereitstellung“ in dieser Dokumentationssammlung.

2.  Wenn Sie ein Hardwaresicherheitsmodul (Hardware Security Module oder HSM) zum Schutz des privaten RMS-Schlüssels verwenden, stellen Sie sicher, dass es korrekt konfiguriert ist, indem Sie dieselben Einstellungen und dieselbe Sicherheitsumgebung wie bei der vorherigen RMS-Installation verwenden.

3.  Installieren Sie RMS auf dem Computer.

4.  Klicken Sie nach der Installation von RMS auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

5.  Klicken Sie neben der Website, auf der Sie RMS bereitstellen möchten, auf **Diesen Server zu einem Cluster hinzufügen**.

6.  Geben Sie im Bereich **RMS-Dienstkonto** den Kontonamen für den RMS-Dienst im Format Domänenname\\Benutzername sowie das Kennwort des RMS-Dienstkontos ein, das zur Ausführung von RMS-Standardoperationen verwendet wird. Hierbei muss es sich um ein Domänenkonto handeln.

7.  Geben Sie im Bereich **Konfigurationsdatenbank** den Namen des Datenbankservers und der Konfigurationsdatenbank für die ursprüngliche RMS-Installation ein, die Sie wiederherstellen möchten.

8.  Wählen Sie im Bereich **Schutz durch privaten Schlüssel** den Mechanismus aus, der von diesem Cluster zum Schutz für den privaten Schlüssel verwendet wird. Wenn Sie einen softwarebasierten Schutz des privaten Schlüssels verwendet haben, müssen Sie das Kennwort bereitstellen, mit dem der private Schlüssel bei der ursprünglichen Bereitstellung dieses Clusters verschlüsselt wurde.

9.  Klicken Sie auf **Absenden**.

Clients können RMS-geschützten Inhalt aufgrund abgelaufener Berechtigungen nicht öffnen
---------------------------------------------------------------------------------------

Wenn die Berechtigungen eines Benutzer abgelaufen sind, kann der Benutzer keinen RMS-geschützten Inhalt mehr abrufen. Wenn die Systemuhr auf dem RMS-Server gegenüber der Systemuhr auf dem RMS-Client vorgeht, ist es ebenfalls möglich, dass ein Benutzer keinen RMS-geschützten Inhalt mehr abrufen kann, selbst wenn seine Berechtigungen nicht abgelaufen sind. Da die Systemuhren auf den beiden Computern nicht synchronisiert sind, kann folgende Fehlermeldung angezeigt werden, wenn der Clientcomputer versucht, den Inhalt zu öffnen:

**Sie sind nicht berechtigt, diese Nachricht zu öffnen, weil Ihre Berechtigungen abgelaufen sind. Möchten Sie die Nachricht mit anderen Anmeldeinformationen öffnen?**

Sowohl die Clientlizenz als auch die Inhaltslizenz ist gültig, aber aufgrund der Zeitabweichung interpretiert der Client die Inhaltslizenz als ungültig und zeigt diese Fehlermeldung für den Benutzer an. Daher kann ein Benutzer den Eindruck erlangen, dass ein Problem mit seinem RMS-Kontozertifikat oder mit den für das Dokument erteilten Rechten besteht. Sobald die Uhrzeit auf dem Client den Zeitbereich für die Gültigkeitsdauer der Veröffentlichungslizenz für den Inhalt erreicht hat, kann der Benutzer den Inhalt öffnen.

Als bewährte Vorgehensweise sollten die Clients und die Server im RMS-System für denselben Uhrzeitdienst synchronisiert werden.

Fehlermeldung wegen verweigertem Zugriff („Access is Denied“), wenn RMS versucht, Ereignisse im Anwendungsereignisprotokoll aufzuzeichnen
-----------------------------------------------------------------------------------------------------------------------------------------

Standardmäßig werden Komponenten wie RMS, die von einer ASP-Seite aus ausgeführt werden, unter dem Konto IUSR\_COMPUTERNAME ausgeführt. Dieses Konto ist ein Mitglied der Gruppe „Gäste“, und die für den Schreibzugriff auf das Anwendungsereignisprotokoll erforderlichen Sicherheitsberechtigungen verhindern, dass Gästekonten Daten in das Ereignisprotokoll schreiben können.

Um dieses Problem zu umgehen, können Sie mit dem Registrierungseditor den Registrierungsschlüssel ändern, der dieses Verhalten steuert.

| ![](images/Cc747605.Caution(WS.10).gif)Vorsicht                                                                                                                                         |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Durch falsches Bearbeiten der Registrierung kann das System schwerwiegend beschädigt werden. Deshalb sollten Sie alle wichtigen Daten auf dem Computer sichern, bevor Sie Änderungen an der Registrierung vornehmen. |

Setzen Sie den folgenden Schlüssel auf 0 anstelle von 1, und starten Sie dann den Computer erneut, um die Änderungen zu übernehmen.

`HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\EventLog\Application`

Name: `RestrictGuestAccess`

Type: `REG_DWORD`

| ![](images/Cc747605.note(WS.10).gif)Hinweis                          |
|---------------------------------------------------------------------------------------------------|
| Dadurch wird allen Gästekonten der Schreibzugriff auf das Anwendungsereignisprotokoll ermöglicht. |

Weitere Informationen zur Ursache dieses Fehlers finden Sie im Artikel zur Aktivierung der Protokollierung von ASP-Seiten aus in der [Microsoft Knowledge Base](http://go.microsoft.com/fwlink/?linkid=44167).
