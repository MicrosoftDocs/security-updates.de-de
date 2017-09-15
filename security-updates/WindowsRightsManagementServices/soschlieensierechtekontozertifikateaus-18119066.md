---
TOCTitle: So schließen Sie Rechtekontozertifikate aus
Title: So schließen Sie Rechtekontozertifikate aus
ms:assetid: 'e5cd9dec-ac29-437e-8515-dc697ec75edf'
ms:contentKeyID: 18119066
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747785(v=WS.10)'
---

So schließen Sie Rechtekontozertifikate aus
===========================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Diese Bedingungen werden vom Client erzwungen, sobald die Nutzungslizenz mit den geschützten Inhalten verbunden ist.

Ausschließen von Rechtekontozertifikaten
----------------------------------------

#### So schließen Sie Rechtekontozertifikate aus

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie Rechtekontozertifikate ausschließen möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Ausschlussrichtlinien**.

3.  Klicken Sie im Bereich „RM-Kontozertifikatausschluss“ auf **Aktivieren**, um das Rechtekontozertifikat eines Benutzers auszuschließen.

4.  Wählen Sie die Methode zum Angeben des auszuschließenden Zertifikats aus:

    -   Um das Kontozertifikat über den Benutzernamen auszuschließen, klicken Sie auf **Benutzername für das auszuschließende RM-Kontozertifikat**, geben Sie den Namen des auszuschließenden Benutzers (im Format *Benutzername*@*Domänenname*.com) ein, und klicken Sie dann auf **Hinzufügen**. Verwenden Sie diese Option zum Ausschließen von Kontozertifikaten interner Benutzer, die über Active Directory-Benutzerkonten verfügen.
    -   Um ein Kontozertifikat über den öffentlichen Schlüssel auszuschließen, klicken Sie auf **Zeichenfolge des öffentlichen Schlüssels für das auszuschließende RM-Kontozertifikat**, geben Sie die entsprechende Zeichenfolge des öffentlichen Schlüssels für das Rechtekontozertifikat ein, und klicken Sie dann auf **Hinzufügen**. Verwenden Sie diese Option zum Ausschließen von Kontozertifikaten externer Benutzer, die nicht über Active Directory-Benutzerkonten verfügen.

    | ![](images/Cc747785.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                         |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Um ein Kontozertifikat aus der Ausschlussliste zu löschen, klicken Sie auf das ausgeschlossene Rechtekontozertifikat in der Liste, und klicken Sie dann auf **Ausgewählte öffentliche Schlüssel aus der Ausschlussliste löschen**. Der Benutzer mit dem jeweiligen Kontozertifikat kann jetzt eine Lizenz für RMS-geschützte Inhalte von diesem Server erhalten. |

    | ![](images/Cc747785.note(WS.10).gif)Hinweis                          |
    |---------------------------------------------------------------------------------------------------|
    | Klicken Sie auf **Deaktivieren**, um den Ausschluss eines Rechtekontozertifikats zu deaktivieren. |

Weitere Informationen zum Ausführen dieses Verfahrens finden Sie oben unter [Ausschließen von Rechtekontozertifikaten](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6).
