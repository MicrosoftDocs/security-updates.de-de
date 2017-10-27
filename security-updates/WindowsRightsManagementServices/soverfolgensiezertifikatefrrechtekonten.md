---
TOCTitle: So verfolgen Sie Zertifikate für Rechtekonten
Title: So verfolgen Sie Zertifikate für Rechtekonten
ms:assetid: 'f9efac9f-c725-4bce-a89f-7691b0d8ffc0'
ms:contentKeyID: 18119081
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747752(v=WS.10)'
---

So verfolgen Sie Zertifikate für Rechtekonten
=============================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Dieses Feature ist nur auf dem Stammzertifizierungscluster verfügbar; es ist nicht auf Lizenzierungsservern oder -clustern verfügbar.

Dieses Verfahren kann nur verwendet werden, um die Anzahl von Nutzungslizenzen zu schätzen. Das Verfahren ist nur sinnvoll, wenn es sich um zu berechnende Lizenzen handelt. Die Anzahl, die auf der Seite RM-Kontozertifizierungsbericht angezeigt wird, ist eine Schätzung. Wenn Sie die Konfigurationsdatenbank nicht aktualisiert haben, um nicht mehr aktuelle Benutzer zu löschen, ist diese Anzahl nicht korrekt. Bei Benutzern, für die mehrere Lizenzen in mehreren Gesamtstrukturen ausgestellt wurden, sind die zusätzlichen Lizenzen nicht in der angezeigten Anzahl enthalten.

Nachverfolgen von Rechtekontozertifikaten
-----------------------------------------

#### So verfolgen Sie Zertifikate für Rechtenkonten

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie Zertifikate nachverfolgen möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf „RM-Kontozertifizierungsbericht“.

3.  Rufen Sie unter **Gesamtanzahl der zertifizierten Benutzer** die Anzahl von Benutzern auf, die Zertifikate für Rechtenkonten von diesem Stammzertifizierungscluster empfangen haben.

Weitere Informationen hierzu finden Sie oben unter [Nachverfolgen von Rechtekontozertifikaten](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902).