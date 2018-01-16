---
TOCTitle: So bearbeiten Sie eine Vorlage für Benutzerrechterichtlinien
Title: So bearbeiten Sie eine Vorlage für Benutzerrechterichtlinien
ms:assetid: '9580b934-bd6f-4097-9d3c-4fc14a3147fa'
ms:contentKeyID: 18119004
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747684(v=WS.10)'
---

So bearbeiten Sie eine Vorlage für Benutzerrechterichtlinien
============================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Bearbeiten von Vorlagen für Benutzerrechterichtlinien
-----------------------------------------------------

#### So bearbeiten Sie eine Vorlage für Benutzerrechterichtlinien

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie eine Vorlage für Benutzerrechterichtlinien bearbeiten möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Vorlagen für Benutzerrechterichtlinien**.

3.  Klicken Sie unter **Vorlagenname** auf den Namen der zu bearbeitenden Vorlage.

4.  Ändern Sie im Bereich **Vorlagenidentifikation** die erforderlichen Informationen in den Bereichen **Vorlagenname**, **Vorlagenbeschreibung** und **URL zur Anforderung von Rechten**.

5.  Führen Sie im Bereich **Benutzer und Gruppen** einen oder mehrere der folgenden Schritte aus:

    -   Geben Sie in das Feld **Benutzer oder Gruppen hinzufügen** die gültige E-Mail-Adresse eines hinzuzufügenden bestimmten Benutzers oder einer Gruppe ein, klicken Sie auf **Hinzufügen**, und wählen Sie dann den Namen im Feld **Aktuelle Benutzer oder Gruppen** aus, um einen Benutzer oder eine Gruppe hinzuzufügen. Wählen Sie im Bereich **Rechte** alle Rechte aus, die dem ausgewählten Benutzer oder der Gruppe erteilt werden sollen.
    -   Zum Ändern der Rechte eines bestehenden Benutzers oder einer bestehenden wählen Sie den Namen im Feld **Aktuelle Benutzer oder Gruppen** aus, und aktivieren oder deaktivieren Sie dann die entsprechenden Kontrollkästchen.
    -   Zum Entfernen eines Benutzers oder einer Gruppe wählen Sie den Namen im Feld **Aktuelle Benutzer oder Gruppen** aus, und klicken Sie dann auf **Entfernen**.

6.  Bearbeiten Sie im Bereich **Ablaufrichtlinie** die zu ändernden Informationen, wenn Inhaltslizenzen ablaufen und erneuert werden müssen.

7.  Bearbeiten Sie im Bereich **Erweiterte Richtlinie** die ggf. zu ändernden Informationen zum Implementieren von Inhaltslizenzen, einschließlich der Dauer der Autorenrechte, der Unterstützung vertrauenswürdiger Browser, Lizenzdauerhaftigkeit innerhalb des Inhalts und Erzwingen anwendungsspezifischer Daten.

8.  Wählen Sie im Bereich **Sperrrichtlinie** aus, ob eine Sperrliste für Inhalte erforderlich ist, die mithilfe dieser Vorlage erstellt werden. Wenn Sie die Option **Sperrung verlangen** auswählen, vervollständigen Sie die folgenden Einstellungen:

    -   Geben Sie im Feld **URL** den URL ein, an dem die Sperrlistendatei gespeichert ist. Wenn nicht verbundene Benutzer oder externe Benutzer unterstützt werden sollen, muss auf diesen URL über das Unternehmensnetzwerk sowie über das Internet zugegriffen werden können. Weitere Informationen hierzu finden Sie oben unter [Implementieren der Sperrung](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a).
    -   Geben Sie in das Feld **Aktualisierungsintervall für Sperrliste** die Anzahl von Tagen ein, die die Sperrliste gültig sein soll. Wenn ein Benutzer über eine Kopie der Sperrliste verfügt, die älter als dieser angegebene Wert ist, muss der Benutzer eine aktualisierte Sperrliste erhalten, um Inhalte abzurufen.
    -   Geben Sie in das Feld **Öffentliche Schlüsseldatei** den Pfad und den Dateinamen der Datei des öffentlichen Schlüssels für die Sperrliste ein. Weitere Informationen zu dieser Datei finden Sie oben unter „Einfügen einer Signatur in eine Sperrliste“.

    | ![](images/Cc747684.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Gehen Sie bei der Implementierung von Sperrung vorsichtig vor. Eine Sperrliste muss basierend auf dem angegebenen Aktualisierungsintervall regelmäßig aktualisiert werden. Erfolgt keine Aktualisierung, läuft die Sperrliste ab und Benutzer können Inhalte, für die diese Liste erforderlich ist, nicht abrufen. Legen Sie das Aktualisierungsintervall für die Sperrliste mit Sorgfalt fest, um sicherzustellen, dass Benutzer nicht unbeabsichtigt am Abrufen von Inhalten gehindert werden. Weitere Informationen hierzu finden Sie oben unter [Verwalten der Sperrung](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0). |

9.  Klicken Sie auf **Absenden**.

Weitere Informationen zum Ausführen dieses Verfahrens finden Sie oben unter [Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).