---
TOCTitle: 'Probleme bei der RMS-Bereitstellung'
Title: 'Probleme bei der RMS-Bereitstellung'
ms:assetid: 'b0e6ef48-ab38-4426-be5b-811cf64c45c0'
ms:contentKeyID: 18118975
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747638(v=WS.10)'
---

Probleme bei der RMS-Bereitstellung
===================================

Bei der Bereitstellung von RMS werden die Ressourcendateien und die Verbindungen zwischen den verschiedenen Komponenten, von denen RMS abhängt, konfiguriert und eingerichtet. Wenn ein Fehler festgestellt wird, während RMS versucht, eine Ressource einzurichten, schlägt die Bereitstellung fehl, und es wird eine Fehlermeldung angezeigt. In diesem Abschnitt werden die häufigsten Ursachen für diese Fehler erläutert, um Sie in unerwarteten Situationen, die verhindern, dass Sie die Bereitstellung von RMS abschließen können, bei der Problembehandlung zu unterstützen.

Der Stammzertifizierungsserver kann nicht bereitgestellt werden
---------------------------------------------------------------

Es könnte sein, dass Sie den Stammzertifizierungsserver nicht bereitstellen können, da die entsprechenden Bereitstellungsseiten nicht angezeigt werden. Dieses Verhalten tritt auf, wenn Sie auf der Seite „Globale Verwaltung“ auf „RMS auf dieser Website bereitstellen“ klicken, um den ersten Stammzertifizierungsserver bereitzustellen. Anstelle der Bereitstellungsseiten für einen Stammzertifizierungsserver werden die Bereitstellungsseiten für einen Lizenzierungsserver angezeigt.

Dieses Problem tritt auf, wenn Sie die Bereitstellung des letzten Stammzertifizierungsservers in dieser Active Directory-Gesamtstruktur nicht aufheben, bevor Sie versuchen, einen neuen Stammzertifizierungsserver bereitzustellen. Wenn Sie die Bereitstellung des letzten Stammzertifizierungsservers in einer Active Directory-Gesamtstruktur aufheben, wird der Dienstverbindungspunkt aus Active Directory entfernt. Falls Sie die Bereitstellung des letzten Stammzertifizierungsservers in der Gesamtstruktur nicht aufheben, bevor Sie RMS deinstallieren, können Sie in dieser Gesamtstruktur erst dann einen Stammzertifizierungsserver erneut bereitstellen, wenn Sie den Dienstverbindungspunkt manuell aus Active Directory entfernt haben.

Wenn bei dem Versuch, den ersten Stammzertifizierungsserver in einer Active Directory-Gesamtstruktur bereitzustellen, die Bereitstellungsseiten für einen Lizenzierungsserver angezeigt werden, entfernen Sie den Dienstverbindungspunkt aus Active Directory wie folgt:

**So entfernen Sie den Dienstverbindungspunkt für RMS**
1.  Falls erforderlich, installieren Sie die Windows Server Support Tools:

    Führen Sie für Windows Server 2003 die Datei Suptools.msi aus, die Sie auf der Installations-CD im Ordner \\Support\\Tools finden.

    Führen Sie für Windows 2000 Server die Datei Setup.exe aus, die Sie auf der Installations-CD im Ordner \\Support\\Tools finden.

2.  Melden Sie sich beim Domänencontroller der Domäne, in der der Stammzertifizierungsserver Mitglied ist, mit einem Konto der Gruppe Domänen-Admins an.

3.  Geben Sie an der Eingabeaufforderung den folgenden Befehl ein, und drücken Sie die Eingabetaste.

    **ldp**

4.  Klicken Sie auf **Verbindung** und dann auf **Verbinden**.

5.  Drücken Sie die Eingabetaste. Geben Sie keine Informationen ein.

6.  Klicken Sie auf **Verbindung** und dann auf **Gebunden**.

7.  Drücken Sie die Eingabetaste. Geben Sie keine Informationen ein.

8.  Klicken Sie auf **Ansicht** und dann auf **Struktur**.

9.  Drücken Sie die Eingabetaste. Geben Sie keine Informationen ein.

    Im linken Fensterbereich wird **dc=YourDomain,dc=com** angezeigt.

10. Erweitern Sie **dc=YourDomain,dc=com**.

11. Erweitern Sie **Konfiguration**.

12. Erweitern Sie **Dienste**.

13. Löschen Sie **RightsManagementServices**.

– Oder –

1.  Downloaden Sie das RMS Administration Toolkit, und installieren Sie es. Das Toolkit kann auf der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=33841)gedownloaded werden.
2.  Öffnen Sie die Eingabeaufforderung, indem Sie auf **Start**, **Ausführen** klicken. Geben Sie im Dialogfeld **Ausführen** den Befehl **cmd** ein, und klicken Sie dann auf **OK**.
3.  Geben Sie auf der Befehlszeile folgenden Befehl ein:
    **ADSCPRegister.exeunregisterscp** &lt;*URLtoUnRegister*&gt;
4.  Geben Sie für &lt;*URLtoUnRegister*&gt; den URL des RMS-Dienstverbindungspunktes ein, z. B. https://my\_domain/\_wmcs/Certification.

Sie können den Stammzertifizierungsserver im Anschluss an diese Schritte bereitstellen.

SSPI-Kontext kann nicht erstellt werden
---------------------------------------

Eventuell wird während der Bereitstellung die Fehlermeldung angezeigt, dass kein SSPI-Kontext erstellt werden kann („Cannot generate SSPI context“), wenn das RMS-Dienstkonto beim Registrieren des Stammzertifizierungsservers beim Microsoft-Registrierungsdienst nicht authentifiziert wird.

Wenn Sie diese Fehlermeldung erhalten, überprüfen Sie, ob es sich bei dem RMS-Dienstkonto um ein gültiges Domänenkonto handelt. Wenn es sich bei dem Konto um ein Gruppenkonto handelt, stellen Sie sicher, dass die Gruppenmitgliedschaft noch aktuell ist, dass Sie alle Benutzerkonten in der Gruppe in der Domäne auflösen können und dass die Konten Berechtigungen für die SQL-Datenbanken haben.
