---
TOCTitle: 'So stellen Sie den RMS-Client bereit'
Title: 'So stellen Sie den RMS-Client bereit'
ms:assetid: 'c84f1724-cf71-4385-9003-ff68bc23c927'
ms:contentKeyID: 18119005
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747749(v=WS.10)'
---

So stellen Sie den RMS-Client bereit
====================================

Wenn Sie Microsoft Windows XP oder Microsoft Windows 2000 verwenden, muss der RMS-Client (Rights Management Services) installiert werden, damit Sie RMS-Features wie die Informationsrechteverwaltung unter Microsoft® Office System 2003 und das Add-On für die Rechteverwaltung für Internet Explorer verwenden können. Der RMS-Client ist in Windows Vista® integriert.

Zahlreiche Unternehmen steuern die Bereitstellung der Clientsoftware in ihrem Hause selbst. Es kann entweder der Systems Management Server (SMS) oder die Gruppenrichtlinie verwendet werden, um den RMS-Client mit Service Pack 2 (SP2) bereitzustellen.

Vor der Bereitstellung müssen Sie den RMS-Client unter [http://go.microsoft.com/fwlink/?linkId=67736](http://go.microsoft.com/fwlink/?linkid=67736) downloaden.

| ![](images/Cc747749.Important(WS.10).gif)Wichtig                                |
|--------------------------------------------------------------------------------------------------------------|
| Der RMS-Client wurde in Windows Vista integriert. Deshalb ist keine separate Installation mehr erforderlich. |

Extrahieren der Installationsdateien
------------------------------------

Nachdem Sie die Datei „WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe“ gedownloadet haben, müssen Sie die Dateien für das Microsoft® Windows®-Installationsprogramm aus dem Paket extrahieren.

Geben Sie hierzu den folgenden Befehl in eine Befehlszeile ein:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x <path>`

„&lt;Pfad&gt;“ bezeichnet hierbei das Zielverzeichnis, in dem die extrahierten Dateien abgelegt werden sollen.

Mit diesem Befehl werden die folgenden Dateien in das angegebene Zielverzeichnis extrahiert:

-   Bootstrap.exe
    Diese Wrapper-Datei wird von der ausführbaren Datei herangezogen, um die anderen Dateien im Paket zu installieren. Wenn Sie den RMS SP2-Client über den SMS oder die Gruppenrichtlinie installieren, wird diese Datei nicht verwendet.
-   MSDrmClient.msi
    Dies ist die Installationsdatei für den RMS SP2-Client. Bei dieser Installation werden alle Vorgängerversionen des RMS-Clients auf dem Computer deinstalliert. Dieses Programm sollte als Erstes auf den Clientcomputern installiert werden.
-   RMClientBackCompat.msi
    Dies ist die Installationsdatei, die den neuen RMS SP2-Client für RMS-fähige Anwendungen (wie Microsoft Office Professional 2003 oder 2007 Microsoft Office System) identifizieren, die wiederum von den vorherigen Versionen des RMS-Clients abhängig sind. Auf diese Weise kann der neue RMS SP2-Client verwendet werden. Installieren Sie dieses Programm auf den Clientcomputern, sobald die Datei „MSDrmClient.msi“ erfolgreich installiert wurde.

| ![](images/Cc747749.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                    |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Unabhängig von der Installationsmethode sollten Sie sicherstellen, dass beide Windows-Installationsprogrammdateien fehlerfrei installiert wurden. Wenn ein Fehler auftritt, durch den die Datei „MSDrmClient.msi“ nicht installiert werden kann, installieren Sie nicht die Datei „RMClientBackCompat.msi“. |

Bereitstellen des RMS-Clients mithilfe einer unbeaufsichtigten Installation
---------------------------------------------------------------------------

Das Extrahieren der Dateien zur Installation der Windows-Installationsprogrammdateien ist optional. Sie können den RMS-Client auch durch eine unbeaufsichtigte Installation bereitstellen. Geben Sie hierzu den folgenden Befehl in eine Befehlszeile ein:
```
WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi 
REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q
```

Durch diesen Befehl wird die unbeaufsichtigte Installation des RMS-Client gestartet.

| ![](images/Cc747749.note(WS.10).gif)Hinweis                                                                                                                                                                                              |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Weil es sich um eine unbeaufsichtigte Installation handelt, werden Sie nicht vom Installationsprogramm darüber informiert, wann die Installation abgeschlossen ist. Unbeaufsichtigte Installationen werden üblicherweise in einer Batch- oder Skriptdatei ausgeführt. |

Bereitstellen des RMS-Clients mithilfe eines SMS
------------------------------------------------

**So stellen Sie den RMS-Client mithilfe eines SMS bereit**
1.  Öffnen Sie die SMS-Verwaltungskonsole.

2.  Erweitern Sie die zu verwendende Site-Datenbank.

3.  Klicken Sie im linken Bereich mit der rechten Maustaste auf **Pakete**, wählen Sie **Neu** aus, und klicken Sie dann auf **Paket aus Definition**.

4.  Erstellen Sie Pakete aus den Dateien „MSDRMClient.msi“ und „RMClientBackCompat.msi“. Die Pakete sollten die folgenden Eigenschaften aufweisen:

    **Allgemein**:

    -   Geben Sie unter **Befehlszeile** Folgendes ein:

        `msiexec.exe /q ALLUSERS=2 /m MSIDGHOG /i "<file_name>.msi"`
        | ![](images/Cc747749.note(WS.10).gif)Hinweis                                                                                               |
        |------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
        | MSIDGHOG ist ein zufälliger Wert. Ersetzen Sie &lt;Dateiname&gt; durch den Namen der Windows-Installationsprogrammdatei, die mit diesem Paket installiert werden soll. |

    -   Wählen Sie unter **Ausführen** die Option **Versteckt** aus.
    -   Wählen Sie unter **Nach Ausführung** die Option **Keine Aktion erforderlich** aus.
    -   Wählen Sie unter **Kategorie** die Option **Verwaltungssoftware** aus.

    **Anforderungen:**

    -   Geben Sie unter **Geschätzter Speicherplatz** den Wert **445 KB** ein.
    -   Wählen Sie unter **Maximal zulässige Ausführungszeit** die Option **Unbekannt** aus.
    -   Aktivieren Sie das Kontrollkästchen **Dieses Programm kann auf jeder Plattform ausgeführt werden**.

    **Umgebung:**

    -   Wählen Sie unter **Programm kann ausgeführt werden** die Option **Unabhängig von Benutzeranmeldung** aus.
    -   Wählen Sie unter **Ausführmodus** die Option **Mit Administratorrechten ausführen** aus.
    -   Wählen Sie unter **Laufwerkmodus** die Option **Unterstützt UNC-Namen** aus.

    **Erweitert:**

    -   Deaktivieren Sie das Kontrollkästchen **Ein anderes Programm zuerst ausführen**.
    -   Deaktivieren Sie das Kontrollkästchen **Programmbenachrichtigung unterdrücken** unter **Wenn das Programm einem Computer zugewiesen ist**.
    -   Deaktivieren Sie das Kontrollkästchen **Dieses Programm auf Computern, auf denen es angekündigt wird, deaktivieren**.

5.  Legen Sie die **Zugriffskonten und Verteilungspunkte** gemäß den Anforderungen Ihres Unternehmens fest.

6.  Erstellen Sie eine Ankündigung für die entsprechende Sammlung. In einer SMS-Bereitstellung verwenden Sie nach Möglichkeit das Programm **Pro-System-Installation unbeaufsichtigt**.

7.  Planen Sie diese Ankündigung gemäß den Anforderungen Ihres Unternehmens ein.

Bereitstellen des RMS-Clients mithilfe der Gruppenrichtlinie
------------------------------------------------------------

Mit der Funktion zur Installation und Pflege von Software in der Gruppenrichtlinie können Sie den RMS-Client auf den Zielcomputern bereitstellen.

Die Gruppenrichtlinie wird als Methode für die aktive Verwaltung der Bereitstellung der RMS-Clients für kleine bis mittelgroße Unternehmen empfohlen, die noch keine Aktualisierungsverwaltungslösung wie Systems Management Server 2003 verwenden.

Wenn Sie ein Programm mit der Gruppenrichtlinie verteilen, können Sie das Programm den gewünschten Computern zuweisen. Das Programm wird installiert, sobald der Computer gestartet wird, und steht für alle Benutzer zur Verfügung, die sich beim Computer anmelden. Weitere Informationen zur Gruppenrichtlinie erhalten Sie unter „Entwerfen einer Gruppenrichtlinieninfrastruktur“ (<http://go.microsoft.com/fwlink/?linkid=24328>). Bei diesem Verfahren wird vorausgesetzt, dass Sie die GPMC (Group Policy Management Console, Gruppenrichtlinien-Verwaltungskonsole) verwenden. Um GPMC zu downloaden, informieren Sie sich im Abschnitt zur GPMC mit Service Pack 1 (<http://go.microsoft.com/fwlink/?linkid=21813>).

Das folgende Verfahren bietet eine Kurzanleitung für Administratoren, die nicht mit der Verteilung von Software über die Gruppenrichtlinie vertraut sind. Sie können diese Schritte je nach Bedarf an die Anforderungen Ihres Unternehmens anpassen.

**So stellen Sie den RMS-Client mithilfe der Gruppenrichtlinie bereit**
1.  Öffnen Sie auf einem Domänencontroller das Snap-In **Active Directory-Benutzer und -Computer** von Microsoft Management Console (MMC).

2.  Erstellen Sie eine neue Organisationseinheit (OU), oder wählen Sie eine vorhandene OU aus.

    Wenn Sie eine neue OU erstellt haben, fügen Sie die Computer hinzu, auf denen der RMS-Client installiert werden soll.

3.  Klicken Sie mit der rechten Maustaste auf die OU, und wählen Sie **Eigenschaften** aus.

4.  Wählen Sie die Registerkarte **Gruppenrichtlinie** aus.

5.  Klicken Sie auf **Neu**, um ein neues Gruppenrichtlinienobjekt (GPO) zu erstellen.

6.  Klicken Sie auf **Bearbeiten**, und bearbeiten Sie das neue GPO.

7.  Erweitern Sie in der Konsolenstruktur den Eintrag für **Computerkonfiguration,Softwareeinstellungen**, und wählen Sie dann Softwareinstallation aus.

8.  Klicken Sie mit der rechten Maustaste in das Detailfenster, klicken Sie auf **Neu** und anschließend auf **Paket**.

9.  Geben Sie einen Pfad zur Datei „MSDRMclient.msi“ in einem freigegebenen Netzwerkordner ein, auf den die Clientcomputer zugreifen können.

10. Klicken Sie auf **OK**, um das Paket zuzuweisen.

11. Wiederholen Sie Schritt 5 bis 10, um ein GPO zu erstellen, mit dem die Datei „RMClientBackCompat.msi“ installiert wird.

| ![](images/Cc747749.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Diese Schritte dienen lediglich als Anhaltspunkt für Benutzer, die nicht über Erfahrungen mit der Verwendung der Gruppenrichtlinie verfügen. Als erfahrener Gruppenrichtlinienadministrator können Sie das Paket „MSDrmClient.msi“ mit Ihren eigenen Verfahren verteilen. Des Weiteren gelten diese Schritte nur für Domänencontroller, auf denen Windows Server 2003 ausgeführt wird. Bei einer Windows 2000-Domäne können das Verfahren und die Terminologie ggf. abweichen. |

Aktualisieren von einer vorherigen Version
------------------------------------------

Es ist möglich, eine unbeaufsichtigte Installationsmethode in einem Skript zu verwenden, die erkennt, ob der RMS SP2-Client installiert ist. Wenn der Client nicht installiert ist, aktualisiert das Skript entweder den vorhandenen Client oder installiert den RMS SP2-Client. Das Skript ist folgendermaßen aufgebaut:

```
Set objShell = Wscript.CreateObject("Wscript.Shell")
Set objWindowsInstaller = Wscript.CreateObject("WindowsInstaller.Installer") 
Set colProducts = objWindowsInstaller.Products 

For Each product In colProducts 
strProductName = objWindowsInstaller.ProductInfo (product, "ProductName")

if strProductName = "Windows Rights Management Client with Service Pack 2" then
strInstallFlag = "False"
Exit For
else
strInstallFlag = "True"
end if
Next

if strInstallFlag = "True" then
objShell.run "WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q "
else
wscript.echo "No installation required"
end if
```

| ![](images/Cc747749.note(WS.10).gif)Hinweis                                    |
|-------------------------------------------------------------------------------------------------------------|
| Dieses Skript funktioniert nicht mit Windows Vista, da der RMS-Client in das Betriebssystem integriert ist. |
