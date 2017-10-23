---
TOCTitle: Migrieren einer Konfigurationsdatenbank
Title: Migrieren einer Konfigurationsdatenbank
ms:assetid: '980e3e94-7d28-40dd-ad01-d34eb3c8d8e6'
ms:contentKeyID: 18118944
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747607(v=WS.10)'
---

Migrieren einer Konfigurationsdatenbank
=======================================

Es kann passieren, dass ein Datenbankserver außer Dienst gestellt werden muss. Dieser Fall kann z. B. eintreten, wenn der RMS-Datenbankserver auf ein neueres Modell umgestellt wird. Bevor der Datenbankserver ausgemustert wird, muss die darauf befindliche Konfigurationsdatenbank auf einen anderen Datenbankserver verschoben werden. Um die Daten in der Konfigurationsdatenbank, einschließlich der darin enthaltenen Schlüsselpaare, zu schützen, sollten Sie eine solche Migration sorgfältig planen und implementieren.

Wir empfehlen, für den RMS-Datenbankserver einen CNAME-Alias zu erstellen und dann RMS so zu konfigurieren, dass dieser Alias verwendet wird. Auf diese Weise müssen Sie den Datenbankservernamen in der RMS-Konfigurationsdatenbank nicht manuell ändern, wenn sich der Servername ändert. Bei Verwendung eines CNAME-Alias braucht nur der Aliasdatensatz aktualisiert zu werden.

Bevor Sie mit der Migration der Konfigurationsdatenbank beginnen, sollten Sie sicherstellen, dass Sie die folgenden Informationen zur Hand haben:

-   den Kontonamen und das Kennwort, das ursprünglich zur Bereitstellung der Server in dem RMS-Cluster verwendet wurde, der mit dieser Datenbank arbeitet
-   das bei der Bereitstellung ursprünglich festgelegte Kennwort des privaten RMS-Schlüssels, sofern zum Speichern des privaten RMS-Schlüssels ein softwarebasierter Kryptografiedienstanbieter (Cryptographic Service Provider, CSP) verwendet wird. Wenn zum Speichern des privaten RMS-Schlüssels ein Hardwaresicherheitsmodul (HSM) verwendet wird, ist dieser Schritt nicht erforderlich.

| ![](images/Cc747607.note(WS.10).gif)Hinweis                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Beim Migrieren der Konfigurationsdatenbank ist kein neues Server-Lizenzgeberzertifikat und auch kein neuer privater Serverschlüssel erforderlich, da RMS die Einstellungen aus der ursprünglichen Konfigurationsdatenbank beibehält. |

