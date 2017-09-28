---
TOCTitle: 'Schritt 5: Konfigurieren von Client-Updates'
Title: 'Schritt 5: Konfigurieren von Client-Updates'
ms:assetid: '5ae60ead-3e94-456c-a692-c0f193ea5d5a'
ms:contentKeyID: 21669469
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd939830(v=WS.10)'
---

Schritt 5: Konfigurieren von Client-Updates
===========================================

In Windows Server Update Services 3.0 (WSUS 3.0 SP2) konfiguriert WSUS Setup IIS automatisch so, dass die neueste Version der automatischen Updates an alle Clientcomputer verteilt wird, die eine Verbindung mit dem WSUS-Server herstellen.

Welche Methode zum Konfigurieren von automatischen Updates am besten ist, hängt von der Netzwerkumgebung ab. In einer Umgebung mit Active Directory®-Verzeichnisservice können Sie ein bestehendes Gruppenrichtlinienobjekt (Group Policy Object, GPO) der Domäne verwenden oder ein neues GPO erstellen. In einer Umgebung ohne Active Directory können Sie das lokale Gruppenrichtlinienobjekt verwenden. In diesem Schritt konfigurieren Sie automatische Updates und ordnen anschließend die Clientcomputer dem WSUS-Server zu.

Bei den folgenden Verfahren wird davon ausgegangen, dass auf Ihrem Netzwerk Active Directory ausgeführt wird. Außerdem wird davon ausgegangen, dass Sie mit Gruppenrichtlinien vertraut sind und diese für die Verwaltung des Netzwerks verwenden.

Weitere Informationen zu Gruppenrichtlinien finden Sie auf der Tech Center-Website über Gruppenrichtlinien unter [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375) (in englischer Sprache).

 
-

Verfahren in Schritt 5
----------------------

In Schritt 4 haben Sie die Konfiguration der herunterzuladenden Updates abgeschlossen. Mit diesen Verfahren können Sie automatische Updates für Clientcomputer konfigurieren.

1.  Konfigurieren von automatischen Updates in der Gruppenrichtlinie
2.  Zuordnen der Clientcomputer zum WSUS-Server
3.  Manuelles Starten der Erkennung durch den WSUS-Server

Die ersten beiden Verfahren führen Sie mithilfe einer beliebigen GPO der Domäne aus, das dritte Verfahren in einer Eingabeaufforderung auf dem Clientcomputer.

**So konfigurieren Sie automatische Updates**
1.  Suchen Sie in der Group Policy Management Console (GPMC) nach der GPO, in der Sie WSUS konfigurieren möchten, und klicken Sie auf **Bearbeiten**.

2.  Erweitern Sie in der GPMC zuerst **Computerkonfiguration**, dann **Administrative Vorlagen**, dann **Windows-Komponenten**, und klicken Sie anschließend auf **Windows Update**.

3.  Doppelklicken Sie im Detailfenster auf **Automatische Updates konfigurieren**.

4.  Klicken Sie auf **Aktiviert**, und klicken Sie dann auf eine der folgenden Optionen:

    -   **Vor Download und Installation benachrichtigen**. Bei dieser Option wird ein angemeldeter Administrator vor dem Herunterladen und vor der Installation der Updates benachrichtigt.
    -   **Autom. Downloaden, aber vor Installation benachrichtigen**. Bei dieser Option wird automatisch mit dem Herunterladen von Updates begonnen und anschließend ein angemeldeter Administrator benachrichtigt, bevor die Updates installiert werden.
    -   **Autom. Downloaden und laut Zeitplan installieren**. Bei dieser Option wird automatisch mit dem Herunterladen von Updates begonnen, anschließend werden die Updates zum von Ihnen festgelegten Zeitpunkt installiert.
    -   **Lokalem Administrator ermöglichen, Einstellung auszuwählen**. Bei dieser Option können lokale Administratoren mithilfe der Systemsteuerungsoption "Automatische Updates" eine Konfigurationsoption auswählen. Sie können beispielsweise den Zeitpunkt für eine Installation planen. Lokale Administratoren können automatische Updates nicht deaktivieren.

5.  Klicken Sie auf **OK**.

**So verweisen Sie den Clientcomputer auf den WSUS-Server**
1.  Doppelklicken Sie im Detailfenster **Windows Update** auf **Internen Pfad für den Microsoft Updatedienst angeben**.

2.  Klicken Sie auf **Aktiviert**, und geben Sie die HTTP-URL des WSUS-Servers sowohl im Feld **Interner Updatedienst zum Ermitteln von Updates** als auch im Feld **Intranetserver für die Statistiken** ein. Geben Sie z. B. *http://Servername* in beiden Feldern ein, und klicken Sie anschließend auf **OK**.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939830.note(WS.10).gif" />Hinweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Wenn Sie diesen Computer dem WSUS-Server mithilfe des lokalen Gruppenrichtlinienobjekts zuordnen, wird diese Einstellung sofort wirksam, und der Computer wird nach kurzer Zeit in der WSUS-Verwaltungskonsole angezeigt. Sie können diesen Vorgang beschleunigen, indem Sie den Erkennungszyklus manuell starten.
</td>
</tr>
</tbody>
</table>
 

Nach dem Einrichten eines Clientcomputers dauert es einige Minuten, bis dieser auf der Seite **Computer** in der WSUS-Verwaltungskonsole angezeigt wird. Bei Clientcomputern, die mithilfe einer domänenbasierten Gruppenrichtlinie konfiguriert wurden, kann dies nach dem Aktualisieren der Gruppenrichtlinie (d. h. nach Anwenden neuer Einstellungen auf den Clientcomputer) ca. 20 Minuten dauern. In der Standardeinstellung werden Gruppenrichtlinien alle 90 Minuten, mit einer zufälligen Verzögerung von bis zu 30 Minuten, im Hintergrund aktualisiert. Wenn Sie Gruppenrichtlinien in kürzeren Abständen aktualisieren möchten, können Sie an einer Eingabeaufforderung auf dem Clientcomputer Folgendes eingeben: **gpupdate /force**.

Bei Clientcomputern, die mithilfe einer lokalen GPO konfiguriert wurden, wird die Gruppenrichtlinie sofort angewendet, und die Aktualisierung dauert ca. 20 Minuten.

Wenn Sie die Erkennung manuell starten, müssen Sie nicht 20 Minuten warten, bis der Clientcomputer eine Verbindung zu WSUS herstellt.

**So starten Sie die Erkennung durch den WSUS-Server manuell**
1.  Klicken Sie auf dem Clientcomputer auf **Start** und anschließend auf **Ausführen**.

2.  Geben Sie **cmd** im Feld **Öffnen** ein, und klicken Sie anschließend auf **OK**.

3.  In die Eingabeaufforderung geben Sie **wuauclt.exe /detectnow** ein. Diese Befehlszeilenoption weist die Funktion "Automatische Updates" an, sofort eine Verbindung zum WSUS-Server herzustellen.

Nächster Schritt
----------------

[Schritt 6: Konfigurieren von Computergruppen](https://technet.microsoft.com/70518732-2179-4e41-9609-7f9999867f41)

Weitere Ressourcen
------------------

[Schrittweise Anleitung für Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
