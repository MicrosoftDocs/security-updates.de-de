---
TOCTitle: 'Schritt 5: Konfigurieren von automatischen Updates'
Title: 'Schritt 5: Konfigurieren von automatischen Updates'
ms:assetid: '5da6d10a-6ff1-4de8-b53a-4893bf8bd9fa'
ms:contentKeyID: 18127466
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720532(v=WS.10)'
---

Schritt 5: Konfigurieren von automatischen Updates
==================================================

Für WSUS-Clientcomputer ist eine kompatible Version der automatischen Updates erforderlich. WSUS Setup konfiguriert Internetinformationsdienste (Internet Information Services, IIS) automatisch so, dass die neueste Version der automatischen Updates an jeden Clientcomputer verteilt wird, der eine Verbindung mit dem WSUS-Server herstellt.

Welche Methode zum Konfigurieren von automatischen Updates die beste ist, ist abhängig von Ihrer Netzwerkumgebung. In einer Umgebung mit Active Directory können Sie ein Gruppenrichtlinienobjekt (Group Policy Object, GPO) der Domäne verwenden. In einer Umgebung ohne Active Directory können Sie das lokale Gruppenrichtlinienobjekt verwenden. Sowohl mit dem lokalen als auch mit einem domänenbasierten Gruppenrichtlinienobjekt müssen Ihre Clientcomputer zunächst dem WSUS-Server zugeordnet werden. Anschließend können automatische Updates konfiguriert werden.

In den folgenden Anleitungen wird davon ausgegangen, dass auf Ihrem Netzwerk Active Directory ausgeführt wird. Außerdem wird davon ausgegangen, dass Sie mit Gruppenrichtlinien vertraut sind und diese für die Verwaltung Ihres Netzwerks verwenden. Sie müssen für die WSUS-Einstellungen ein neues GPO erstellen und dieses mit der Domäne verknüpfen.

Weitere Informationen zu Gruppenrichtlinien finden Sie auf der Tech Center-Website über Gruppenrichtlinien unter [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375) (möglicherweise in englischer Sprache).

**Schritt 5 umfasst die folgenden Verfahren**:

-   Hinzufügen der administrativen Vorlage für WSUS
-   Konfigurieren der automatischen Updates
-   Zuordnen der Clientcomputer zum WSUS-Server
-   Manuelles Starten der Erkennung durch den WSUS-Server

Führen Sie die ersten drei Verfahren mithilfe eines Gruppenrichtlinienobjekts der Domäne aus. Sie müssen entweder ein neues GPO erstellen oder ein bereits vorhandenes verwenden. Wenn Sie die Group Policy Management Console (GPMC) verwenden, um Ihre GPOs zu verwalten, navigieren Sie zu dem GPO, das Sie ändern möchten, und klicken Sie anschließend auf **Bearbeiten**.

Um die Richtlinieneinstellungen zur Verwaltung von WSUS anzuzeigen, müssen Sie sicherstellen, dass die Datei der administrativen Vorlage für WSUS, "wuau.adm", dem Gruppenrichtlinienobjekt-Editor hinzugefügt wurde. Da in der Standardeinstellung "wuau.adm" vom Betriebssystem freigegeben ist, sollte diese Datei im Gruppenrichtlinienobjekt-Editor bereits vorhanden sein.

**So fügen Sie die administrative Vorlage für WSUS hinzu**
1.  Klicken Sie im Gruppenrichtlinienobjekt-Editor auf einen der Knoten **Administrative Vorlagen**.

2.  Klicken Sie im Menü **Aktion** auf **Vorlagen hinzufügen/entfernen**, und klicken Sie anschließend auf **Hinzufügen**.

3.  Klicken Sie im Dialogfeld **Richtlinienvorlagen** auf **wuau.adm**, und klicken Sie dann auf **Öffnen**.

4.  Klicken Sie im Dialogfeld **Vorlagen hinzufügen/entfernen** auf **Schließen**.

**So konfigurieren Sie automatische Updates**
1.  Erweitern Sie im Gruppenrichtlinienobjekt-Editor zuerst **Computerkonfiguration**, dann **Administrative Vorlagen**, dann **Windows-Komponenten**, und klicken Sie anschließend auf **Windows Update**.

2.  Doppelklicken Sie im Detailfenster auf **Automatische Updates konfigurieren**.

