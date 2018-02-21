---
TOCTitle: So richten Sie eine Administratorengruppe ein
Title: So richten Sie eine Administratorengruppe ein
ms:assetid: 'f2ef847e-2824-471f-9079-5c343094aba8'
ms:contentKeyID: 18119094
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747798(v=WS.10)'
---

So richten Sie eine Administratorengruppe ein
=============================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Bevor die Gruppe als Administratorengruppe für RMS bestimmt werden kann, muss die Gruppe in Active Directory vorhanden sein. Die Eigenschaften der Gruppe müssen außerdem über eine E-Mail-Adresse (voll gekennzeichneter Domänenname) verfügen, die mit dem Kontonamen identisch ist.

Einrichten der Administratorengruppe
------------------------------------

#### So richten Sie eine Administratorengruppe ein

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie eine Administratorengruppe einrichten möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Sicherheitseinstellungen**.

3.  Klicken Sie im Bereich **Administratoren** auf **Aktivieren**, um eine Administratorengruppe hinzuzufügen.

4.  Geben Sie in das Feld **Name der RMS-Administratorgruppe** den voll gekennzeichneten Domänennamen im Format *Gruppenname*@*Domänenname*.com einer bestehenden Gruppe in dieser Active Directory-Gesamtstruktur ein, deren Mitgliedern Besitzerrechte für alle RMS-geschützten Dokumente erteilt werden sollen. Klicken Sie dann auf **Speichern**.

    Klicken Sie auf **Deaktivieren**, um Rechte für die Administratorgruppe zu deaktivieren.

Weitere Informationen zum Ausführen dieses Verfahrens finden Sie oben unter [Verwenden der Administratorengruppe](https://technet.microsoft.com/0febcb3e-7124-4e51-971a-1013b928d33b).