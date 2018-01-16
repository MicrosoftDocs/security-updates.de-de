---
TOCTitle: 'Verteilen des RMS-Clients'
Title: 'Verteilen des RMS-Clients'
ms:assetid: '4b8dd930-4105-4e73-918c-12d2b05d5fb5'
ms:contentKeyID: 18118834
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720266(v=WS.10)'
---

Verteilen des RMS-Clients
=========================

Der RMS-Client ist in das Windows Vista®-Betriebssystem integriert, so dass es sich bei ihm nicht mehr um ein separates Programm handelt. Bei Betriebssystemen vor Windows Vista müssen Sie die RMS-Client-Software installieren und aktivieren.

Durch den Aktivierungsprozess werden eine Lockbox und ein Computerzertifikat für den aktuell angemeldeten Benutzer erstellt. Bei der Aktivierung handelt es sich um ein lokales Verfahren, das keine Netzwerkverbindung erfordert. Nach erfolgreicher Aktivierung erhält der Benutzer nach der ersten Nutzung von RMS durch eine aktivierte Anwendung ein Benutzerzertifikat. Der RMS-Client kann auf allen Clientcomputern in der Organisation anhand der Gruppenrichtlinie, von Windows Update oder einem Verwaltungsskript ausgeführt werden.

> [!NOTE]
> Unabhängig davon, welche Clientverteilungsmethode eingesetzt wird, verwendet der RMS-Client entweder Port 80 oder Port 443 zur Kommunikation mit dem RMS-Server. Sie sollten sicherstellen, dass der Clientcomputer an diesen Ports ausgehende Anforderungen an das RMS-Stammverzeichnis und den Lizenzierungscluster durchführen kann. 

**Verwenden einer Gruppenrichtlinie**

Wird in Ihrem Unternehmen Software mithilfe der Gruppenrichtlinie verteilt, können Sie diese Methode zum Verteilen des RMS-Clients verwenden. Bei einer derartigen Verteilung des RMS-Clients benötigt der Benutzer keine Administratorrechte und kann den RMS-Client entweder mithilfe von **Software** unter **Systemsteuerung** oder durch das Öffnen von RMS-geschützten Inhalten mit einer RMS-fähigen Anwendung installieren.

**Verwenden von Windows Update**

Windows Update stellt die einfachste Möglichkeit zur Installation des RMS-Clients auf einem Computer dar. Diese Methode hat den Vorteil, dass die Benutzer mit dem Mechanismus vertraut sind. Es ist jedoch erforderlich, dass der Benutzer, der den RMS-Client installiert, über lokale Administratorrechte auf dem Computer verfügt.

**Verwenden von Skriptinstallation**

Zur höchstmöglichen Kontrolle über das Verfahren der Clientinstallation können Sie die Software erwerben und danach deren Integrität bei jedem Schritt des Installationsverfahrens durch das Ausführen eines Skripts validieren. Dieses Skript kann geschrieben und einem Gruppenrichtlinienobjekt (Group Policy Object oder GPO) als Startskript hinzugefügt werden. Mit dieser Methode muss der Benutzer nicht als lokaler Administrator auf dem Computer angemeldet sein, und der RMS-Client wird automatisch beim Neustart installiert.

Im Folgenden finden Sie ein Beispielskript:

```
Set objShell = Wscript.CreateObject("Wscript.Shell")
objShell.run "WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q"
```
Grundlegende Informationen über das Verteilen des RMS-Clients anhand einer Gruppenrichtlinie finden Sie nachstehend unter [Einrichten von SMS oder einer Gruppenrichtlinie zur Unterstützung der Clientbereitstellung](https://technet.microsoft.com/9e37c27b-8cc1-40c6-adb7-0937aa64c8db).

Verfahrensrichtlinien zur RMS-Clientbereitstellung finden Sie nachstehend unter [So stellen Sie den RMS-Client bereit](https://technet.microsoft.com/c84f1724-cf71-4385-9003-ff68bc23c927).
