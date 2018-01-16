---
TOCTitle: So geben Sie den Administratorkontakt an
Title: So geben Sie den Administratorkontakt an
ms:assetid: '31777458-5530-4ae0-ac1f-131b3d98dd35'
ms:contentKeyID: 18118799
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720237(v=WS.10)'
---

So geben Sie den Administratorkontakt an
========================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Bei diesem Verfahren sollte ein Administrator angegeben werden, der sich lokal auf dem Stammzertifizierungsserver befindet, da der angemeldete Benutzer zum Bereitstellen eines Lizenzierungsservers über Berechtigungen für die Datei „SubEnrollService.asmx“ verfügen muss, die sich auf dem Stammzertifizierungsserver befindet. Ein Benutzer, der versucht, einen Lizenzierungsserver bereitzustellen und nicht über Berechtigungen für diese Datei verfügt, kann eine Anforderung an den dedizierten Administrator senden. Dieser ist dann dafür verantwortlich, dem Benutzerkonto die erforderlichen Berechtigungen zu erteilen. Weitere Informationen hierzu finden Sie oben unter „[Festlegen von Berechtigungen für die Unterregistrierungsdienstdatei](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295)“.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Angeben des Administratorkontakts
---------------------------------

#### So geben Sie den Administratorkontakt an

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie den Administratorkontakt angeben möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Zertifizierungseinstellungen**.

3.  Geben Sie im Bereich **Administratorkontakt** die E-Mail-Adresse des Administrators ein, an den sich Benutzer bei auftretenden Unterregistrierungsproblemen während der Bereitstellung eines Lizenzierungsservers wenden können. Verwenden Sie hierzu das folgende Format: *Benutzername*@*Domänenname*.com.

4.  Klicken Sie unten auf der Seite auf **Absenden**.