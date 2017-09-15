---
TOCTitle: So aktivieren Sie die Zertifizierung von mobilen Geräten
Title: So aktivieren Sie die Zertifizierung von mobilen Geräten
ms:assetid: '93ec088e-9056-4c3c-bd97-1173fb194578'
ms:contentKeyID: 18118938
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747603(v=WS.10)'
---

So aktivieren Sie die Zertifizierung von mobilen Geräten
========================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Dieses Verfahren wird nur auf den Stammzertifizierungscluster angewendet.

Bei diesem Verfahren wird vorausgesetzt, dass Sie eine Benutzergruppe erstellt haben, die Benutzerkonten von Benutzern mobiler Geräte enthält, die RMS-geschützten Inhalt abrufen.

Aktivieren der Zertifizierung mobiler Geräte
--------------------------------------------

#### So aktivieren Sie die Zertifizierung von mobilen Geräten

1.  Öffnen Sie auf dem Stammzertifizierungsserver einen Dateisystembrowser, und navigieren Sie zum Ordner des &lt;Systemlaufwerks&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification.

2.  Damit mobile Geräte Rechtekontozertifikate (Rights Account Certificates oder RACs) erhalten können, klicken Sie mit der rechten Maustaste auf die Datei MobileDeviceCertification.asmx, und klicken Sie dann auf **Eigenschaften**.

3.  Klicken Sie auf der Registerkarte **Sicherheit** auf **Hinzufügen**, und fügen Sie die für diese Benutzerkategorie erstellte Gruppe und die **RMS Service Group** (RMS-Dienstgruppe) hinzu.

4.  Aktivieren Sie in der Liste **Berechtigungen** für die Gruppen das Kontrollkästchen **Zulassen** für die Berechtigungen zum **Lesen** und zum **Lesen und Ausführen**, und klicken Sie dann auf **OK**.
