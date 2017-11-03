---
TOCTitle: Verwenden der Verwaltungsstartseite
Title: Verwenden der Verwaltungsstartseite
ms:assetid: '6c155977-bd0e-47d6-ac65-1746cddb505e'
ms:contentKeyID: 18118885
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720290(v=WS.10)'
---

Verwenden der Verwaltungsstartseite
===================================

Auf der Webseite der **Verwaltungsstartseite** können Sie Informationen zum Server oder Cluster anzeigen und auf Verwaltungsoptionen zugreifen. Diese Seite ist erst nach der Bereitstellung der Server verfügbar.

Führen Sie die folgenden Schritte aus, um von dem zu verwaltenden Server Zugriff auf diese Website zu erhalten:

1.  Melden Sie sich als lokaler Administrator an.
2.  Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**.
3.  Klicken Sie auf der Seite **Globale Verwaltung** auf **RMS auf dieser Website verwalten**.

Wenn Sie die Remoteverwaltung mithilfe von SSL (Secure Socket Layer) aktiviert haben, können Sie auf folgende Weise auch von einem anderen Computer auf die **Verwaltungsstartseite** zugreifen:

1.  Geben Sie in der Adressleiste des Webbrowsers den folgenden URL ein:
    https://*Clustername:Portnummer*/\_wmcs/admin
    Dabei ist *Clustername:Portnummer* der URL (Uniform Resource Locator), den Sie bei der Bereitstellung für diesen Cluster angegeben haben. Die Angabe der Portnummer ist nur dann erforderlich, wenn Sie eine andere Portnummer als den Standardwert 80 angegeben haben.
2.  Geben Sie bei Aufforderung die Anmeldeinformationen eines lokalen Administrators des Servers ein, auf den Sie zugreifen.

Auf der **Verwaltungsstartseite** werden beispielsweise folgende Informationen zum Cluster angezeigt: der Cluster-URL, der Name und Speicherort der Konfigurationsdatenbank, das Ablaufdatum des Server-Lizenzgeberzertifikats usw. Hier werden darüber hinaus Verknüpfungen zu Seiten bereitgestellt, auf denen Sie die folgenden Verwaltungsoptionen für den Cluster konfigurieren können:

-   **Vertrauensrichtlinien.** Hinzufügen und Entfernen von vertrauenswürdigen Domänen. Weitere Informationen finden Sie nachstehend unter „[Verwalten von Vertrauensstellungen und Vertrauensrichtlinien](https://technet.microsoft.com/1c96ee74-fd28-4511-be21-087e2b04c3ee)“.
-   **Vorlagen für Benutzerrechterichtlinien**. Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien. Weitere Informationen finden Sie nachstehend unter „[Verwalten von Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/718286dc-3399-4556-96c9-ec3a33d31877)“.
-   **Protokollierungseinstellungen**. Aktivieren und Deaktivieren der Protokollierung und Anzeigen der Namen des Protokollierungsservers und der Protokollierungsdatenbank. Weitere Informationen finden Sie nachstehend unter „[Verwalten der Protokollierung](https://technet.microsoft.com/8fccfc57-2135-494e-8e44-f6191bf5e4a0)“.
-   **Einstellungen für Extranet-Cluster-URL.** Angeben eines extern verfügbaren URLs für Lizenzierungs- und Kontozertifizierungsanforderungen. Weitere Informationen finden Sie nachstehend unter „[Konfigurieren eines Extranet-URLs](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)“.
-   **RMS-Proxyeinstellungen.** Geben Sie die Adresse des Proxyservers, den Authentifizierungstyp und den Benutzernamen an. Diese Informationen werden verwendet, wenn der Server mit RMS eine Internetverbindung über einen Proxyserver herstellen muss. Weitere Informationen finden Sie unter nachstehend „[Konfigurieren von RMS-Proxyeinstellungen](https://technet.microsoft.com/179d2970-62e9-4487-aa5b-f4334234991e)“.
-   **Sicherheitseinstellungen.** Zurücksetzen des Kennwortes für den privaten Serverschlüssel, Angeben der Administratorengruppe, deren Mitglieder die gesamten lizenzierten Inhalte entschlüsseln können, sowie Außerbetriebsetzen von RMS (Rights Management Services oder Dienste für die Rechteverwaltung). Weitere Informationen finden Sie nachstehend unter „[Verwalten der Sicherheit bei der Verwendung von RMS](https://technet.microsoft.com/62050812-de4f-4392-8d63-f2f89aa01ed4)“.
-   **Zertifizierungseinstellungen.** Angeben des Gültigkeitszeitraums von Rechtekontozertifikaten und Angeben eines Administratorkontakts. (Diese Option ist nur im Stammzertifizierungscluster verfügbar, nicht aber auf Lizenzierungsservern.) Weitere Informationen finden Sie nachstehend unter „[Verwalten von Rechtekontozertifikaten](https://technet.microsoft.com/49c5c2ba-e197-4e4b-b3b3-b3248f068bcc)“.
-   **Ausschlussrichtlinien.** Angeben des Ausschlusses mithilfe der Lockbox-Version, des Rechtekontozertifikats, der Windows-Version oder der RMS-fähigen Anwendung. Weitere Informationen finden Sie nachstehend unter „[Verwalten von Ausschlussrichtlinien](https://technet.microsoft.com/ee31e099-e095-4648-95da-0009fbeb48cb)“.
-   **RM-Kontozertifizierungsbericht.** Anzeigen der Anzahl von ausgestellten Rechtekontozertifikaten. (Diese Option ist nur im Stammzertifizierungscluster verfügbar, nicht aber auf Lizenzierungsservern.) Weitere Informationen finden Sie nachstehend unter „[Nachverfolgen von Rechtekontozertifikaten](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)“.

In den verbleibenden Themen dieses Abschnitts wird die Verwendung dieser Features beschrieben. Schrittweise Anleitungen hierzu finden nachstehend Sie unter „[Vorgehensweisen bei RMS](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)“.

> [!NOTE]
> Einige Funktionen können auf der RMS-Verwaltungswebsite in Popup-Fenstern konfiguriert werden. Wenn Sie in Ihrem Webbrowser Popup-Blocker verwenden, sollten Sie Ihre Browsereinstellungen dahingehend ändern, dass Popup-Fenster der RMS-Verwaltungswebsite zugelassen werden. 