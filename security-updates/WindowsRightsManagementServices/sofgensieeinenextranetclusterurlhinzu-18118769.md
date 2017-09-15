---
TOCTitle: 'So fügen Sie einen Extranet-Cluster-URL hinzu'
Title: 'So fügen Sie einen Extranet-Cluster-URL hinzu'
ms:assetid: '12c83186-ce9e-4100-bbd1-d87a885331c7'
ms:contentKeyID: 18118769
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720193(v=WS.10)'
---

So fügen Sie einen Extranet-Cluster-URL hinzu
=============================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Registrieren Sie den URL in DNS (Domain Name System), und überprüfen Sie, ob er einwandfrei ausgeführt und über das Internet-Extranet verfügbar ist. Wenn SSL (Secure Sockets Layer) für die Webdienstedateien aktiviert ist, müssen Sie HTTPS für den Cluster-URL angeben.

Wenn Sie einen Extranet-Cluster-URL einem RMS-Server hinzufügen, der bereits im Einsatz ist, müssen die aktuellen RMS-Clients neue Client-Lizenzgeberzertifikate erwerben, damit sie zur Lizenzierung auf den Extranet-Cluster zugreifen können.

Hinzufügen von Extranet-Cluster-URLs
------------------------------------

#### So fügen Sie einen Extranet-Cluster-URL hinzu

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie einen Extranet-Cluster-URL (Uniform Resource Locator) hinzufügen möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Einstellungen für Extranet-Cluster-URL**.

3.  Geben Sie im Bereich **Extranet-Cluster-URL** den URL an, über den externe Benutzer Lizenzen erwerben sollen. Sie können außerdem entweder HTTP (Hypertext Transfer Protocol) oder HTTPS (Hypertext Transfer Protocol Secure) auswählen.

4.  Klicken Sie auf **Absenden**.