3.  Klicken Sie auf **Aktiviert**, und klicken Sie dann auf eine der folgenden Optionen:

    -   **Vor Download und Installation benachrichtigen**: Mit dieser Option wird ein angemeldeter Administrator vor dem Download und vor der Installation der Updates benachrichtigt.
    -   **Autom. Herunterladen, aber vor Installation benachrichtigen**: Mit dieser Option wird das Herunterladen von Updates automatisch begonnen. Anschließend wird ein angemeldeter Administrator vor dem Installieren der Updates benachrichtigt.
    -   **Autom. Herunterladen und laut Zeitplan installieren**: Wenn automatische Updates für eine geplante Installation konfiguriert sind, müssen Sie auch den Tag und die Uhrzeit für die geplante wiederholte Installation angeben.
    -   **Lokalen Administratoren ermöglichen, Einstellung auszuwählen**: Mit dieser Option können lokale Administratoren mithilfe der Option "Automatische Updates" in der Systemsteuerung eine Konfigurationsoption auswählen. Sie können beispielsweise den Zeitpunkt für eine Installation planen. Lokale Administratoren können die automatischen Updates nicht deaktivieren.

4.  Klicken Sie auf **OK**.

| ![](images/Cc720532.note(WS.10).gif)Hinweis                                                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Die Einstellung **Lokalen Administratoren ermöglichen, Einstellung auszuwählen** wird nur angezeigt, wenn die automatischen Updates auf die mit WSUS kompatible Version aktualisiert wurden. |

**So ordnen Sie den Clientcomputer dem WSUS-Server zu**
1.  Erweitern Sie im Gruppenrichtlinienobjekt-Editor zuerst **Computerkonfiguration**, dann **Administrative Vorlagen**, dann **Windows-Komponenten**, und klicken Sie anschließend auf **Windows Update**.

2.  Doppelklicken Sie im Detailfenster auf **Internen Pfad für den Microsoft Updatedienst angeben**.

3.  Klicken Sie auf **Aktiviert**, und geben Sie die HTTP-URL des WSUS-Servers sowohl im Feld **Interner Updatedienst zum Ermitteln von Updates** als auch im Feld **Intranetserver für die Statistiken** ein. Geben Sie z. B. *http://Servername* in beiden Feldern ein, und klicken Sie anschließend auf **OK**.

| ![](images/Cc720532.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie diesen Computer dem WSUS-Server mithilfe des lokalen Gruppenrichtlinienobjekts zuordnen, wird diese Einstellung sofort wirksam, und der Computer sollte nach kurzer Zeit in der WSUS-Verwaltungskonsole angezeigt werden. Sie können diesen Vorgang beschleunigen, indem Sie den Erkennungszyklus manuell starten. |

Nach dem Einrichten eines Clientcomputers dauert es einige Minuten, bis dieser auf der Seite **Computer** in der WSUS-Konsole angezeigt wird. Bei Clientcomputern, die mithilfe einer domänenbasierten Gruppenrichtlinie konfiguriert wurden, dauert dies nach dem Aktualisieren der Gruppenrichtlinie (d. h. nach dem Anwenden neuer Einstellungen auf den Clientcomputer) ca. 20 Minuten. In der Standardeinstellung werden Gruppenrichtlinien alle 90 Minuten, mit einer zufälligen Verzögerung von bis zu 30 Minuten, im Hintergrund aktualisiert. Wenn Sie Gruppenrichtlinien in kürzeren Abständen aktualisieren möchten, können Sie an einer Eingabeaufforderung auf dem Clientcomputer Folgendes eingeben: **gpupdate /force**.

Auf Clientcomputern, die mithilfe des lokalen GPOs konfiguriert wurden, wird die Gruppenrichtlinie sofort angewendet, und die Aktualisierung dauert ca. 20 Minuten.

Nach dem Anwenden der Gruppenrichtlinie können Sie die Erkennung manuell starten. Wenn Sie die Erkennung manuell starten, müssen Sie nicht 20 Minuten warten, bis der Clientcomputer eine Verbindung zu WSUS herstellt.

**So starten Sie die Erkennung durch den WSUS-Server manuell**
1.  Klicken Sie auf dem Clientcomputer auf **Start** und anschließend auf **Ausführen**.

2.  Geben Sie **cmd** im Feld **Öffnen** ein, und klicken Sie anschließend auf **OK**.

3.  Geben Sie in der Eingabeaufforderung **wuauclt.exe /detectnow** ein. Diese Befehlszeilenoption weist die Funktion "Automatische Updates" an, sofort eine Verbindung zum WSUS-Server herzustellen.