Bevor Sie irgendwelche Aktionen am Datenbankserver ausführen, sollten Sie eine Sicherungskopie der RMS-Datenbanken erstellen. Wenn dies nicht möglich ist, müssen Sie Ihr Server-Lizenzgeberzertifikat zumindest exportieren. Weitere Informationen zum Exportieren des Server-Lizenzgeberzertifikats finden Sie unter [So exportieren Sie ein Server-Lizenzgeberzertifikat in eine Datei](https://technet.microsoft.com/d683a629-71b3-4b11-932b-4ab0317334af). Wenn beim Migrieren der Datenbanken ein Fehler auftritt, können Sie das Server-Lizenzgeberzertifikat in eine neue RMS-Installation importieren und Inhalte abrufen, die in der älteren Installation durch Rechte geschützt waren.

Führen Sie zum Migrieren einer Konfigurationsdatenbank die folgenden Schritte aus:

-   Aktualisieren Sie die RMS-Konfigurationsdatenbank so, dass diese den Namen des neuen Datenbankservers verwendet.
-   Aktualisieren der „web.config“-Dateien und der Registrierung auf allen Servern im RMS-Cluster, sodass diese den Namen des neuen Datenbankservers verwenden

| ![](images/Cc747607.Important(WS.10).gif)Wichtig                                                                                       |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| In diesem Abschnitt wird davon ausgegangen, dass die RMS-Datenbanken bereits auf den neuen Datenbankserver kopiert wurden, auf dem sich die RMS-Datenbank befindet. |

Aktualisieren der RMS-Konfigurationsdatenbank, sodass diese den Namen des neuen Datenbankservers verwendet
----------------------------------------------------------------------------------------------------------

Der Name des Datenbankservers, auf dem sich die RMS-Datenbanken befinden, ist in der RMS-Konfigurationsdatenbank gespeichert. Nach dem Migrieren der Datenbankdateien auf den neuen Datenbankserver müssen Sie die RMS-Konfigurationsdatenbank aktualisieren. Diese Aktualisierung können Sie mit dem Tool „RMS Config Editor“ aus dem RMS Administration Toolkit oder mit SQL Management Studio vornehmen.

Führen Sie zum Aktualisieren des Namens des RMS-Datenbankservers mit „RMS Config Editor“ die folgenden Schritte aus:

**So aktualisieren Sie die RMS-Konfigurationsdatenbank mit „RMS Config Editor“**
1.  Melden Sie sich auf einem RMS-Server im Cluster als Mitglied der Datenbankrolle „Systemadministratoren“ an.

2.  Laden Sie das RMS Administration Toolkit aus dem Microsoft Download Center ([http://go.microsoft.com/fwlink/?LinkId=98961](http://go.microsoft.com/fwlink/?linkid=98961)) (möglicherweise in englischer Sprache) herunter, und installieren Sie es.

3.  Wechseln Sie zu „%SystemDrive%:\\Programme\\RMS SP2 Administration Toolkit\\RMSConfigEditor“, und doppelklicken Sie auf **RMSCONFIGEDITOR.EXE**.

4.  Geben Sie im Feld **Server** den Namen des neuen Servers ein, auf dem sich die RMS-Konfigurationsdatenbank befindet, und klicken Sie dann auf **Go**.

5.  Klicken Sie im Feld **Database** auf **DRMS\_Config\_***&lt;RMS-Clustername&gt;***\_***&lt;Port&gt;*, wobei *&lt;RMS-Clustername&gt;* der Name des RMS-Clusters und *&lt;Port&gt;* der TCP-Port ist, über den RMS kommuniziert. Klicken Sie dann auf **Go**.

6.  Klicken Sie auf **DRMS\_ClusterPolicies**.

7.  Geben Sie im Ergebnisbereich in der Spalte **PolicyData** der Zeile **LoggingDatabaseServer** anstelle des vorhandenen Werts den Namen des neuen RMS-Datenbankservers ein.

8.  Klicken Sie auf **Persist**.

9.  Geben Sie in der Spalte **PolicyData** der Zeile **CertificationUserKeyStorageConnectionString** anstelle des vorhandenen Werts den Namen des neuen Datenbankservers ein. Der Wert muss wie folgt aussehen: **data source=***&lt;Neuer Datenbankserver&gt;***;integrated**, wobei *&lt;Neuer Datenbankserver&gt;* der Name des neuen Datenbankservers ist.

10. Klicken Sie auf **Persist**.

11. Wiederholen Sie die Schritte 9 und 10 für den Wert in der Spalte **PolicyData** der Zeile **DirectoryServicesCacheDatabase**.

12. Klicken Sie im linken Bereich auf **DRMS\_PluginProperties**.

13. Geben Sie für **PropertyID** 101 mit der Bezeichnung **PERSISTENT\_STORAGE** in der Spalte **PropertyValue** anstelle des vorhandenen Werts den Namen des neuen Datenbankservers ein. Der Wert muss wie folgt aussehen: **data source=***&lt;Neuer Datenbankserver&gt;***;integrated**, wobei *&lt;Neuer Datenbankserver&gt;* der Name des neuen Datenbankservers ist.

14. Klicken Sie auf **Persist**.

15. Schließen Sie das Tool „RMS Config Editor“.

Führen Sie zum Aktualisieren der RMS-Konfigurationsdatenbank mit SQL Server Management Studio die folgenden Schritte aus:

**So aktualisieren Sie die RMS-Konfigurationsdatenbank mit SQL Server Management Studio**
1.  Melden Sie sich auf dem Server mit der RMS-Konfigurationsdatenbank als lokaler Administrator oder mit einem anderen Benutzerkonto an, das Mitglied der Gruppe der lokalen Administratoren ist.

2.  Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Microsoft SQL Server 2005**, und klicken Sie dann auf **SQL Server Management Studio**.

3.  Vergewissern Sie sich auf der Seite **Verbindung mit Server herstellen**, dass der Name des neuen Datenbankservers im Feld **Servername** aufgeführt ist. Klicken Sie dann auf **Verbinden**.

4.  Blenden Sie die Einträge unter **Datenbanken** ein, blenden Sie die Einträge unter **DRMS\_Config\_***&lt;RMS-Clustername&gt;***\_***&lt;Port&gt;* ein, und blenden Sie dann die Einträge unter **Tabellen** ein.

5.  Klicken Sie mit der rechten Maustaste auf **DRMS\_ClusterPolicies**, und klicken Sie dann auf **Tabelle öffnen**.

6.  Geben Sie im Ergebnisbereich in der Spalte **PolicyData** der Zeile **LoggingDatabaseServer** anstelle des vorhandenen Werts den Namen des neuen RMS-Datenbankservers ein.

7.  Geben Sie in der Spalte **PolicyData** der Zeile **CertificationUserKeyStorageConnectionString** anstelle des vorhandenen Werts den Namen des neuen Datenbankservers ein. Der Wert muss wie folgt aussehen: **data source=***&lt;Neuer Datenbankserver&gt;***;integrated**, wobei *&lt;Neuer Datenbankserver&gt;* der Name des neuen Datenbankservers ist.

8.  Wiederholen Sie die Schritte 6 und 7 für den Wert in der Spalte **PolicyData** der Zeile **DirectoryServicesCacheDatabase**.

9.  Klicken Sie im Objekt-Explorer mit der rechten Maustaste auf **DRMS\_PluginProperties**, und klicken Sie dann auf **Tabelle öffnen**.

10. Geben Sie für **PropertyID** 101 mit der Bezeichnung **PERSISTENT\_STORAGE** in der Spalte **PropertyValue** anstelle des vorhandenen Werts den Namen des neuen Datenbankservers ein. Der Wert muss wie folgt aussehen: **data source=***&lt;Neuer Datenbankserver&gt;***;integrated**, wobei *&lt;Neuer Datenbankserver&gt;* der Name des neuen Datenbankservers ist.

11. Schließen Sie Microsoft SQL Server Management Studio.

Konfigurieren der einzelnen Server im RMS-Cluster, sodass diese den Namen des neuen Datenbankservers verwenden
--------------------------------------------------------------------------------------------------------------

Wenn Sie die einzelnen Server im RMS-Cluster so konfigurieren möchten, dass diese den Namen des neuen Datenbankservers verwenden, müssen Sie die „web.config“-Dateien und drei Registrierungseinträge aktualisieren. Wenn Sie damit fertig sind, müssen Sie Internetinformationsdienste (IIS) neu starten, damit die Änderungen wirksam werden.

So aktualisieren Sie die „web.config“-Dateien auf jedem einzelnen Server im RMS-Cluster:

**So aktualisieren Sie die „web.config“-Dateien auf jedem einzelnen Server im RMS-Cluster**
1.  Melden Sie sich auf einem Server im RMS-Cluster als Mitglied der Gruppe der lokalen Administratoren an.

2.  Wechseln Sie zu „%Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\admin“.

3.  Doppelklicken Sie auf **web.config**, aktivieren Sie die Option **Programm aus einer Liste auswählen**, und klicken Sie auf **OK**.

4.  Klicken Sie auf **Editor**, deaktivieren Sie die Option **Dateityp immer mit dem ausgewählten Programm öffnen**, und klicken Sie auf **OK**.

5.  Klicken Sie auf **Bearbeiten** und dann auf **Ersetzen**.

6.  Geben Sie im Feld **Suchen nach** den Namen des Datenbankservers ein, der außer Dienst gestellt werden soll und auf dem sich die RMS-Datenbanken bisher befinden.

7.  Geben Sie im Feld **Ersetzen mit** den Namen des neuen Datenbankservers ein, auf dem sich die RMS-Datenbanken zukünftig befinden.

8.  Klicken Sie auf **Alle ersetzen** und dann auf **Abbrechen**.

9.  Klicken Sie auf **Datei** &gt; **Speichern**.

10. Schließen Sie Editor.

11. Wiederholen Sie die Schritte 2 bis 9 für die „web.config“-Dateien in den Verzeichnissen „%Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\certification“ und „%Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\licensing“.

12. Wiederholen Sie die Schritte 1 bis 11 für jeden Server im RMS-Cluster.

Aktualisieren Sie zum Schluss die Registrierung auf jedem Server im RMS-Cluster so, dass sie den Namen des neuen Datenbankservers enthält:

| ![](images/Cc747607.Caution(WS.10).gif)Vorsicht                                                                                                                                           |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Durch eine fehlerhafte Bearbeitung der Registrierung können schwerwiegende Schäden am System verursacht werden. Bevor Sie Änderungen an der Registrierung vornehmen, sollten Sie alle wichtigen Computerdaten sichern. |

**So aktualisieren Sie die Registrierung auf jedem einzelnen Server im RMS-Cluster**
1.  Melden Sie sich auf einem Server im RMS-Cluster als Mitglied der Gruppe der lokalen Administratoren an.

2.  Klicken Sie auf **Start** und dann auf **Ausführen**.

3.  Geben Sie **regedit.exe** ein, und klicken Sie auf **OK**.

4.  Wechseln Sie zu **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\KeyProtection**.

5.  Ändern Sie den Registrierungseintrag „PASSWORDDERIVEDKEY\_*&lt;Alter Datenbankserver&gt;*\_DRMS\_CONFIG\_*&lt;RMS-Clustername&gt;*\_*&lt;Port&gt;*“ wie folgt:

    PASSWORDDERIVEDKEY\_*&lt;Neuer Datenbankserver&gt;*\_DRMS\_CONFIG\_*&lt;RMS-Clustername&gt;*\_*&lt;Port&gt;*

    wobei gilt:

    -   *&lt;Alter Datenbankserver&gt;* ist der Name des alten Datenbankservers.
    -   *&lt;RMS-Clustername&gt;* ist der Name des RMS-Clusters.
    -   *&lt;Port&gt;* ist der TCP-Port, über den RMS kommuniziert.
    -   *&lt;Neuer Datenbankserver&gt;* ist der Name des neuen Datenbankservers.

6.  Wechseln Sie zu **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet001\\Services\\DRMS\_Logging\_&lt;RMS-Clustername&gt;\_&lt;Port&gt;\\Params**.

7.  Ändern Sie den Registrierungseintrag **ConnectionString** so, dass der Wert für die Datenquelle mit dem Namen des neuen Datenbankservers identisch ist.

8.  Wiederholen Sie die Schritte 6 und 7 für **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\DRMS\_Logging\_&lt;RMS-Clustername&gt;\_&lt;Port&gt;\\Params**.

9.  Geben Sie an einer Eingabeaufforderung **IISRESET** ein, und drücken Sie die EINGABETASTE.

10. Wiederholen Sie die Schritte 1 bis 9 für alle Server im RMS-Cluster.