---
TOCTitle: 'So ändern Sie das RMS-Dienstkonto'
Title: 'So ändern Sie das RMS-Dienstkonto'
ms:assetid: 'a3e522b0-e23d-49f2-b00a-cff90ac2c36a'
ms:contentKeyID: 18118974
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747713(v=WS.10)'
---

So ändern Sie das RMS-Dienstkonto
=================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Das RMS-Dienstkonto darf nicht mit dem Domänenkonto identisch sein, das zum Installieren von RMS mit Service Pack 1 verwendet wurde.

Ändern des RMS-Dienstkontos
---------------------------

#### So ändern Sie das RMS-Dienstkonto

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der RMS (Rights Management Services oder Dienste für die Rechteverwaltung) bereitgestellt ist, auf **RMS-Dienstkonto ändern**.

2.  Geben Sie den Namen des Kontos an, unter dem RMS für die meisten Operationen ausgeführt werden soll. Verwenden Sie für Konten auf Domänenebene das Format *Domänenname*\\*Benutzername*.

3.  Geben Sie das Kennwort ein, und klicken Sie dann auf **Absenden**.
