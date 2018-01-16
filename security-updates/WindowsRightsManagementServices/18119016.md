---
TOCTitle: 'So installieren Sie Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) zur Bereitstellung von Datenbankunterstützung für RMS'
Title: 'So installieren Sie Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) zur Bereitstellung von Datenbankunterstützung für RMS'
ms:assetid: 'c9b9cd08-98c4-424f-b3fc-d685f57c002e'
ms:contentKeyID: 18119016
ms:mtpsurl: 'https://msdn.microsoft.com/de-de/library/Cc747667(v=WS.10)'
---

So installieren Sie Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) zur Bereitstellung von Datenbankunterstützung für RMS
==============================================================================================================================

Installieren von Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) zur Bereitstellung von Datenbankunterstützung für RMS
---------------------------------------------------------------------------------------------------------------------------

#### So installieren Sie Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) zur Bereitstellung von Datenbankunterstützung für RMS

1.  Melden Sie sich am Server, auf dem Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) installiert werden soll, unter Verwendung eines Domänenkontos an, das Mitglied der lokalen Gruppe Administratoren ist.

2.  Downloaden Sie MSDE 2000 von der [Microsoft-Website](http://www.microsoft.com/)(http://www.microsoft.com/), und speichern Sie es auf Ihrem Computer.

3.  Führen Sie MSDE2000A.exe aus, um das MSDE 2000-Setuppaket in einen Ordner zu extrahieren. Standardmäßig wird dieser Ordner „MSDERelA“ genannt, Sie können jedoch auch einen anderen Namen angeben.

4.  Öffnen Sie eine Eingabeaufforderung, und navigieren Sie zu dem Speicherort, an dem Sie die Installation MSDE 2000 gespeichert haben.

5.  Geben Sie den folgenden Befehl ein, um die Anwendung Microsoft SQL Server 2000 Desktop Engine mit der richtigen Konfiguration für die Verwendung mit RMS (Rights Management Services oder Dienste für die Rechteverwaltung) zu installieren, und ersetzen Sie *Kennwort* durch ein sicheres Kennwort Ihrer Wahl:

    **Setup.exe /i setup\\sqlrun10.msi INSTANCENAME=RMS DISABLEAGENTSTARTUP=1 SAPWD=***Kennwort*

    | ![](https://msdn.microsoft.com/de-de/Cc747667.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                          |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Der Dienst MSDE muss nach der Installation gestartet werden. Sie können den Dienst in der **Systemsteuerung** unter **Dienste** starten. Sie sollten den automatischen Start des Dienstes konfigurieren, um sicherzustellen, dass die MSDE-Datenbank immer verfügbar ist, wenn RMS ausgeführt wird. |

Stellen Sie RMS nicht auf einem Server bereit, bevor Sie eine Datenbank installiert haben, um die RMS-Konfigurationsdatenbank zu unterstützen.

Sie sollten Microsoft SQL Server Desktop Engine (MSDE) nur in Testumgebungen zur Unterstützung von RMS-Datenbanken verwenden, da Microsoft SQL Server Desktop Engine nicht die notwendigen Tools für die uneingeschränkte Ausführung und Unterstützung einer unternehmensweiten Datenbank enthält. MSDE unterstützt außerdem nicht den Remote-Netzwerkbetrieb und muss daher auf demselben Server wie RMS installiert werden. Zudem können Sie keine weiteren RMS-Server in den RMS-Cluster aufnehmen. In den Nutzungsbedingungen für Microsoft SQL Server Desktop Engine wird angegeben, dass SQL Server-Clienttools nicht zur Bearbeitung einer Microsoft SQL Server Desktop Engine-Datenbank verwendet werden können. Aufgrund dieser Einschränkung können Sie weder die RMS-Konfigurationsdatenbank sichern und wiederherstellen noch Protokollierungsinformationen anzeigen oder in der Konfigurationsdatenbank gespeicherte Daten direkt bearbeiten.