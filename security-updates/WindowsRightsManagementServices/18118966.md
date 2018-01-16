---
TOCTitle: Einrichten von SMS oder einer Gruppenrichtlinie zur Unterstützung der Clientbereitstellung
Title: Einrichten von SMS oder einer Gruppenrichtlinie zur Unterstützung der Clientbereitstellung
ms:assetid: '9e37c27b-8cc1-40c6-adb7-0937aa64c8db'
ms:contentKeyID: 18118966
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747703(v=WS.10)'
---

Einrichten von SMS oder einer Gruppenrichtlinie zur Unterstützung der Clientbereitstellung
==========================================================================================

Beim Bereitstellen von RMS muss eine RMS-fähige Anwendung auf den Benutzercomputern installiert werden, damit die Benutzer Inhalte schützen und RMS-geschützte Inhalte abrufen können.

Eine RMS-fähige Anwendung muss den RMS-Client in ihre Operationen integrieren. In älteren Betriebssystemen als Windows Vista® steht der RMS-Client als separat downloadbare Windows-Komponente im Microsoft Download Center zur Verfügung. Wenn Sie allerdings den Client nicht individuell für jeden Clientcomputer des Unternehmens herunterladen möchten, können Sie Microsoft Systems Management Server (SMS), eine Gruppenrichtlinie oder Skripts zur Automatisierung der Übertragung der RMS-Clients an die Clientcomputer verwenden.

> [!IMPORTANT]
> Der RMS-Client ist in Windows Vista integriert. Deshalb ist keine separate Installation mehr erforderlich. 

Beim Einsatz von SMS zur Verteilung des RMS-Clients müssen Sie folgende Schritte ausführen:

-   Erstellen Sie eine neue Paketdefinitionsdatei.
-   Extrahieren Sie die Windows-Installationsdateien aus der Datei „WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe“. Dazu müssen Sie zunächst die Datei „WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe“ speichern. Installieren Sie sie nicht. Nehmen wir an, die Datei ist im Pfad c:\\Ordnername gespeichert. Öffnen Sie ein Eingabeaufforderungsfenster, und geben Sie folgenden Befehl ein:

    `c:\folder_name\WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x/t:c:\folder_name`
    
    Durch diesen Befehl werden die Dateien „MSDrmClient.msi“ und „RMClientBackCompat.msi“ aus der .exe-Datei extrahiert und unter dem Pfad c:\\*Ordnername* abgelegt.
-   Verwenden Sie die Windows-Installationsdateien für die Paketdefinition und Quelle.
-   Verbreiten Sie die Verfügbarkeit der Pakete über das Netzwerk.

> [!NOTE]
> Zur Installation der Software sind Administratorrechte nötig. Die Sicherheitsrichtlinie Ihrer Organisation erfordert möglicherweise die Installation der RMS-Clientsoftware durch einen Systemadministrator. 

Weitere Informationen über die Verwendung von SMS zum Verteilen von Software finden Sie im Handbuch für Konzepte, Planung und Bereitstellung für Systems Management Server 2003 ([http://go.microsoft.com/fwlink/?LinkId=17401](http://go.microsoft.com/fwlink/?linkid=17401)).

Weitere Informationen zum Bereitstellen von Client-Software durch Gruppenrichtlinien erhalten Sie in den Themen zur gruppenrichtlinienbasierten Softwarebereitstellung ([http://go.microsoft.com/fwlink/?LinkID=38997](http://go.microsoft.com/fwlink/?linkid=38997)).