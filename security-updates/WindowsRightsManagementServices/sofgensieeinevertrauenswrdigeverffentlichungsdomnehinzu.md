---
TOCTitle: So fügen Sie eine vertrauenswürdige Veröffentlichungsdomäne hinzu
Title: So fügen Sie eine vertrauenswürdige Veröffentlichungsdomäne hinzu
ms:assetid: '731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c'
ms:contentKeyID: 18118881
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747624(v=WS.10)'
---

So fügen Sie eine vertrauenswürdige Veröffentlichungsdomäne hinzu
=================================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Wenn Sie den privaten RMS-Schlüssel mithilfe eines Hardwaresicherheitsmoduls schützen und ein Server-Lizenzgeberzertifikat aus einer RMS-Installation installieren, die Software zum Schützen des privaten Schlüssels verwendet, müssen Sie für jeden RMS-Server im Cluster auf der Seite **Sicherheitseinstellungen** jeweils ein Kennwort für den privaten Schlüssel angeben, bevor Sie das Zertifikat importieren.

Hinzufügen von vertrauenswürdigen Veröffentlichungsdomänen
----------------------------------------------------------

#### So fügen Sie eine vertrauenswürdige Veröffentlichungsdomäne hinzu

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie eine vertrauenswürdige Veröffentlichungsdomäne hinzufügen möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Vertrauensrichtlinien**.

3.  Klicken Sie im Bereich **Vertrauenswürdige veröffentlichende Domänen** auf **Durchsuchen**. Suchen Sie die Domäne, und doppelklicken Sie dann auf das Zertifikat der hinzuzufügenden Veröffentlichungsdomäne. Geben Sie in das Feld **Kennwort zum Entschlüsseln der importierten Datei** das erforderliche Kennwort zum Entschlüsseln dieser Datei ein, und klicken Sie dann auf **Importieren**.

    Diese kennwortverschlüsselte Datei enthält das Lizenzgeberzertifikat, den privaten Schlüssel (wenn der Schlüssel in der Software gespeichert ist) und Vorlagen für Benutzerrechterichtlinien.

4.  Der Name der Domäne wird in der Liste **Vertrauenswürdige veröffentlichende Domänen** angezeigt.

Weitere Informationen zum Ausführen dieses Verfahrens Sie oben unter „[Hinzufügen und Entfernen von vertrauenswürdigen Veröffentlichungsdomänen](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee)“.