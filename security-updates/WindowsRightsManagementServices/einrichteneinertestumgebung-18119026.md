---
TOCTitle: Einrichten einer Testumgebung
Title: Einrichten einer Testumgebung
ms:assetid: 'cdd96b05-49e2-4b6f-bfae-40b5c028ec66'
ms:contentKeyID: 18119026
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747673(v=WS.10)'
---

Einrichten einer Testumgebung
=============================

RMS wird in Ihre bestehende Active Directory-Infrastruktur und den vorhandenen Datenbankserver wie etwa Microsoft SQL Server™ 2000 integriert. Aufgrund der Unabdingbarkeit dieser unterstützenden Komponenten sollten Sie RMS in einer isolierten Testumgebung umfassend testen, bevor Sie es auf Ihre Organisation anwenden. g8Dazu ist das Einrichten von separaten Active Directory- und Datenbankserver-Installationen in der Testumgebung erforderlich.

Beginnen Sie zunächst mit der grundlegendsten Konfiguration eines RMS-Servers in einer Gesamtstruktur mit Datenbankserver und Client. Nachdem Sie sich mit RMS vertraut gemacht haben, können Sie Ihre Konfiguration auf genau die Topologie ausweiten, die Sie in der Produktionsumgebung Ihrer Organisation anwenden möchten, und mehrere Gesamtstrukturen und erforderlichenfalls externen Zugriff hinzufügen. Selbst wenn die Testumgebung nicht alle Redundanzen und Konfigurationen mehrerer Sites des Bereitstellungsplans der Organisation aufweist, sollte zumindest ein Server mit den einzelnen unterstützenden Komponenten, die bereitgestellt werden müssen, enthalten sein.

In der folgenden Liste wird eine mögliche Mindestkonfiguration für eine Testumgebung beschrieben, die Sie zum Testen einer grundlegenden Konfiguration für RMS verwenden können:

-   Ein unter Windows 2000 Server mit Service Pack 3 (SP3) oder später ausgeführter Domänencontroller sowie ein SQL Server 2000 mit installiertem SP3a; SQL Server hostet die RMS-Protokollierung, Konfiguration und Verzeichnisdienste-Datenbanken; RMS kann entweder mit Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A oder SQL Server verwendet werden, wenn sich die Datenbank auf demselben Server wie RMS befindet. Wenn Sie einen Remoteserver für die Datenbankunterstützung verwenden möchten, ist SQL Server erforderlich. Sie können MSDE 2000 von der Microsoft-Website herunterladen.

| ![](images/Cc747673.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Windows 2000 Server mit Service Pack 3 (SP3) gilt als Mindestanforderung für den Domänencontroller, Windows Server 2003 sollte aufgrund der Leistungsverbesserungen in der Active Directory-Gruppenerweiterung verwendet werden. MSDE 2000 sollte zur Unterstützung von RMS-Datenbanken nur in Testumgebungen verwendet werden, weil MSDE 2000 keine Netzwerkschnittstellen unterstützt. Darüber hinaus wird in den Nutzungsbedingungen für MSDE 2000 angegeben, dass SQL Server-Clienttools nicht zur Bearbeitung einer MSDE 2000-Datenbank verwendet werden können. Aufgrund dieser Einschränkung können Sie weder Protokollierungsinformationen anzeigen lassen noch in der Konfigurationsdatenbank gespeicherte Daten ändern. |

-   Ein unter Windows Server 2003 ausgeführter Stammzertifizierungsserver, auf dem RMS installiert und bereitgestellt wird; Im Laufe der Testverfahren können Sie gegebenenfalls mehr Server zur Erstellung eines Stammzertifizierungsclusters hinzufügen.
-   Ein unter Windows XP Professional ausgeführter Client-Computer, ein RMS-Client und eine RMS-fähige Anwendung;
-   Benutzerkonten, die E-Mail-Adressenattribute in Active Directory aufweisen;

Informationen zur Installation und Konfiguration einer grundlegenden RMS-Infrastruktur sowie zur Anwendung der Infrastrukturanforderungen auf eine Produktionsumgebung finden Sie nachstehend unter „[Einrichten einer grundlegenden Infrastruktur](https://technet.microsoft.com/3a0a3a47-e755-4455-bb22-0e05053723e4)“.
