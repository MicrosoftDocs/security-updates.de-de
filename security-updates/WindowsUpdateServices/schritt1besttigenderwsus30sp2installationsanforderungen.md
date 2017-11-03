---
TOCTitle: 'Schritt 1: Bestätigen der WSUS 3.0 SP2-Installationsanforderungen'
Title: 'Schritt 1: Bestätigen der WSUS 3.0 SP2-Installationsanforderungen'
ms:assetid: 'ec01bd75-5def-4899-8cee-ddab827bbd83'
ms:contentKeyID: 21669580
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd939916(v=WS.10)'
---

Schritt 1: Bestätigen der WSUS 3.0 SP2-Installationsanforderungen
=================================================================

Bestätigen Sie vor der Installation oder Aktualisierung auf Windows Server Upgrade Services 3.0 Service Pack 2 (WSUS 3.0 SP2), dass der Server und die Clientcomputer die Systemanforderungen von WSUS 3.0 SP2 erfüllen. Darüber hinaus müssen Sie bestätigen, dass Sie berechtigt sind, die Installation abzuschließen.

Hardware- und Softwareanforderungen für Server bei der Installation von WSUS 3.0 SP2
------------------------------------------------------------------------------------

1.  Bestätigen Sie, dass der Server die Systemanforderungen von WSUS 3.0 SP2 für Hardware, Betriebssystem und andere erforderliche Software erfüllt. Die Systemanforderungen finden Sie in den Anmerkungen zu WSUS unter [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) (in englischer Sprache). Wird die Installation des WSUS 3.0 SP2-Servers mit dem Server-Manager ausgeführt, können Sie die Erfüllung der Softwareanforderungen bestätigen, indem Sie den Schritten im Abschnitt "Installationsvorbereitungen für WSUS 3.0 SP2" folgen.
2.  Wenn Sie Rollen- oder Softwareupdates installieren, die nach abgeschlossener Installation einen Neustart des Servers erfordern, starten Sie den Server neu, bevor Sie WSUS 3.0 SP2 installieren.

Anforderungen an die Clientsoftware
-----------------------------------

Automatische Updates sind der Client von WSUS 3.0. Für automatische Updates bestehen abgesehen von einer Netzwerkverbindung keine Hardwareanforderungen.

1.  Bestätigen Sie, dass der Computer, auf dem Sie automatische Updates installieren, die Systemanforderungen von WSUS 3.0 SP2 für Clientcomputer erfüllt. Die Systemanforderungen finden Sie in den Anmerkungen zu WSUS unter [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) (in englischer Sprache).
2.  Wenn Sie Softwareupdates installieren, die einen Neustart des Computers erfordern, starten Sie diesen neu, bevor Sie WSUS 3.0 SP2 installieren.

Berechtigungen
--------------

Folgende Berechtigungen sind für die angegebenen Benutzer und Verzeichnisse erforderlich:

1.  Das Konto "NT-AUTORITÄT\\NETWORKSERVICE" muss über die Berechtigung "Vollzugriff" für die folgenden Ordner verfügen, damit das WSUS-Verwaltungs-Snap-In ordnungsgemäß angezeigt werden kann:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp
2.  Bestätigen Sie, dass das für die Installation von WSUS 3.0 SP2 vorgesehene Konto Mitglied der lokalen Administratorgruppe ist.

Installationsvorbereitungen für WSUS 3.0 SP2
--------------------------------------------

Bei Windows 7 oder Windows Server 2008 SP2 kann WSUS 3.0 SP2 vom Server-Manager aus installiert werden. Wenn Sie ein anderes unterstütztes Betriebssystem verwenden oder nur die WSUS-Verwaltungskonsole installieren, gehen Sie zum nächsten Abschnitt dieses Handbuchs, und installieren Sie WSUS 3.0 SP2 mit der Datei WSUSSetup.exe.

**So bereiten Sie die Installation des WSUS 3.0 SP2-Servers mit dem Server-Manager vor**
1.  Melden Sie sich auf dem für die Installation von WSUS 3.0 SP2 vorgesehenen Server mit einem Konto an, das Mitglied der lokalen Administratorgruppe ist.

2.  Klicken Sie auf **Start**, zeigen Sie auf **Verwaltung**, und klicken Sie dann auf **Server-Manager**.

3.  Klicken Sie im Bereich "Rollenübersicht" auf der rechten Seite des Fensters "Server-Manager" auf **Rollen hinzufügen**.

4.  Wenn die Seite "Vorbemerkung" angezeigt wird, klicken Sie auf **Weiter**.

5.  Auf der Seite "Serverrollen auswählen" müssen Sie bestätigen, dass **Anwendungsserver** und **Webserver (IIS)** ausgewählt werden. Wenn diese ausgewählt wurden, müssen Sie nur noch bestätigen, dass die erforderlichen Rollendienste ausgewählt sind. Andernfalls müssen Sie den Anwendungsserver und den Webserver (IIS) folgendermaßen installieren.

    1.  Wählen Sie auf der Seite "Serverrollen auswählen" **Anwendungsserver** und **Webserver (IIS)**. Klicken Sie auf **Weiter**.
    2.  Wenn Sie Anwendungsrollendienste installieren, klicken Sie auf der Seite "Anwendungsserver" auf **Weiter**. Akzeptieren Sie auf der Seite "Rollendienste für Anwendungsserver" die Standardeinstellungen, und klicken Sie auf **Weiter**.
    3.  Wenn Sie den Webserver IIS installieren, klicken Sie auf der Seite "Webserver (IIS)" auf **Weiter**. Wählen Sie auf der Seite "Rollendienste für Webserver (IIS)" zusätzlich zu den Standardeinstellungen **ASP.NET**, **Windows-Authentifizierung**, **Dynamische Inhaltskomprimierung**, und **IIS 6 Verwaltungskompatibilität**. Wenn das Fenster des Assistenten für das Hinzufügen von Rollen angezeigt wird, klicken Sie auf **Erforderliche Rollendienste hinzufügen**. Klicken Sie auf **Weiter**.
    4.  Klicken Sie auf der Seite "Installationsauswahl bestätigen" auf **Installieren**.
    5.  Bestätigen Sie auf der Seite "Installationsergebnisse" die Meldung über die erfolgreiche Installation der in diesem Schritt installierten Rollendienste, und klicken Sie anschließend auf **Schließen**.

Nächster Schritt
----------------

[Schritt 2: Installieren des WSUS-Servers oder der WSUS-Verwaltungskonsole](https://technet.microsoft.com/6db6fcb0-c55d-43b9-9b07-4040c6267759)

Weitere Ressourcen
------------------

[Schrittweise Anleitung für Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
