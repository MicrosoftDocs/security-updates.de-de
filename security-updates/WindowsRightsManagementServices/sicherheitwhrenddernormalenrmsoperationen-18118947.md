---
TOCTitle: 'Sicherheit während der normalen RMS-Operationen'
Title: 'Sicherheit während der normalen RMS-Operationen'
ms:assetid: '98f3d584-6320-4aa1-9959-7133cfdb6df7'
ms:contentKeyID: 18118947
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747609(v=WS.10)'
---

Sicherheit während der normalen RMS-Operationen
===============================================

Nachdem Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) installiert und bereitgestellt haben, werden die RMS-Webdienste als IIS-Anwendungen (Internet Information Services oder Internetinformationsdienste) ausgeführt, die auf verschiedene Systemressourcen zugreifen, wofür eine Authentifizierung und Autorisierung erforderlich ist. Alle Systemressourcen müssen authentifiziert werden. Eine andere Art der Konfiguration ist nicht möglich. Nachfolgend wird auf dieser Seite die Autorisierungsstruktur in RMS beschrieben.

Die RMS-Webdienste werden im Rahmen eines IIS-Anwendungspools ausgeführt. Jeder Anwendungspool in IIS hat eine eindeutige Identität, die einem Domänenbenutzerkonto, einem lokalen Benutzerkonto, dem lokalen Konto Netzwerkdienst oder dem lokalen Konto Lokales System entsprechen kann. Diese Konten erfordern ein unterschiedliches Maß an Autorisierung innerhalb des Systems. Wenn RMS bereitgestellt wird, können Sie wählen, ob die RMS-Webdienste als Konto „Lokales System“ oder als Domänenbenutzerkonto ausgeführt werden sollen. Dieses Konto wird dann zur Anwendungspoolidentität für den RMS-Anwendungspool. Der Anwendungspool für die Website Globale Verwaltung ist der DRMS-Anwendungspool. Der Anwendungspool für die bereitgestellte Website heißt \_DRMSAppPool1. Der RMS-Protokollierungsdienst wird als separater Windows-Dienst unter demselben Konto ausgeführt, das für die RMS-Anwendungspoolidentität angegeben ist.

Zu den Ressourcen, die für den Zugriff der RMS-Webdienste erforderlich sind, gehören verschiedene Dateien und Ordner auf dem System, Datenbanken und gespeicherte Prozeduren auf dem Datenbankserver, die lokale Registrierung, Active Directory, der Assemblierungscache, Speicherressourcen und andere Prozesse, die auf dem System ausgeführt werden. Der RMS-Protokollierungsdienst muss darüber hinaus auch Zugriff auf die Protokollierungswarteschlange auf dem lokalen System haben. Jede dieser Ressourcen verfügt über eigene freigegebene Zugriffssteuerungslisten (Discretionary Access Control Lists oder DACLs), die definieren, wer zum Zugriff auf die Ressource berechtigt ist und welchem Zweck die Ressource dient.

Um das Zuweisen von Berechtigungen und das Verwalten von Dienstkonten zu vereinfachen, werden alle erforderlichen Berechtigungen der lokalen RMS Service Group (RMS-Dienstgruppe) zugewiesen, die RMS während der Bereitstellung erstellt hat. Da das RMS-Dienstkonto ein Mitglied dieser Gruppe ist, erhält es alle Berechtigungen, die dieser Gruppe erteilt werden.

Folgende Liste fasst die Berechtigungen zusammen, die der RMS Service Group erteilt werden:

-   Berechtigung Lesen für die virtuellen Stammverzeichnisse
-   Berechtigung Schreiben für das Assemblierungscacheverzeichnis
-   Berechtigung Schreiben für das temporäre Systemverzeichnis
-   Berechtigung Schreiben für die Protokollierungswarteschlange
-   Berechtigung Lesen für Active Directory

Wenn Sie Microsoft SQL Server 2000 als Datenbankserver verwenden, sollten Sie bedenken, dass dieses Programm eine etwas andere Methode beim Erteilen von Berechtigungen verwendet als Windows Server 2003. Beim Bereitstellen von RMS wird eine Anmeldung für das RMS-Dienstkonto bei SQL Server erstellt. Wenn Sie sich dafür entschieden haben, RMS als Konto „Lokales System“ bereitzustellen, wird eine Anmeldung für SQL Server im Format *DOMAIN\\Computername* erstellt. Dabei ist *DOMAIN* der Name der Active Directory-Domäne, in der der Computer Mitglied ist, und *Computername* ist der Name des Servers. Die SQL-Rolle rms\_service wird erstellt, und ihr werden alle erforderlichen Berechtigungen zugewiesen. Die Anmeldung für das RMS-Dienstkonto wird dieser Gruppe hinzugefügt. Es werden keine Berechtigungen explizit für das RMS-Dienstkonto erteilt.

Darüber hinaus weist SQL Server jeder Datenbank einen Datenbankbesitzer (Database Owner oder DBO) zu. Die Datenbankbesitzrechte werden während der Bereitstellung wie folgt zugewiesen:

-   Der Datenbankbesitzer für die Konfigurationsdatenbank wird dem Domänenkonto zugewiesen, das zur Bereitstellung von RMS verwendet wurde.
-   Der Datenbankbesitzer für die Datenbank der Verzeichnisdienste und die Protokollierungsdatenbank wird dem RMS-Dienstkonto zugewiesen.

Die Berechtigungen für alle von RMS erstellten Ressourcen wurden bei der Entwicklung von RMS sehr sorgfältig im Hinblick auf Sicherheit ausgewählt. In der Regel ist es nicht erforderlich, die während der Bereitstellung für die Ressourcen zugewiesenen Berechtigungen zu ändern. Wenn Sie nach der Bereitstellung das Benutzerkonto oder Kennwort des Dienstkontos ändern müssen, können Sie dies auf der Seite „Globale Verwaltung“ der RMS-Webseite tun. Weitere Informationen hierzu finden Sie unter „So ändern Sie das RMS-Dienstkonto“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.