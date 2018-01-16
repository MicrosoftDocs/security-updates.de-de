---
TOCTitle: 'Schritt 5: Aktualisieren und Konfigurieren der automatischen Updates'
Title: 'Schritt 5: Aktualisieren und Konfigurieren der automatischen Updates'
ms:assetid: '4ac8d574-f48e-4d9d-86c9-9aeb0f57e750'
ms:contentKeyID: 18127452
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720533(v=WS.10)'
---

Schritt 5: Aktualisieren und Konfigurieren der automatischen Updates
====================================================================

Für WSUS-Clientcomputer ist eine kompatible Version der automatischen Updates erforderlich. WSUS Setup konfiguriert Internetinformationsdienste (Internet Information Services, IIS) automatisch so, dass die neueste Version der automatischen Updates an jeden Clientcomputer verteilt wird, der den WSUS-Server kontaktiert.

> [!NOTE]
> Die meisten Versionen der automatischen Updates können auf den WSUS-Server verwiesen werden und aktualisieren sich automatisch auf die WSUS-kompatible Version. Die Version der automatischen Updates, die Bestandteil von Windows XP ohne Service Packs ist, kann sich jedoch nicht automatisch aktualisieren. Wenn in Ihrer Umgebung Windows XP ohne Service Packs vorhanden ist und Sie Software Update Services (SUS) bisher noch nicht verwendet haben, lesen Sie die Anweisung im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache). 

Die beste Möglichkeit, die automatischen Updates zu konfigurieren, richtet sich nach Ihrer Netzwerkumgebung. In einer Active Directory-Umgebung können Sie ein Active Directory-basiertes Gruppenrichtlinienobjekt verwenden. Verwenden Sie in anderen Umgebungen das Richtlinienobjekt der lokalen Gruppe. Wenn Sie das Richtlinienobjekt der lokalen Gruppe oder ein auf einem Domänencontroller gespeichertes Gruppenrichtlinienobjekt verwenden, müssen Sie Ihre Clientcomputer auf den WSUS-Server verweisen und dann die automatischen Updates konfigurieren.

Die folgenden Anweisungen gelten für Netzwerke, in denen Active Directory ausgeführt wird. Diese Verfahren setzen auch voraus, dass Sie bereits Gruppenrichtlinien eingerichtet haben, mit ihnen vertraut sind und sie für die Netzwerkverwaltung verwenden. Sie müssen ein neues Gruppenrichtlinienobjekt für WSUS-Einstellungen erstellen und das Gruppenrichtlinienobjekt auf Domänenebene verknüpfen.

