---
TOCTitle: So schließen Sie Anwendungen aus
Title: So schließen Sie Anwendungen aus
ms:assetid: '422f2ddd-bcf4-45f1-905a-b8bad30fd7dd'
ms:contentKeyID: 18118810
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720262(v=WS.10)'
---

So schließen Sie Anwendungen aus
================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Ausschlussrichtlinien werden vom Client erzwungen, sobald die Nutzungslizenz mit den geschützten Inhalten verbunden ist.

Ausschließen von Anwendungen oder Beenden des Ausschließens von Anwendungen
---------------------------------------------------------------------------

#### So schließen Sie Anwendungen aus

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie steuern möchten, welche Anwendungsversionen mit geschützten Inhalten verwendet werden können, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Ausschlussrichtlinien**.

3.  Klicken Sie im Bereich **Anwendungsausschluss** auf **Aktivieren**, um eine RMS-fähige Anwendung oder Komponente auszuschließen.

    Klicken Sie auf **Deaktivieren**, um den Ausschluss von Anwendungen zu deaktivieren.

4.  Geben Sie den Dateinamen der auszuschließenden Anwendung oder Komponente ein, geben Sie die auszuschließenden minimalen und maximalen Versionen (im Format *x*.*x*.*x*.*x*) ein, und klicken Sie dann auf **Diese Anwendung ausschließen**.

    Wählen Sie den Dateinamen aus, und klicken Sie dann auf **Ausgewählte Anwendungen aus der Ausschlussliste löschen**, um eine Anwendung (oder Komponente) aus der Ausschlussliste zu löschen.

    | ![](images/Cc720262.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                   |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | RMS erfordert, dass die Anwendungsversion durch vier jeweils durch Punkte getrennte Ziffern (\#.\#.\#.\# ) angegeben wird. Bei manchen Anwendungen ist die Anwendungsversion allerdings in zwei bzw. drei durch Punkte getrennten Ziffern angegeben. Ist dies der Fall, sollte „.0“ angefügt werden, um die Versionsnummer an das für RMS erforderliche Format anzupassen. |

#### So beenden Sie das Ausschließen von Anwendungen

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie steuern möchten, welche Anwendungsversionen mit geschützten Inhalten verwendet werden können, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Ausschlussrichtlinien**.

3.  Klicken Sie im Bereich **Anwendungsausschluss** auf **Deaktivieren**.

Weitere Informationen zum Ausführen dieses Verfahrens finden Sie oben unter „[Ausschließen von Anwendungen](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)“.