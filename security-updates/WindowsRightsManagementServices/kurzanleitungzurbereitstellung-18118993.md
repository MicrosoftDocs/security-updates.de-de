---
TOCTitle: Kurzanleitung zur Bereitstellung
Title: Kurzanleitung zur Bereitstellung
ms:assetid: 'b8fb69b6-3e0b-4836-8c05-8bd93f522a7c'
ms:contentKeyID: 18118993
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747735(v=WS.10)'
---

Kurzanleitung zur Bereitstellung
================================

Diese Kurzanleitung soll Sie darin unterstützen, einen Server mit Windows RMS (Windows Rights Management Services oder Dienste für die Windows-Rechteverwaltung) und Service Pack 1 auf einfache und schnelle Weise für Testzwecke einzurichten und auszuführen, sodass Sie entscheiden können, ob eine größere Bereitstellung in der Organisation erfolgen soll.

**Schritt 1 – Vorbereitungen für RMS**

RMS ist von anderen Komponenten abhängig, die vor der Verwendung dieses Dienstes installiert und konfiguriert werden. Die Infrastruktur erfüllt die grundlegenden Anforderungen für RMS, nachdem Sie die folgenden Schritte erfolgreich ausgeführt haben:

1.  Konfigurieren Sie einen Computer unter Windows Server 2003, und fügen Sie den Computer dann zu einer Active Directory-Domäne hinzu. (Bei kleinen Organisationen mit nur einem Server kann es sich bei diesem Computer auch um den Domänencontroller für Active Directory handeln. In diesem Fall muss auf dem Computer jedoch Windows Server 2003 Standard Edition, Windows Server 2003 Enterprise Edition oder Windows Server 2003 Datacenter Edition ausgeführt werden. Ein Computer mit Windows Server 2003 Web Edition kann nicht als Domänencontroller verwendet werden.)
2.  Konfigurieren Sie den Server für die Rolle als **Anwendungsserver**. Klicken Sie hierzu auf **Start**, doppelklicken Sie auf **Systemsteuerung**, und doppelklicken Sie dann auf **Software**. Klicken Sie unter **Software** auf **Windows-Komponenten hinzufügen/entfernen**, und stellen Sie dann sicher, dass die folgenden Dienste unter **Anwendungsserver** aktiviert sind:
    -   **ASP.NET**
    -   **Internetinformationsdienste (Internet Information Services oder IIS)**
    -   **Message Queuing**

    Übernehmen Sie die Standardoptionen für jeden Dienst. Es ist keine weitere Konfiguration erforderlich.
