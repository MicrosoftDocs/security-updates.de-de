---
TOCTitle: So aktivieren Sie die Zertifizierung von Serverdiensten
Title: So aktivieren Sie die Zertifizierung von Serverdiensten
ms:assetid: '0ed78c85-7acb-4e3b-a594-613f8ccb5b14'
ms:contentKeyID: 18118750
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720196(v=WS.10)'
---

So aktivieren Sie die Zertifizierung von Serverdiensten
=======================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren ist. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Dieses Verfahren wird nur auf den Stammcluster angewendet.

Bei diesem Verfahren wird vorausgesetzt, dass Sie eine Benutzergruppe erstellt haben, die jene Benutzerkonten enthält, die die Serverdienste beim Abrufen von durch Rechte geschütztem Inhalt verkörpern.

Aktivieren der Zertifizierung von Serverdiensten
------------------------------------------------

#### So aktivieren Sie die Zertifizierung von Serverdiensten

1.  Melden Sie den Computer als Mitglied einer lokalen Gruppe Administratoren an.

2.  Öffnen Sie einen Dateisystembrowser, und navigieren Sie zum Ordner des &lt;Systemlaufwerks&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification.

3.  Damit Serverdienste Rechtekontozertifikate (Rights Account Certificates; RACs) erhalten können, klicken Sie mit der rechten Maustaste auf die Datei **ServerCertification.asmx**, und klicken Sie dann auf Eigenschaften.

4.  Klicken Sie auf der Registerkarte **Sicherheit** auf **Hinzufügen**, und fügen Sie die für diese Benutzerkategorie erstellte Gruppe und die **RMS Service Group** (RMS-Dienstgruppe) hinzu.

5.  Aktivieren Sie in der Liste **Berechtigungen** für die Gruppen das Kontrollkästchen **Zulassen** für die Berechtigungen **Lesen & Ausführen**, und klicken Sie danach auf **OK**.

6.  Wiederholen Sie die Schritte 1 bis 4 für jeden Server im Cluster.

| ![](images/Cc720196.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Für Microsoft Exchange Server 2007 müssen Sie die Active Directory-Computerobjekte aller Bridgeheadserver der freigegebenen Zugriffssteuerungsliste (Discretionary Access Control List oder DACL) der Datei ServerCertification.asmx hinzufügen. Gleichermaßen müssen Sie für Microsoft Office SharePoint Server 2007 das Active Directory-Computerobjekt des Office SharePoint Server 2007-Servers dieser DACL hinzufügen. Sie sollten dieser DACL eine Sicherheitsgruppe hinzufügen, der Sie die entsprechenden Computerobjekte hinzufügen. |
