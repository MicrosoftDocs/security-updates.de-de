---
TOCTitle: So aktivieren oder deaktivieren Sie die Protokollierung
Title: So aktivieren oder deaktivieren Sie die Protokollierung
ms:assetid: '8e672f95-566f-4070-9a2a-2f70f087148f'
ms:contentKeyID: 18118931
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747674(v=WS.10)'
---

So aktivieren oder deaktivieren Sie die Protokollierung
=======================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Stellen Sie sicher, dass der Server mit RMS eine Verbindung zum Datenbankserver hat und dass der Datenbankdienst vor dem Aktivieren der Protokollierung gestartet wurde. Wenn Message Queuing die Protokolle nicht an die Protokollierungsdatenbank liefern kann, bleiben die Daten in einer Warteschlange auf der Festplatte des Servers mit RMS gespeichert. Dieser Vorgang wird fortgesetzt, bis der gesamte Speicherplatz des Servers belegt ist. RMS zeigt für diesen Umstand keine Fehlermeldung an, da diese Funktion nur zur Unterstützung der Protokollierung während einer Verbindungsunterbrechung zum SQL-Server vorgesehen ist.

Protokollierung aktivieren und deaktivieren
-------------------------------------------

#### So aktivieren oder deaktivieren Sie die Protokollierung

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie Protokollierung aktivieren oder deaktivieren möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Protokollierungseinstellungen**.

3.  Aktivieren Sie im Bereich **Protokollierungsserver und-datenbank** das Kontrollkästchen **Protokollierung aktivieren**, und klicken Sie dann auf **Aktualisieren**.

    Deaktivieren Sie das Kontrollkästchen, und klicken Sie dann auf **Aktualisieren**, um die Protokollierung zu deaktivieren.

Weitere Informationen zum Ausführen dieses Verfahrens finden Sie oben unter [Aktivieren und Deaktivieren der Protokollierung](https://technet.microsoft.com/50ccd827-2d39-41e7-a395-3d5f5836869b).