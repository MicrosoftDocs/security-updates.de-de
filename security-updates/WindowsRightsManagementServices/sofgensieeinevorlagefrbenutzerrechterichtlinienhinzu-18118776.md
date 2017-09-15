---
TOCTitle: So fügen Sie eine Vorlage für Benutzerrechterichtlinien hinzu
Title: So fügen Sie eine Vorlage für Benutzerrechterichtlinien hinzu
ms:assetid: '1a5555cd-6d39-4078-a879-4106864674be'
ms:contentKeyID: 18118776
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720206(v=WS.10)'
---

So fügen Sie eine Vorlage für Benutzerrechterichtlinien hinzu
=============================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Hinzufügen von Vorlagen für Benutzerrechterichtlinien
-----------------------------------------------------

#### So fügen Sie eine Vorlage für Benutzerrechterichtlinien hinzu

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie eine Vorlage für Benutzerrechterichtlinien hinzufügen möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Vorlagen für Benutzerrechterichtlinien**.

3.  Klicken Sie im Bereich **Sprache** auf die Sprache, die in der Vorlage verwendet werden soll.

4.  Klicken Sie auf **Vorlagen für Benutzerrechterichtlinien hinzufügen**.

5.  Geben Sie im Bereich **Vorlagenidentifikation** einen Namen, eine Beschreibung und den URL (Uniform Resource Locator) zur Anforderung von Rechten für die Vorlage an.

6.  Geben Sie im Bereich **Benutzer und Gruppen** unter **Benutzer und Gruppen hinzufügen** die gültige E-Mail-Adresse eines hinzuzufügenden Benutzers oder einer Gruppe ein, und klicken Sie dann auf **Hinzufügen**. Wiederholen Sie bei Bedarf diesen Schritt, um weitere Benutzer oder Gruppen hinzuzufügen.

7.  Wählen Sie unter **Aktuelle Benutzer oder Gruppen** die E-Mail-Adresse eines Benutzers oder einer Gruppe aus, dem bzw. der Rechte zugewiesen werden sollen.

8.  Aktivieren Sie die Kontrollkästchen der Rechte, die dem ausgewählten Benutzer oder der Gruppe erteilt werden sollen. Wiederholen Sie diesen Schritt, um den weiteren Benutzern und Gruppen Rechte zu erteilen.

9.  Wählen Sie im Bereich **Ablaufrichtlinie** eine der drei Ablaufoptionen aus, und geben Sie dann ein geeignetes Ablaufdatum oder eine Ablaufzeit an. Wählen Sie gegebenenfalls die Option **Nutzungslizenzen für Inhalte müssen erneuert werden alle** aus, und geben Sie die Anzahl von Tagen zwischen den Aktualisierungen an.

10. Wählen Sie im Bereich **Erweiterte Richtlinie** eine oder mehrere der vier Optionen aus. Wenn Sie **Anwendungsspezifische Daten erzwingen** auswählen, geben Sie einen Namen und einen Wert für die zu erzwingenden Daten an, und klicken Sie auf **Hinzufügen**.

11. Zum Implementieren von Sperrung aktivieren Sie im Bereich **Sperrrichtlinie** das Kontrollkästchen **Sperrung verlangen**, und führen Sie dann die folgenden Schritte aus:

    1.  Geben Sie im Feld **URL oder UNC** den URL ein, an dem die Sperrlistendatei gespeichert ist. Wenn nicht verbundene Benutzer oder externe Benutzer unterstützt werden sollen, muss auf diesen URL über das Unternehmensnetzwerk sowie über das Internet zugegriffen werden können.
    2.  Geben Sie in das Feld **Aktualisierungsintervall für Sperrliste** die Anzahl von Tagen ein, die die Sperrliste gültig sein soll. Wenn ein Benutzer über eine Kopie der Sperrliste verfügt, die älter als dieser angegebene Wert ist, muss der Benutzer eine aktualisierte Sperrliste erhalten, um Inhalte abzurufen.
    3.  Geben Sie in das Feld **Öffentliche Schlüsseldatei** den Pfad und den Dateinamen ein, oder klicken Sie auf **Durchsuchen**, um die Datei mit dem öffentlichen Schlüssel für die Sperrliste zu suchen. Weitere Informationen zu dieser Datei finden Sie oben unter „Einfügen einer Signatur in eine Sperrliste“.

    | ![](images/Cc720206.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Gehen Sie bei der Implementierung von Sperrung vorsichtig vor. Eine Sperrliste muss basierend auf dem angegebenen Aktualisierungsintervall regelmäßig aktualisiert werden. Erfolgt keine Aktualisierung, läuft die Sperrliste ab und Benutzer können Inhalte, für die diese Liste erforderlich ist, nicht abrufen. Legen Sie das Aktualisierungsintervall für die Sperrliste mit Sorgfalt fest, um sicherzustellen, dass Benutzer nicht unbeabsichtigt am Abrufen von Inhalten gehindert werden. Weitere Informationen finden Sie oben unter „[Verwalten der Sperrung](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)“. |

12. Klicken Sie auf **Absenden**.

Weitere Informationen zur Sperrung finden Sie oben unter „[Verwalten der Sperrung](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)“.

Überlegungen zum Festlegen von Sperroptionen finden Sie oben unter „[Definieren von Sperrrichtlinien](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)“.

Weitere Informationen zum Ausführen dieses Verfahrens finden Sie oben unter „[Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)“.
