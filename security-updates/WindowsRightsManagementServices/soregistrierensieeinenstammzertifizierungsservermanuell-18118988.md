---
TOCTitle: So registrieren Sie einen Stammzertifizierungsserver manuell
Title: So registrieren Sie einen Stammzertifizierungsserver manuell
ms:assetid: 'aecdebb5-b28b-4b58-937a-392bb6ce9643'
ms:contentKeyID: 18118988
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747727(v=WS.10)'
---

So registrieren Sie einen Stammzertifizierungsserver manuell
============================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren Ausführen als verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Wenn Sie den Offlineregistrierungsvorgang verwenden, sollten Sie sicherstellen, dass die RMS-Clients nicht schon vor der Registrierung des RMS-Servers eine Verbindung zum Server herstellen und Lizenzen anfordern. Wenn Clients eine Verbindung zu einem nicht registrierten RMS-Server herstellen, gehen die Webdienste in einen Fehlerzustand über, der bewirkt, dass sie nicht mehr verwendet werden können. Wenn Sie nicht sicherstellen können, dass die Clients keine Verbindung zum RMS-Server herstellen, sollten Sie als bewährte Methode nach Abschluss der Registrierung IIS zurücksetzen, um eventuelle Fehlerzustände zu beseitigen.

Wenn Sie sich für die Offlineregistrierung entschieden haben und für die Verbindung zum Internet einen Computer mit verstärkter Browsersicherheit verwenden, beispielsweise einen Computer mit Windows Server 2003 oder Windows XP Service Pack 2, müssen Sie beim Anfordern eines Server-Lizenzgeberzertifikats den URL der Registrierungsdienst-Website zu den vertrauenswürdigen Sites hinzufügen, damit das Server-Lizenzgeberzertifikat heruntergeladen werden kann. Der URL lautet https://activation.drm.microsoft.com.

Stellen Sie bei Verwendung der Offlineregistrierung sicher, dass „GTE Cyber Trust Root CA“ im Zertifikatspeicher des Computers gespeichert ist, den Sie zum Übertragen der Registrierungsanforderung an den Microsoft-Registrierungsdienst verwenden. Auf Computern mit Windows Server 2003 gehört diese Zertifizierungsstelle standardmäßig zu den vertrauenswürdigen Entitäten. Wenn auf dem Computer eine andere Windows-Version ausgeführt wird, können Sie dieser Zertifizierungsstelle (Certification Authority oder CA) eine Vertrauensstellung zuweisen, indem Sie die neusten Zertifikatsaktualisierungen von Windows Update downloaden.

Manuelles Registrieren eines Stammzertifizierungsservers
--------------------------------------------------------

#### So registrieren Sie einen Stammzertifizierungsserver manuell

1.  Öffnen Sie nach der Installation von RMS auf einem Server, den Sie als Stammzertifizierungsserver verwenden möchten, die Seite **Globale Verwaltung**, und klicken Sie neben der Website, auf der Sie ein Stammserver-Lizenzgeberzertifikat importieren möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Clusterressourcen** auf **Registrieren**. Das Dialogfeld **Registrieren** wird geöffnet.

3.  Wählen Sie die Option **Offline**, und klicken Sie dann auf die Schaltfläche **Exportieren**. Das Dialogfeld **Dateidownload** wird angezeigt.

4.  Klicken Sie auf **Speichern**. Das Dialogfeld **Speichern unter** wird angezeigt.

    | ![](images/Cc747727.note(WS.10).gif)Hinweis                                                                                                                              |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Klicken Sie im Dialogfeld **Dateidownload** nicht auf **Öffnen**. Wenn Sie auf **Öffnen** klicken, wird eine Fehlermeldung angezeigt, und die Registrierungsanforderungsdatei wird nicht gespeichert. |

5.  Klicken Sie auf **Speichern**, um die Registrierungsanforderung in eine Datei zu exportieren. Die Datei wird standardmäßig auf Ihrem Desktop gespeichert und mit *Servername*EnrollRequest.xml benannt. Dabei wird *Servername* durch den Namen Ihres RMS-Servers ersetzt. Sie können die Datei an einem anderen Speicherort speichern, indem Sie im Dropdownmenü **Speichern unter** den gewünschten Speicherort auswählen. Sie können auch den standardmäßigen Dateinamen ändern, indem Sie im Feld **Dateiname** einen anderen Namen eingeben.

6.  Nachdem Sie die Registrierungsanforderungsdatei gespeichert haben, wird das Dialogfeld **Download beendet** angezeigt. Sie können auf **Öffnen** klicken, um den XML-Code in der Datei anzuzeigen. Sie dürfen jedoch keine Änderungen an der Datei vornehmen. Klicken Sie auf **Ordner öffnen**, um den Ordner zu öffnen, in dem die Datei gespeichert ist. Wenn Sie mit dem Überprüfen des Dateiinhalts und des Speicherorts fertig sind, klicken Sie auf **Schließen**.

7.  Übertragen Sie die Registrierungsanforderungsdatei von Ihrem Server auf einen Computer, der eine Verbindung zum Internet herstellen kann, und gehen Sie zur [Registrierungsdienst-Website]().

8.  Befolgen Sie die Anweisungen auf der Website, um ein Server-Lizenzgeberzertifikat zu erwerben.

9.  Übertragen Sie das Server-Lizenzgeberzertifikat zurück auf diesen Stammzertifizierungsserver.

10. Klicken Sie im Bereich **Clusterressourcen** auf **Registrieren**. Das Dialogfeld **Registrieren** wird geöffnet.

11. Klicken Sie im Dialogfeld **Registrieren** auf die Schaltfläche **Durchsuchen**, suchen Sie nach dem Server-Lizenzgeberzertifikat, das Sie gedownloadet haben, und klicken Sie dann auf die Schaltfläche **Importieren**.

12. Klicken Sie auf **Ja**, um zu bestätigen, dass Sie dieses Zertifikat importieren möchten.

13. Der Bereich **Clusterressourcen** wird aktualisiert, sodass er das Server-Lizenzgeberzertifikat anzeigt.