Weitere Informationen zu Gruppenrichtlinien finden Sie auf der Seite zu [Gruppenrichtlinien](http://go.microsoft.com/fwlink/?linkid=47375) unter **http://go.microsoft.com/fwlink/?LinkID=47375** (möglicherweise in englischer Sprache).

Schritt 5 umfasst die folgenden Verfahren:

-   Laden der administrativen Vorlage für WSUS.
-   Konfigurieren der automatischen Updates.
-   Verweisen der Clientcomputer auf den WSUS-Server.
-   Manuelles Initiieren der Ermittlung auf dem Clientcomputer.

Führen Sie die drei folgenden Verfahren für ein Active Directory-basiertes Gruppenrichtlinienobjekt aus.

**So fügen Sie die administrative Vorlage für WSUS hinzu**
1.  Klicken Sie im Gruppenrichtlinienobjekt-Editor auf einen der Knoten **Administrative Vorlagen**.

2.  Klicken Sie im Menü **Aktion** auf **Vorlagen hinzufügen/entfernen**.

3.  Klicken Sie auf **Hinzufügen**.

4.  Klicken Sie im Dialogfeld **Richtlinienvorlagen** auf **wuau.adm**, und klicken Sie dann auf **Öffnen**.

5.  Klicken Sie im Dialogfeld **Vorlagen hinzufügen/entfernen** auf **Schließen**.

**So konfigurieren Sie das Verhalten der automatischen Updates**
1.  Erweitern Sie im Gruppenrichtlinienobjekt-Editor zuerst **Computerkonfiguration**, dann **Administrative Vorlagen**, dann **Windows-Komponenten**, und klicken Sie anschließend auf **Windows Update**.

2.  Doppelklicken Sie im Detailfenster auf **Automatische Updates konfigurieren**.

3.  Klicken Sie auf **Aktiviert**, und klicken Sie dann auf eine der folgenden Optionen:

    -   **Vor Download und Installation benachrichtigen** Mit dieser Option wird ein angemeldeter Administrator vor dem Download und vor der Installation der Updates benachrichtigt.
    -   **Autom. Downloaden, aber vor Installation benachrichtigen** Mit dieser Option wird das Downloaden von Updates automatisch begonnen, und anschließend wird ein angemeldeter Administrator vor dem Installieren der Updates benachrichtigt.
    -   **Autom. Downloaden und laut Zeitplan installieren** Wenn automatische Updates für eine geplante Installation konfiguriert sind, müssen Sie auch den Tag und die Uhrzeit für die wiederholt geplante Installation angeben.
    -   **Lokalen Administrator ermöglichen, Einstellung auszuwählen** Mit dieser Option lassen Sie zu, dass lokale Administratoren mithilfe der Option **Automatische Updates** in der Systemsteuerung eine gewünschte Konfigurationsoption auswählen. Sie können z. B. einen Zeitpunkt für eine Installation nach Zeitplan auswählen. Lokale Administratoren können die automatischen Updates nicht deaktivieren.

4.  Klicken Sie auf **OK**.

> [!NOTE]
> Die Einstellung **Lokalen Administrator ermöglichen, Einstellung auszuwählen** wird nur angezeigt, wenn die automatischen Updates sich automatisch auf die mit WSUS kompatible Version aktualisiert haben. 

**So verweisen Sie Clientcomputer auf den WSUS-Server**
1.  Erweitern Sie im Gruppenrichtlinienobjekt-Editor zuerst **Computerkonfiguration**, dann **Administrative Vorlagen**, dann **Windows-Komponenten**, und klicken Sie anschließend auf **Windows Update**.

2.  Doppelklicken Sie im Detailfenster auf **Internen Pfad für den Microsoft Updatedienst angeben**.

3.  Klicken Sie auf **Aktiviert**, und geben Sie den HTTP-URL des WSUS-Servers sowohl im Feld **Interner Updatedienst zum Ermitteln von Updates** als auch im Feld **Intranetserver für die Statistiken** ein. Geben Sie z. B. **http://***Servername* in beiden Feldern ein.

4.  Klicken Sie auf **OK**.

> [!NOTE]
> Wenn Sie diesen Computer mithilfe des Richtlinienobjekts der lokalen Gruppe auf WSUS verweisen, wird diese Einstellung sofort wirksam, und der Computer sollte nach ca. 20 Minuten in der WSUS-Verwaltungskonsole angezeigt werden. Sie können diesen Vorgang beschleunigen, indem Sie den Ermittlungszyklus manuell initiieren. 

Nach dem Einrichten eines Clientcomputers dauert es einige Minuten, bis dieser auf der Seite **Computer** in der WSUS-Konsole angezeigt wird. Bei Clientcomputern, die mithilfe eines Active Directory-basierten Gruppenrichtlinienobjekts konfiguriert wurden, dauert dies nach dem Aktualisieren der Gruppenrichtlinie ca. 20 Minuten (d. h., nach dem Anwenden neuer Einstellungen auf den Clientcomputer). Standardmäßig werden Gruppenrichtlinien alle 90 Minuten im Hintergrund (mit einer zufälligen Verzögerung zwischen 0 und 30 Minuten) aktualisiert. Wenn Sie Gruppenrichtlinien in kürzeren Abständen aktualisieren möchten, können Sie an einer Eingabeaufforderung auf dem Clientcomputer Folgendes eingeben: **gpupdate /force**.

Auf Clientcomputern, die mithilfe des Richtlinienobjekts der lokalen Gruppe konfiguriert wurden, wird die Gruppenrichtlinie sofort angewendet. Dieser Vorgang dauert ca. 20 Minuten.

Nach dem Anwenden der Gruppenrichtlinie können Sie die Ermittlung manuell initiieren. Wenn Sie diesen Schritt ausführen, müssen Sie nicht 20 Minuten warten, bis der Clientcomputer WSUS kontaktiert.

**So initiieren Sie die Ermittlung durch den WSUS-Server manuell**
1.  Klicken Sie auf dem Clientcomputer auf **Start** und anschließend auf **Ausführen**.

2.  Klicken Sie auf **cmd** und dann auf **OK**.

3.  Geben Sie an der Eingabeaufforderung **wuauclt.exe /detectnow** ein. Diese Befehlszeilenoption weist die automatischen Updates an, den WSUS-Server sofort zu kontaktieren.
