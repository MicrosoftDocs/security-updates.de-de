---
TOCTitle: 'RMS-Verwaltungswebsite'
Title: 'RMS-Verwaltungswebsite'
ms:assetid: 'f003c1d9-9a17-4e50-9e1e-5d67677552a0'
ms:contentKeyID: 18119098
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747796(v=WS.10)'
---

RMS-Verwaltungswebsite
======================

Jeder Stammzertifizierungs- und Lizenzierungscluster hostet eine Verwaltungswebsite, über die Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwalten können. Diese Website ist nur auf dem jeweils verwalteten RMS-Server oder über eine Remotedesktopverbindung verfügbar.

Dieses Thema beschreibt die Funktionen der Verwaltungswebsite. Anweisungen zur Verwendung der Website beim Verwalten von RMS finden Sie unter „Vorgehensweisen bei RMS“ und „Verwalten von RMS“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.

**Hinweis** Die Clusterkonfiguration ist global. Sie können die Konfiguration für einen Cluster von der Verwaltungswebsite aus auf jedem beliebigen Server im Cluster verwalten.

Öffnen Sie die Seite **Globale Verwaltung** zur Ausführung der folgenden Aufgaben:

-   Bereitstellen von RMS auf einer Website.
-   Bereitstellen eines Servers und Hinzufügen des Servers zu einem Cluster.
-   Entfernen von RMS von einer Website.
-   Wechseln zu den Verwaltungsseiten für den Cluster.

Öffnen der Seite **Verwaltung** für einen Cluster, um folgende Aufgaben auszuführen:

-   **Anzeigen von Informationen zum Cluster.** Sie können Informationen zum Cluster anzeigen, wie z. B. Installations-URL, Server-URL, Zertifikatsname, Konfigurationsdatenbankserver, Konfigurationsdatenbankname und Ablaufdatum des Zertifikats.
-   **Registrieren oder Erneuern des Server-Lizenzgeberzertifikats.** Sie können das Server-Lizenzgeberzertifikat für den Cluster registrieren oder erneuern.
-   **Einrichten von Vertrauensrichtlinien.** Klicken Sie auf den Link, um die Webseite „Vertrauensrichtlinien“ zu öffnen, auf der Sie vertrauenswürdige Benutzerdomänen und Veröffentlichungsdomänen hinzufügen oder entfernen können. Fügen Sie Benutzer zur Ausschlussliste in einer vertrauenswürdigen Benutzerdomäne hinzu, oder entfernen Sie Benutzer aus dieser Liste. Exportieren Sie das Server-Lizenzgeberzertifikat in eine Datei, damit es von einer anderen RMS-Installation importiert werden kann.
-   **Konfigurieren von Vorlagen für Benutzerrechterichtlinien.** Klicken Sie auf den Link, um die Webseite „Vorlagen für Benutzerrechterichtlinien“ zu öffnen, auf der Sie Vorlagen für Benutzerrechterichtlinien für das Unternehmen erstellen und ändern können.
-   **Konfigurieren der Protokollierung.** Klicken Sie auf den Link, um die Webseite „Protokollierungseinstellungen“ zu öffnen, auf der Sie die Protokollierung aktivieren und deaktivieren sowie den Server und die Datenbank für Protokollierung anzeigen können.
-   **Angeben des Extranet-Cluster-URLs.** Klicken Sie auf den Link, um die Webseite „Einstellungen für Extranet-Cluster-URL“ zu öffnen, auf der Sie die URL angeben können, die für den Zugriff auf Zertifizierungsdienste des Stammclusters vom Extranet aus verwendet werden soll.
-   **Konfigurieren von RMS-Proxyeinstellungen.** Klicken Sie auf den Link, um die Webseite „RMS-Proxyeinstellungen“ zu öffnen, auf der Sie die Adresse des Proxyservers, den Authentifizierungstyp und den Benutzernamen angeben können, der verwendet werden soll, wenn der RMS-Server über den Proxyserver eine Verbindung zum Internet herstellen muss.
-   **Nachverfolgen der Anzahl von ausgestellten Rechtekontozertifikaten.** Klicken Sie auf den Link, um die Webseite „Nachverfolgen von Rechtekontozertifikaten“ zu öffnen, auf der Sie anzeigen können, wie viele Rechtekontozertifikate vom Stammcluster verteilt wurden. Anhand dieser Anzahl können Sie die Anzahl der benötigten Clientzugriffslizenzen (Client Access Licenses oder CALs) abschätzen.
-   **Verwalten von Sicherheitseinstellungen.** Klicken Sie auf den Link, um die Webseite „Sicherheitseinstellungen“ zu öffnen, auf der Sie Mitglieder der Administratorengruppe, die vollständige Kontrolle über den gesamten lizenzierten Inhalt haben, hinzufügen und entfernen sowie das Kennwort für den privaten Schlüssel zurücksetzen können.
-   **Anzeigen und Konfigurieren von Kontozertifikatseinstellungen.** Klicken Sie auf den Link, um die Webseite „Zertifizierungseinstellungen“ zu öffnen, auf der Sie die Gültigkeitsdauer des Zertifikats sowie einen Administratorkontakt angeben können.
-   **Aktivieren von Ausschlussrichtlinien.** Klicken Sie auf den Link, um die Webseite „Ausschlussrichtlinien“ zu öffnen, auf der Sie Ausschlussrichtlinien aktivieren können, die auf Lockbox-Versionen, Windows-Versionen, Kontozertifikaten und Anwendungen basieren können.
-   **Registrieren des Dienstverbindungspunktes.** Klicken Sie auf den Link, um die Webseite „Dienstverbindungspunkt“ zu öffnen, auf der Sie den Dienstverbindungspunkt für Ihr Cluster registrieren und seine Registrierung wieder aufheben können.

Administratoren können über die Microsoft Management Console (MMC) weitere Aufgaben ausführen, darunter das Überwachen von Ereignissen sowie das Verwalten von Active Directory, Internetinformationsdienste (Internet Information Services oder IIS) und SQL Server.