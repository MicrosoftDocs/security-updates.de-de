---
TOCTitle: So beenden Sie die Bereitstellung von RMS
Title: So beenden Sie die Bereitstellung von RMS
ms:assetid: '9fa63daa-5fb9-4afd-8371-b38248619857'
ms:contentKeyID: 18119024
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747706(v=WS.10)'
---

So beenden Sie die Bereitstellung von RMS
=========================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Wenn Sie die Bereitstellung eines Servers beenden, wird dieser aus der Tabelle „ClusterServer“ in der Konfigurationsdatenbank entfernt. Wenn Sie die Bereitstellung für den letzten Server in einem Cluster beenden, wird die Datenbank der Verzeichnisdienste in SQL Server gelöscht. Wenn Sie die Bereitstellung des letzten Stammzertifizierungsservers in einem Cluster beenden, müssen Sie die Registrierung des Verbindungspunktes des Zertifizierungsdienstes (Service Connection Point oder SCP) manuell aufheben. Das Beenden der Bereitstellung und das Deinstallieren führen nicht dazu, dass der Dienstverbindungspunkt aus Active Directory entfernt wird.

Wenn Sie einen Stammzertifizierungsserver vor der Bereitstellung deinstallieren, erhalten Sie die Warnung, dass die Site noch nicht bereitgestellt wurde und dass der Dienstverbindungspunkt nicht aus Active Directory entfernt wird. Wenn Sie **Ja** auswählen, um den Vorgang fortzusetzen, wird die Bereitstellung der Site für Sie beendet. Das Deinstallieren führt nicht dazu, dass der Dienstverbindungspunkt aus Active Directory entfernt wird.

Beenden der Bereitstellung von RMS
----------------------------------

#### So beenden Sie die Bereitstellung von RMS

1.  Melden Sie sich an dem Server an, auf dem Sie die Bereitstellung von RMS (Rights Management Services oder Dienste für die Rechteverwaltung) beenden möchten.

2.  Öffnen Sie die Seite **Globale Verwaltung**.

3.  Klicken Sie neben der Website, auf der RMS bereitgestellt wird, auf **RMS von dieser Website entfernen**, und klicken Sie dann auf **OK**.

4.  Klicken Sie auf der Webseite für den RMS-Dienstverbindungspunkt auf **URL-Registrierung aufheben**, um die Registrierung der Zertifizierungsdienstverbindung in Active Directory aufzuheben.
