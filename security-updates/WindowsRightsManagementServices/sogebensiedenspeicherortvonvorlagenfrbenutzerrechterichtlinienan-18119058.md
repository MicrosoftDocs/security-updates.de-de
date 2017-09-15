---
TOCTitle: So geben Sie den Speicherort von Vorlagen für Benutzerrechterichtlinien an
Title: So geben Sie den Speicherort von Vorlagen für Benutzerrechterichtlinien an
ms:assetid: 'e1bee46d-33db-424f-ba45-1dcedcb883ab'
ms:contentKeyID: 18119058
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747781(v=WS.10)'
---

So geben Sie den Speicherort von Vorlagen für Benutzerrechterichtlinien an
==========================================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Wenn Sie Vorlagen für Benutzerrechterichtlinien in einem freigegebenen Ordner speichern und dann den Speicherort des freigegebenen Ordners ändern, müssen Sie die Vorlagen für die Benutzerrechterichtlinien manuell vom ursprünglichen Speicherort an den neuen Speicherort kopieren.

Vorlagen für Benutzerrechterichtlinien werden außerdem in der Konfigurationsdatenbank gespeichert. Weitere Informationen zum Verteilen von Vorlagen für Benutzerrechterichtlinien finden Sie oben unter [Verteilen von Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe).

Wenn Sie Microsoft Office 2003 als RMS-fähige Anwendung verwenden, wird der Speicherort von Vorlagen für Benutzerrechterichtlinien über den Registrierungsschlüssel `AdminTemplatePath` gesteuert, und der RMS-Client sucht die Vorlagen in der Folge an dem im Registrierungsschlüssel angegebenen Speicherort.

Angeben des Speicherorts von Vorlagen für Benutzerrechterichtlinien
-------------------------------------------------------------------

#### So geben Sie den Speicherort von Vorlagen für Benutzerrechterichtlinien an

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie den Speicherort von Vorlagen für Benutzerrechterichtlinien angeben möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Vorlagen für Benutzerrechterichtlinien**.

3.  Geben Sie im Bereich **Speicherort der Vorlage** den UNC-Pfad (Universal Naming Convention oder Universelle Benennungskonvention) eines freigegebenen Ordners an, in dem die Vorlagen für Benutzerrechterichtlinien für diesen Cluster gespeichert werden sollen. Verwenden Sie hierzu das folgende Format: \\\\*Servername*\\*Freigabename*. Das Konto, das den **Admin**-Anwendungspool ausführt, muss über Schreibrechte für den freigegebenen Ordner verfügen. Stellen Sie sicher, dass die Vorlagen an einem netzwerkzugänglichen Speicherort gespeichert werden, der den organisationsinternen Sicherheitsrichtlinien entspricht. Freigegebene Ordner für Vorlagen sollten nicht in den von RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwendeten Hauptordnern erstellt werden. Hierzu zählen z. B. die Ordner „Programme“ oder „IISRoot“.

4.  Klicken Sie auf **Speichern**.

5.  Nachdem Sie Vorlagen für Benutzerrechterichtlinien erstellt und an diesem Speicherort gespeichert haben, müssen die Vorlagen für Benutzer verfügbar gemacht werden. Standardmäßig sucht der RMS-Client nach Vorlagen für Benutzerrechterichtlinien am folgenden Speicherort auf dem lokalen Computer:

    %HOMEPATH%\\Lokale Einstellungen\\Anwendungsdaten\\Microsoft\\DRM\\Vorlagen

    Die Vorlagen für Benutzerrechterichtlinien sollten aus dem unter Schritt 3 angegebenen Speicherort an diesen Speicherort für alle Benutzer kopiert werden, die in Ihrer Organisation RMS verwenden.
