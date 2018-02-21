---
TOCTitle: 'So aktualisieren Sie ein Server-Lizenzgeberzertifikat'
Title: 'So aktualisieren Sie ein Server-Lizenzgeberzertifikat'
ms:assetid: 'affce9cf-8b46-4293-8e1c-ee06f2ca6537'
ms:contentKeyID: 18118973
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747636(v=WS.10)'
---

So aktualisieren Sie ein Server-Lizenzgeberzertifikat
=====================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Wenn Sie sich für die Offline-Erneuerung entschieden haben und für die Verbindung zum Internet einen Computer mit verstärkter Browsersicherheit verwenden, beispielsweise einen Computer mit Windows Server 2003 oder Windows XP Service Pack 2, müssen Sie beim Anfordern eines Server-Lizenzgeberzertifikats den URL der Registrierungsdienst-Website zu den vertrauenswürdigen Sites hinzufügen, damit das Server-Lizenzgeberzertifikat gedownloadet werden kann. Der URL lautet https://activation.drm.microsoft.com.

Stellen Sie bei Verwendung der Offlineregistrierung sicher, dass „GTE Cyber Trust Root CA“ im Zertifikatspeicher des Computers gespeichert ist, den Sie zum Übertragen der Registrierungsanforderung an den Microsoft-Registrierungsdienst verwenden. Auf Computern mit Windows Server 2003 gehört diese Zertifizierungsstelle standardmäßig zu den vertrauenswürdigen Entitäten. Wenn auf dem Computer eine andere Windows-Version ausgeführt wird, können Sie dieser Zertifizierungsstelle (Certification Authority oder CA) eine Vertrauensstellung zuweisen, indem Sie die neusten Zertifikatsaktualisierungen von Windows Update downloaden.

Erneuern eines Server-Lizenzgeberzertifikats
--------------------------------------------

#### So aktualisieren Sie ein Server-Lizenzgeberzertifikat

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie ein Zertifikat aktualisieren möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie auf der Seite **Verwaltung** im Bereich **Clusterressourcen** auf die Schaltfläche **Erneuern**. Das Dialogfeld Erneuern wird angezeigt.

3.  Wenn Ihr Computer mit dem Verbindung verbunden ist, wählen Sie die Option **Online** aus, und klicken Sie dann auf **Erneuern**, um das Server-Lizenzgeberzertifikat automatisch zu erneuern.

4.  Wenn Ihr Computer nicht mit dem Internet verbunden ist, wählen Sie die Option **Offline** aus, und klicken Sie dann auf die Schaltfläche **Exportieren**. Das Dialogfeld **Dateidownload** wird angezeigt.

5.  Klicken Sie auf **Speichern**. Das Dialogfeld **Speichern unter** wird angezeigt.

    | ![](images/Cc747636.note(WS.10).gif)Hinweis                                                                                                                              |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Klicken Sie im Dialogfeld **Dateidownload** nicht auf **Öffnen**. Wenn Sie auf **Öffnen** klicken, wird eine Fehlermeldung angezeigt, und die Registrierungsanforderungsdatei wird nicht gespeichert. |

6.  Klicken Sie auf **Speichern**, um die Erneuerungsanforderung in eine Datei zu exportieren. Standardmäßig wird die Datei auf Ihrem Desktop mit dem Namen *Servername*RenewRequest.xml gespeichert. Dabei wird *Servername* durch den Namen Ihres RMS-Servers ersetzt. Sie können die Datei an einem anderen Speicherort speichern, indem Sie im Dropdownmenü Speichern unter den gewünschten Speicherort auswählen. Sie können auch den standardmäßigen Dateinamen ändern, indem Sie im Feld **Dateiname** einen anderen Namen eingeben.

7.  Wenn Sie die Erneuerungsanforderungsdatei gespeichert haben, wird das Dialogfeld **Download abgeschlossen** angezeigt. Sie können auf **Öffnen** klicken, um den XML-Code in der Datei anzuzeigen. Sie dürfen jedoch keine Änderungen an der Datei vornehmen. Klicken Sie auf **Ordner öffnen**, um den Ordner zu öffnen, in dem die Datei gespeichert ist. Wenn Sie mit dem Überprüfen des Dateiinhalts und des Speicherorts fertig sind, klicken Sie auf **Schließen**.

8.  Übertragen Sie die Erneuerungsanforderungsdatei von Ihrem Server auf einen Computer, der eine Verbindung zum Internet herstellen kann, und rufen Sie die [Website des Registrierungsdienstes]() (https://go.microsoft.com/fwlink/?LinkId=25828) auf.

9.  Befolgen Sie die Anweisungen auf der Website, um ein Server-Lizenzgeberzertifikat zu erwerben.

10. Übertragen Sie das Server-Lizenzgeberzertifikat zurück auf diesen Stammzertifizierungsserver.

11. Klicken Sie im Bereich **Clusterressourcen** auf **Erneuern**. Das Dialogfeld **Erneuern** wird angezeigt.

12. Klicken Sie im Dialogfeld **Erneuern** auf die Schaltfläche **Durchsuchen**, wählen Sie das gedownloadete Server-Lizenzgeberzertifikat aus, und klicken Sie dann auf die Schaltfläche **Importieren**.

13. Klicken Sie auf **Ja**, um zu bestätigen, dass Sie dieses Zertifikat importieren möchten.

14. Nachdem das Server-Lizenzgeberzertifikat erfolgreich erneuert wurde, wird der Bereich **Clusterressourcen** aktualisiert und das neue Ablaufdatum des Server-Lizenzgeberzertifikats angezeigt.

Weitere Informationen zum Erneuern von Server-Lizenzgeberzertifikaten finden Sie oben unter [Verwalten von Server-Lizenzgeberzertifikaten](https://technet.microsoft.com/549979ad-13ee-4abc-8281-3e002a5a9561).