3.  Konfigurieren Sie einen Datenbankserver mithilfe einer der folgenden Datenbankanwendungen:
    -   Microsoft® SQL Server 2000 mit SP3. Hierbei kann es sich um eine lokale Installation von SQL Server 2000 handeln oder um eine Remoteinstallation in derselben Domäne.
    -   Microsoft SQL Server 2000 Desktop Engine (MSDE 2000), Release A. Hierbei muss es sich um eine lokale Installation handeln. Sie können MSDE 2000 von der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=17799)(http://go.microsoft.com/fwlink/?LinkID=17799) herunterladen.

    Sie sollten Microsoft SQL Server Desktop Engine (MSDE) nur in Testumgebungen zur Unterstützung von RMS-Datenbanken verwenden, da Microsoft SQL Server Desktop Engine nicht über die zur vollen Ausführung und Unterstützung einer unternehmensweiten Datenbank erforderlichen Tools verfügt. Darüber hinaus unterstützt MSDE die Vernetzung auf Distanz nicht. Deshalb müssen Sie es auf demselben Server installieren, auf dem RMS installiert ist, und können keine zusätzlichen RMS-Server zum RMS-Cluster hinzufügen. In den Nutzungsbedingungen für Microsoft SQL Server Desktop Engine wird angegeben, dass SQL Server-Clienttools nicht zur Bearbeitung einer Microsoft SQL Server Desktop Engine-Datenbank verwendet werden können. Aufgrund dieser Einschränkung können Sie weder die RMS-Konfigurationsdatenbank sichern oder wiederherstellen, noch Protokollierungsinformationen anzeigen lassen, noch in der Konfigurationsdatenbank gespeicherte Daten direkt ändern.
4.  Entscheiden Sie, welcher Name für diesen Dienst verwendet werden soll, wenn Benutzer über das Intranet eine Verbindung mit dem Dienst herstellen möchten (beispielsweise http://certification.contoso.com). Konfigurieren Sie das DNS (Domain Name System oder Domänennamensystem) so, dass der URL in die IP-Adresse des RMS-Computers aufgelöst wird. Verwenden Sie einen voll gekennzeichneten Domänennamen für den Cluster-URL, um sicherzustellen, dass Clients in anderen DNS-Zonen die IP-Adresse des bzw. der RMS-Server(s) auflösen können.
5.  Erstellen Sie ein Administratorkonto für die Verwendung mit RMS.
6.  Nun können Sie RMS SP1 installieren. Weitere Anleitungen dazu finden Sie unter „So installieren Sie RMS mit Service Pack 1“ im Abschnitt „Betreiben eines RMS-Server“ in dieser Dokumentationssammlung.

**Häufig verwendete optionale Funktionen**

Die folgenden Funktionen sind optional. Wenn Sie sie verwenden möchten, sollten Sie die notwendigen Vorbereitungen treffen, bevor Sie mit dem Installations- und Bereitstellungsvorgang für RMS beginnen.

-   Sie können RMS für die Verwendung eines Hardwaresicherheitsmoduls (HSM) konfigurieren, um private Schlüssel zu speichern. Wenn Sie ein Hardwaresicherheitsmodul verwenden möchten, stellen Sie sicher, dass die Treiber einwandfrei konfiguriert sind und die Sicherheitsumgebung definiert ist.
-   Wenn Ihr RMS-Computer über eine Verbindung zum Internet verfügt, können Sie während der Bereitstellung automatisch ein Server-Lizenzgeberzertifikat herunterladen. Wenn die Organisation für die Verbindung mit dem Internet einen Proxyserver verwendet, überprüfen Sie die Proxyeinstellungen in Internet Explorer, einschließlich aller Authentifizierungsanforderungen, und zeichnen Sie diese für eine spätere Verwendung auf.
-   Wenn Sie RMS auf einem Domänencontroller ausführen und ein Benutzerkonto verwenden möchten, um die RMS-Dienste auszuführen, stellen Sie sicher, dass die Sicherheitsrichtlinie für Domänencontroller so konfiguriert ist, dass dem Benutzerkonto die lokale Anmeldeberechtigung erteilt wird. Weitere Informationen zum Konfigurieren der Sicherheitsrichtlinie für Domänencontroller finden Sie im Windows Server 2003 Hilfe- und Supportcenter.

**Schritt 2 – Bereitstellen des ersten RMS-Servers**

Als Bereitstellung bezeichnet man das Konfigurieren einer Website mit RMS, sodass Benutzer mit der Verwendung des Dienstes beginnen können. Führen Sie die folgenden Schritte aus, um den Stammzertifizierungsserver für Ihre Organisation bereitzustellen:

1.  Melden Sie sich am Computer als Domänenbenutzer mit lokalen Administratorrechten an. Wenn Sie RMS auf einem Domänencontroller installieren, melden Sie sich als Domänenadministrator an.
2.  Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Webseite **Globale Verwaltung** zu öffnen. Auf dieser Seite sind die Websites aufgeführt, die auf diesem Server verfügbar sind.
3.  Klicken Sie auf die Website, die Sie mit RMS bereitstellen möchten, und klicken Sie dann auf **RMS auf dieser Website bereitstellen**. Beim Öffnen der Seite wird oben Folgendes angezeigt: **RMS-Stammzertifizierungsserver bereitstellen**.
4.  Vervollständigen Sie die Seite, indem Sie die Informationen für Ihre Organisation eingeben.
    -   Geben Sie in das Feld **Cluster-URL** den Dienstnamen – z. B. certification.contoso.com – ein, den Sie unter Schritt 4 des vorherigen Verfahrens konfiguriert haben. Wenn Sie SSL mit der RMS-Installation verwenden möchten, klicken Sie in der Protokollliste auf das Protokoll HTTPS. Hierdurch wird SSL aktiviert. Dies bedeutet jedoch nicht, dass SSL für die RMS-Webdienste erforderlich ist. Diese Option muss separat über IIS konfiguriert werden.
    -   Ist der Server über einen Proxyserver mit dem Internet verbunden, füllen Sie im Bereich **RMS-Proxyeinstellungen** die von Internet Explorer erfassten Informationen fertig aus und befolgen Sie dabei die Anleitungen im Teil über die optionalen Funktionen des vorherigen Verfahrens.
    -   Wählen Sie im Bereich **Serverinternetkonnektivität** die Option **Online**, wenn der Server über das Internet eine Verbindung zum Microsoft-Registrierungsdienst herstellen und während des Bereitstellungsvorgangs automatisch ein Server-Lizenzgeberzertifikat erhalten soll. Wählen Sie **Offline**, wenn Sie die Verbindung zum Microsoft-Registrierungsdienst manuell herstellen, das Server-Lizenzgeberzertifikat downloaden und das Zertifikat nach der Bereitstellung von RMS importieren möchten.
5.  Klicken Sie auf **Absenden**.
    In ungefähr 60 bis 90 Sekunden ist die Bereitstellung erfolgreich abgeschlossen. Sie können dann zur Seite **Globale Verwaltung** zurückkehren und den neu bereitgestellten Server mit RMS verwalten.
6.  Wählen Sie auf der Seite **Globale Verwaltung** die Option **RMS auf dieser Website verwalten**, um die **Verwaltungsstartseite** für den RMS-Server zu öffnen.
    Wenn Sie in Schritt 4 für „Serverinternetkonnektivität“ die Option „Offline“ gewählt haben, führen Sie das Verfahren „So registrieren Sie einen Stammzertifizierungsserver manuell“ aus, bevor Sie fortfahren.
7.  Klicken Sie auf der Verwaltungsstartseite auf die Verknüpfung **RMS-Dienstverbindungspunkt**.

| ![](images/Cc747735.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Für den nächsten Schritt in diesem Verfahren, der Registrierung eines Dienstverbindungspunkts, ist ein Domänenkonto mit ausreichenden Berechtigungen zum Erstellen eines Containerobjekts unter dem Dienstecontainer im Konfigurationscontainer der Active Directory-Gesamtstruktur erforderlich. Die vordefinierte Sicherheitsgruppe **Organisations-Admins** ist ein Beispiel für ein Konto mit den erforderlichen Berechtigungen. |

1.  Klicken Sie auf der Seite **RMS-Dienstverbindungspunkt** auf die Schaltfläche **URL registrieren**. Dadurch wird der RMS-Dienstverbindungspunkt in Active Directory registriert, sodass RMS-fähige Anwendungen RMS-Lizenzierungsdienste, Aktivierungsproxydienste und Zertifizierungsdienste suchen können.

**Schritt 3 – Testen von RMS**

Bevor Sie RMS vollständig verwenden können, müssen Sie den RMS-Client und eine RMS-fähige Anwendung auf den Clientcomputern installieren. Benutzer sollten Mitglied der Active Directory-Domäne sein, und die Clientcomputer sollten zu dieser Domäne hinzugefügt werden. Domänenbenutzer sollten außerdem über E-Mail-Adressen verfügen, die in Active Directory definiert sind. So testen Sie RMS:

1.  Melden Sie sich am Clientcomputer als gültiger Domänenbenutzer an.
2.  Installieren Sie den RMS-Client für Service Pack 1.
3.  Installieren Sie eine RMS-fähige Anwendung.
4.  Erstellen Sie eine RMS-geschützte Datei, erteilen Sie allen Benutzern Nur-Lese-Rechte für diese Datei, und speichern Sie die Datei dann in einem freigegebenen Ordner, auf den die Benutzer Vollzugriff haben.
5.  Melden Sie sich als ein anderer Benutzer am Computer an. Öffnen Sie die Datei, und versuchen Sie, Änderungen vorzunehmen. Wenn RMS ordnungsgemäß installiert ist, können Sie keine Änderungen an der Datei durchführen.
