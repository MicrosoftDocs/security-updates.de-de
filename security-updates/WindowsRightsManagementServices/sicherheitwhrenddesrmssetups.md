---
TOCTitle: 'Sicherheit während des RMS-Setups'
Title: 'Sicherheit während des RMS-Setups'
ms:assetid: '0a3d40b2-f27e-4e63-baff-a9c8433f5f91'
ms:contentKeyID: 18118757
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720192(v=WS.10)'
---

Sicherheit während des RMS-Setups
=================================

RMS-Setup nutzt die Informationen des angemeldeten Benutzers für die Installation und Konfiguration von RMS-Dateien. Zu diesem Zweck muss der Administrator, der den Installationsvorgang ausführt, mit einem Benutzerkonto, das Mitglied der lokalen Gruppe Administratoren ist, angemeldet sein. Für alle Installationen, mit Ausnahme von Einzelcomputerinstallationen, muss es sich dabei außerdem um ein Domänenbenutzerkonto handeln.

Während des Installationsvorgangs wird der Windows Installer-Dienst (Msiexec.exe) gestartet. Dieser Dienst erbt das entsprechende übergeordnete Benutzertoken. Wenn zu einem späteren Zeitpunkt die benutzerdefinierten Nachverarbeitungsaktionen erfolgen, verwendet der Dienst Msiexec.exe die Identität des angemeldeten Benutzers. Dies geschieht unabhängig davon, ob der Prozess in einem Browser oder über die Befehlszeile gestartet wurde.

Die folgenden Aufgaben werden von RMS-Setup übergenommen:

-   Kopiert Dateien in den Ordner C:\\Programme\\RMS. Auf diesen Ordner können normalerweise sowohl Administratoren als auch Hauptbenutzer zugreifen. Sie können das Laufwerk und den Dateipfad beim Ausführen von Setups konfigurieren.
-   Erstellt eine Bereitstellungswebsite, die Verwaltungswebsite für RMS, standardmäßig auf Port 5720. Diese Website ist mit den installierten Dateien verknüpft.
-   Erstellt einen Anwendungspool (WMCSProvisioningAppPool) und verknüpft ihn mit der RMS-Verwaltungswebsite. Dieser Anwendungspool verwendet das Dienstkonto Netzwerkdienste.
-   Installiert Leistungsindikatoren.
-   Gewährt der RMS-Dienstgruppe Lese- und Schreibrechte für den folgenden Registrierungsschlüssel.

    Auf Computern mit der 32-Bit-Version von Windows Server 2003:

    ```
    HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0
    ```

    Auf Computern mit der 64-Bit-Version von Windows Server 2003:

    ```
    HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0
    ```