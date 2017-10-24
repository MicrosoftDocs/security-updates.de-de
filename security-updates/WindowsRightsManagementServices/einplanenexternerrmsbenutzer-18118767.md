---
TOCTitle: 'Einplanen externer RMS-Benutzer'
Title: 'Einplanen externer RMS-Benutzer'
ms:assetid: '107e1338-4dcf-4ed5-a49d-e875cc883db1'
ms:contentKeyID: 18118767
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720190(v=WS.10)'
---

Einplanen externer RMS-Benutzer
===============================

In diesem Abschnitt werden Topologien beschrieben, durch deren Implementierung eine Organisation sowie auch externe Benutzer über das Internet auf RMS-geschützte Inhalte zugreifen können.

Mithilfe der folgenden Optionen können Sie RMS-Cluster sowohl für interne als auch externe Nutzung bereitstellen:

-   Legen Sie für den Stammzertifizierungscluster einen URL fest, auf den über das Internet zugegriffen werden kann. Stellen Sie sicher, dass dieser URL im Intranet für RMS-Server aus dem gleichen Cluster erreichbar ist. In diesem Fall ist der URL der Veröffentlichungslizenz, der von Endbenutzer-Computern für den Lizenzerwerb verwendet wird, sowohl im Intranet als auch über das Internet erreichbar.
-   Richten Sie einen separaten RMS-Cluster ein, der nur für die Internetveröffentlichung vorgesehen ist. Jeder Inhalt, der über das Internet lizenziert werden muss, sollte auf diesem Cluster veröffentlicht werden. Wenn Inhalte intern und extern verfügbar sein müssen, sollten sie an beiden Speicherorten veröffentlicht werden. Alternativ hierzu müssen Benutzer auf den Internetserver zuzugreifen können.

Zulassen externer Benutzer
--------------------------

Sie können externe Benutzer in Ihre RMS-Installation einbinden, indem Sie interne Konten für sie einrichten und ihnen gestatten, über ein virtuelles Privatnetzwerk (Virtual Private Network = VPN) auf das Unternehmensnetzwerk zuzugreifen. Das Konto kann über ein internes Postfach oder eine E-Mail-Adresse verfügen, die mit einem externen Postfach verknüpft ist.

Wenn ein internes Postfach verwendet wird, müssen intern verfasste Nachrichten mit der E-Mail-Adresse versehen werden, die mit diesem internen Postfach verbunden ist, wenn RMS-geschützte Inhalte veröffentlicht werden sollen. E-Mail-Adressen, die von externen Benutzern außerhalb der Organisation verwendet werden, sind nicht dazu geeignet. Wenn ein externes Postfach verwendet wird, müssen intern verfasste Nachrichten mit der externen E-Mail-Adresse des Kontos versehen werden, wenn RMS-geschützte Inhalte veröffentlicht werden sollen.

Um die Netzwerksicherheit zu gewährleisten und zugleich den Netzwerkzugriff für externe Benutzer bereitzustellen, ist es möglich, eine separate Active Directory-Struktur für Partnerkonten zu erstellen. Mit dieser Topologie können Sie einen separaten Stammzertifizierungscluster für den mit dem Internet verbundenen Teil des RMS-Systems einrichten. Auf diese Weise können externe Benutzer RMS-Computerzertifikate und Rechtekontozertifikate über diesen für das Internet zuständigen Stammzertifizierungscluster erhalten, wenn Sie das erste Mal Zugriff auf durch RMS geschützte Inhalte erhalten.

Wenn Sie eine separate Struktur für externe Partner einrichten, die auch die Partnerkonten umfasst, muss RMS in dieser Struktur installiert werden. Sie können mit dem RMS-Feature für vertrauenswürdige Veröffentlichungsdomänen Vertrauensstellungen zwischen den beiden RMS-Servern herstellen. Darüber hinaus ist erforderlich, dass die externen DNS-Datensätze den externen Cluster-URL der RMS-Installation in der für externe Partner erstellten Struktur identifizieren. Das Herstellen dieser Vertrauensstellung ermöglicht es dem externen RMS-Server, Lizenzen für alle Inhalte auszustellen, die vom internen RMS-System ausgestellt werden, und umgekehrt.

Als Alternative zum Einrichten eines RMS-Servers in einer externen Struktur können Sie beispielsweise auch einen ISA-Server verwenden, um eingehenden Verkehr zu filtern und Proxy-Lizenzanforderungen an den internen RMS-Server umzukehren.

Verwenden externer Zertifikate
------------------------------

Sie können externen Benutzern Zugriff auf RMS-geschützte Inhalte erteilen, indem Sie einen separaten RMS-Server als internetseitigen Lizenzierungsserver einrichten, die Inhalte auf diesem Lizenzierungsserver veröffentlichen und dann die Vertrauensbeziehungen auf diesem Server festlegen.

Der internetseitige Bereich von RMS stellt einen separaten Lizenzierungsserver dar, der für die Kommunikation mit dem Internet vorgesehen ist. Der Lizenzierungsserver ist Teil desselben Clusters wie die interne Lizenzierungsinstallation. Er verwendet dieselbe Datenbank und denselben URL wie die interne Lizenzierungsinstallation, kann aber als einziger Server eingehenden Internetdatenverkehr empfangen.

Wenn externe Benutzer eine Nutzungslizenz über diesen RMS-Lizenzierungsserver anfordern, werden sie dies mithilfe eines Rechtekontozertifikats eines anderen RMS-Zertifizierungsdienstes tun, das beim Lizenzierungsserver eine Vertrauensstellung hat.

#### Vertrauen auf Passport-basierte Rechtekontozertifikate

Eine Organisation kann sich entscheiden, Rechtekontozertifikaten zu vertrauen, die auf Microsoft .NET Passport-Anmeldeinformationen beruhen. Diese Kontozertifikate machen es für Benutzer erforderlich, Rechtekontozertifikate direkt vom Microsoft Certification Service (Zertifizierungsdienst von Microsoft) aus dem Internet zu beziehen.

In einem solchen Fall erhalten externe Benutzer RMS-Computerzertifikate und Rechtekontozertifikate von Microsoft. Wenn Inhalte veröffentlicht werden, muss das Microsoft .NET Passport-Konto des externen Benutzers als Empfänger der Veröffentlichungslizenz angegeben werden.

Das Microsoft® .NET Passport-Konto muss dem .NET Passport-Konto entsprechen, das beim Herunterladen des Rechtkontozertifikats bei Microsoft angegeben wurde. Der Autor muss dieses Konto angeben, wenn er Empfänger in der RMS-fähigen Anwendung hinzufügt. Wenn die Konten nicht übereinstimmen, können die Inhalte nicht verwendet werden.

#### Vertrauen bei sonstigen externen Zertifikaten

Wenn das Unternehmen des externen Benutzers ebenfalls über eine RMS-Instanz verfügt, ist es möglich, eine Vertrauensstellung mit diesem Unternehmen einzurichten. Zu diesem Zweck muss das Unternehmen sein RMS-Server-Lizenzgeberzertifikat exportieren und Ihnen übermitteln. Sie können dieses Zertifikat anschließend mithilfe der RMS-Verwaltungskonsole für Ihren internetseitigen Lizenzierungsserver importieren.