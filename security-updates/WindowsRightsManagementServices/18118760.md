---
TOCTitle: 'Betreiben eines RMS-Servers'
Title: 'Betreiben eines RMS-Servers'
ms:assetid: '1533426b-89c2-43e0-8068-ca97ddab8606'
ms:contentKeyID: 18118760
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720205(v=WS.10)'
---

Betreiben eines RMS-Servers
===========================

Das Betreiben eines RMS-Server bezieht sich auf die Verwaltungsaufgaben, die nach der Bereitstellung von RMS in einer Organisation durchgeführt werden. Dieses Thema behandelt die Verwaltung des RMS-Servers, das Durchführen häufiger Verwaltungsaufgaben und die Verwaltung von Ressourcen für zusätzliche Informationen, sowie bewährte Methoden.

In diesem Thema

-   [Verwalten von RMS](https://technet.microsoft.com/9b573c55-c14c-436c-b3c5-7ba445de1562)
-   [Vorgehensweisen bei RMS](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)
-   [RMS-Ressourcen](https://technet.microsoft.com/d91221cf-e38e-4add-b7b9-50e63aad9a28)

In diesem Handbuch verwendete Terminologie
------------------------------------------

**Kontozertifizierung**  
Der Prozess, bei dem im Rechtekontozertifikat (RAC) Benutzerkonten Schlüsselpaare zugeordnet werden

**Kontozertifizierungsdienst**  
Ein RMS-Webdienst, der Rechtekontozertifikate erstellt und verteilt. Siehe auch Kontozertifizierung.

**Aktivierungsproxydienst**  
Ein RMS-Webdienst, der Computeraktivierung von RMS-Clients der Version 1.0 unterstützt. Wird zum Weiterleiten von Computeraktivierungsanforderungen an den Microsoft-Aktivierungsdienst verwendet. Dieser erstellt eine einmalige Lockbox und ein entsprechendes RMS-Computerzertifikat für den Clientcomputer, das vom Aktivierungsproxydienst auf dem Server mit RMS dann zurück zu dem Client geleitet wird, der das Zertifikat angefordert hat. Siehe auch Lockbox.

**Verwaltungsdienst**  
Ein RMS-Webdienst, der die Verwaltungswebsite hostet, die die RMS-Verwaltung ermöglicht und die Konfigurationsdatenbank für den Cluster aktualisiert.

**Anwendungsmanifest**  
Ein XML-Dokument, das die Module einer zugeordneten RMS-fähigen Anwendung beschreibt und in der Anwendungsumgebung ausgeführt werden kann. Jede Anwendung, die zur Erstellung oder zum Einsatz von RMS-geschützten Daten an APIs des RMS-Client schreibt, muss ein Manifest zur Laufzeit bereitstellen.

**Attribut**  
Eine Objekteigenschaft in Active Directory. Das Schema definiert für jede Objektklasse, welche Attribute eine Instanz einer Klasse aufweisen muss und welche zusätzlichen Attribute möglicherweise zutreffen.

**Bindung**  
Der Mechanismus zum Ausführen von Rechten in einem RMS-System. Der RMS-Client prüft dabei die Bedingungen einer Nutzungslizenz gegen die angeforderten Rechte. Wenn diese Bedingungen erfüllt werden, werden die Rechte erteilt.

**Zertifikat**  
Ein digitales Dokument, das in der Regel zur Authentifizierung und Sicherung von Informationen auf offenen Netzwerken verwendet wird. Ein Zertifikat bindet einen öffentlichen Schlüssel sicher an eine Entität, die mit dem entsprechenden privaten Schlüssel versehen ist. Zertifikate werden von der herausgebenden Zertifizierungsstelle digital signiert und können für einen Benutzer, einen Computer oder einen Dienst ausgestellt werden. Siehe auch privater Schlüssel; öffentlicher Schlüssel.

**Clientregistrierung**  
Der Erstellungsprozess des Client-Lizenzgeberzertifikats, das es dem Computer oder Gerät des Benutzers ermöglicht, Veröffentlichungslizenzen zu erstellen, die von einem Lizenzierungsserver berücksichtigt werden.

**Client-Lizenzgeberzertifikat**  
Das von einem Server mit RMS erstellte und auf Clientcomputern mit RMS gespeicherte Zertifikat, das es Benutzern ermöglicht, geschützte Inhalte offline zu veröffentlichen, ohne mit dem RMS-fähigen Netzwerk verbunden zu sein. Das Client-Lizenzgeberzertifikat enthält den Schlüssel, den der RMS-Client zum digitalen Signieren von Veröffentlichungslizenzen verwendet.

**Bedingung**  
Eine Reihe von angegebenen Einschränkungen und Parametern, die Teil der als Gruppe in einer Veröffentlichungslizenz gebündelten Rechte sind. Diese Einschränkungen und Parameter werden beim Abrufen erzwungen. Häufig wird eine zeitliche Einschränkung als Bedingung eingesetzt, über die der Benutzer ein Ablaufdatum für RMS-geschützte Daten einrichten kann.

**Konfigurationsdatenbank**  
Die Datenbank, die die RMS-Konfigurationsdaten für einen Server oder Cluster enthält.

**Abrufen von Inhalt**  
Entschlüsseln von geschütztem Inhalt und Verwenden von Benutzerrechten für geschützten Inhalt.

**Inhaltsschlüssel**  
Der Schlüssel, der zum Verschlüsseln und Entschlüsseln von geschützten Inhalten während der Veröffentlichung und während des Abrufens verwendet wird. Der Inhaltsschlüssel wird auch als symmetrischer Schlüssel bezeichnet. RMS verwendet AES-Inhaltsschlüssel mit 128 Bit.

**Inhaltsanbieter**  
Die Person oder Organisation, die die Zugriffsrichtlinie für geschützten Inhalt einrichtet.

**Entschlüsselung**  
Das Verfahren, bei dem verschlüsselte Daten wieder lesbar gemacht werden, indem chiffrierter Text in Nur-Text konvertiert wird.

**Digitale Signatur**  
Damit können Verfasser von Nachrichten, Dateien oder anderen digital codierten Informationen ihre Identität an die Information binden. Beim digitalen Signieren von Informationen werden Daten sowie vom Absender geheim gehaltene Informationen in die so genannte Signatur umgewandelt. Digitale Signaturen werden in Umgebungen mit öffentlichen Schlüsseln verwendet und stellen Nachweisbarkeits- und Integritätsdienste bereit.

**DRMRemote-Dienst**  
Ein RMS-Webdienst, der Dienste über .NET Remoting darstellt, das für die Kommunikation zwischen unterschiedlichen Servern mit RMS verwendet wird.

**Verschlüsselung**  
Vorgang, bei dem Informationen in eine Form umgewandelt werden, die nur von einem speziellen Empfänger gelesen werden kann. Die Verschlüsselung stellt eine effektive Möglichkeit zur vertraulichen Behandlung von Daten dar. Der Empfänger muss den geheimen Schlüssel oder ein Kennwort besitzen, um eine verschlüsselte Datei zu entschlüsseln. Siehe auch Verschlüsselung eines öffentlichen Schlüssels.

**Registrierung**  
Der Prozess, bei dem der Stammzertifizierungsserver ein Server-Lizenzgeberzertifikat erhält, das durch den Microsoft-Registrierungsdienst signiert ist.

**Registrierungsanforderung**  
Eine Anforderung vom RMS-Stammzertifizierungsserver an den Microsoft-Registrierungsdienst zum Erhalt eines Server-Lizenzgeberzertifikats.

**Ausschluss**  
Der Prozess, bei dem der RMS-Server eine Ausschlussrichtlinie zum Verweigern einer Nutzungslizenzanforderung für einen Client basierend einsetzt. Siehe auch Ausschlussliste.

**Ausschlussliste**  
Liste von Prinzipalen, denen durch den RMS-Lizenzierungsdienst Lizenzen verweigert werden sollen.

**Ausschlussrichtlinie**  
Einstellungen in der RMS-Konfigurationsdatenbank, die das Ausschlussverhalten in einer Organisation steuern.

**eXtensible Rights Markup Language (XrML)**  
Das Format auf XML-Basis, das von RMS für alle unterstützten Lizenzen verwendet wird: Computerzertifikate, RACs, CLCs, Nutzungslizenzen, Veröffentlichungslizenzen und Server-Lizenzgeberzertifikate. Diese Dokumente legen die RMS-Richtlinie fest, die auf den geschützten Inhalt angewendet wird.

**Ausstellungslizenz**  
Daten, die die RMS-Richtlinie für geschützte Inhalte angeben.

**Lizenzierungscluster**  
Ein oder mehrere Server, der oder die die RMS-Lizenzierungs- und Veröffentlichungsdienste außerhalb des Stammzertifizierungsclusters ausführt bzw. ausführen. Diese Server verwenden einen gemeinsamen Datenbank- und Verbindungs-URL und sollten bei Einsatz mehrerer Server hinter einem Lastenausgleich für Software oder Hardware bereitgestellt werden. Im Gegensatz zu einem Zertifizierungs- oder Stammcluster kann der bzw. können die Server mit RMS in einem Lizenzierungscluster keine Benutzerzertifizierung ausführen.

**Lizenzierungsserver**  
Ein Server, der die RMS-Lizenzierungs- und Veröffentlichungsdienste außerhalb des Stammzertifizierungsclusters ausführt.

**Lizenzierungsdienst**  
Ein RMS-Webdienst, der Nutzungslizenzen ausstellt.

**Lockbox**  
Das Softwaremodul zum Authentifizieren der gültigen Verwendung von geschützten Inhalten, zum Verschlüsseln und Entschlüsseln von Daten und zum Schützen vertrauenswürdiger Softwareverarbeitung vor Änderung und Beobachtung. Eine RM-Lockbox wird auch als sicheres Repository bezeichnet.

**Protokollierungsdienst**  
Ein RMS-Protokollierungslistenerdienst, der protokollierte Daten von der Nachrichtenwarteschlange in die Protokollierungsdatenbank für den RMS-Server oder -Cluster überträgt.

**Computeraktivierung**  
Der Prozess zum Abrufen einer eindeutigen Lockbox und eines Computerzertifikats für einen Computer in RMS Version 1.0. Bei RMS Version 1.0 SP1 wird bei der Computeraktivierung ein Computerzertifikat für einen Benutzer dieses Computers empfangen.

**Manifest**  
Das signierte XML-Dokument, das die Bibliotheken oder Programme identifiziert, die in den Arbeitsspeicher für die Anwendung geladen oder nicht geladen werden dürfen.

**Microsoft-Aktivierungsdienst**  
Ein von Microsoft gehosteter Webdienst, der RMS-Computerzertifikate und Lockboxen als Antwort auf Anforderungen von RMS-Clients der Version 1.0 ausstellt.

**Microsoft-Registrierungsdienst**  
Ein von Microsoft gehosteter Webdienst, der ein Server-Lizenzgeberzertifikat für den Stammzertifizierungsserver in einer RMS-Bereitstellung ausstellt.

**Vorzertifizierung**  
Eine Funktion des RMS-Zertifizierungsdienstes, durch die eine Anwendung im Namen eines Benutzers vom Server mit RMS ein Rechtekontozertifikat anfordern kann. Rechtekontozertifikate, die unter Verwendung der Vorzertifizierung ausgestellt wurden, enthalten nur den öffentlichen Schlüssel des Benutzers.

**Prinzipal**  
Eine im RMS-Sicherheitsschema eingerichtete Entität (z. B. ein Administrator, der Benutzer, Gruppen oder geschützte Inhalte verwaltet), für die Objekte gesichert werden können.

**Privater Schlüssel**  
Die geheime Hälfte eines kryptografischen Schlüsselpaares, die mit einem öffentlichen Schlüsselalgorithmus verwendet wird. Private Schlüssel werden gewöhnlich verwendet, um Daten digital zu signieren oder um Daten zu entschlüsseln, die mithilfe des entsprechenden öffentlichen Schlüssels verschlüsselt wurden. Siehe auch öffentlicher Schlüssel; Verschlüsselung des öffentlichen Schlüssels.

**Bereitstellung**  
Das Konfigurieren eines Servers mit RMS für die Verwendung in einer Organisation.

**Öffentlicher Schlüssel**  
Die nicht geheime Hälfte eines kryptografischen Schlüsselpaares, die mit einem öffentlichen Schlüsselalgorithmus verwendet wird. Öffentliche Schlüssel werden gewöhnlich zum Verschlüsseln von Sitzungen, Überprüfen digitaler Signaturen oder Verschlüsseln von Daten verwendet, die mit dem entsprechenden privaten Schlüssel entschlüsselt werden können. Siehe auch privater Schlüssel; Verschlüsselung des öffentlichen Schlüssels.

**Verschlüsselung des öffentlichen Schlüssels**  
Eine Verschlüsselungsmethode, die zur Verschlüsselung zwei miteinander verbundene Schlüssel verwendet. Einer dieser Schlüssel ist der private Schlüssel, der geheim gehalten wird. Der andere Schlüssel, der öffentliche Schlüssel, wird an beliebige Empfänger ausgegeben. In der Regel verwendet der Absender zum Verschlüsseln einer Nachricht den öffentlichen Schlüssel des Empfängers. Nur der Empfänger besitzt den dazugehörigen privaten Schlüssel zum Entschlüsseln der Nachricht. Durch die Komplexität der Beziehung zwischen öffentlichem und privaten Schlüssel ist es bei ausreichender Länge beider Schlüssel rechnerisch unwahrscheinlich, den zweiten Schlüssel aus dem ersten abzuleiten. Wird auch asymmetrische Verschlüsselung genannt. Siehe auch privater Schlüssel; öffentlicher Schlüssel.

**Veröffentlichungslizenz**  
Die Lizenz, die beim Veröffentlichen von RMS-geschützten Inhalten erstellt wurde. Darin wird unter anderem festgelegt, wer auf den Inhalt zugreifen kann, welche Rechte gewährt werden und unter welcher Bedingung darauf zugegriffen werden kann. Die Veröffentlichungslizenz wird auch als eine Ausstellungslizenz bezeichnet.

**Veröffentlichungsdienst**  
Ein RMS-Dienst, der Veröffentlichungslizenzen signiert und Client-Lizenzgeberzertifikate ausstellt. Siehe auch Client-Lizenzgeberzertifikat; Veröffentlichungslizenz.

**RAC**  
Siehe auch Definition für das Rechtekontozertifikat.

**Sperrung**  
Das Auflisten von Entitäten, die über ungültige Lizenzen verfügen.

**Sperrliste**  
Ein XrML-basiertes Dokument, das die Zertifikate und Lizenzen auflistet, die vom Aussteller gesperrt wurden. Siehe auch Sperrung.

**Recht**  
Eine Aktion, die von angegebenen berechtigten Benutzern mit Inhalten ausgeführt werden kann, die durch RMS-Technologie geschützt sind. Diese Rechte können mithilfe von Bedingungen weiter eingeschränkt werden.

**Rechtekontozertifikat (RAC)**  
Das Zertifikat, das das Computerzertifikat der RMS-Aktivierung verwendet, um das Konto und den Schlüssel eines Benutzers an bestimmte Computer oder Computergruppen zu binden. Die Komponenten des Zertifikats werden verwendet, um es Benutzern zu ermöglichen, geschützte Inhalte zu verwenden. Rechtekontozertifikate werden im SDK (Software Development Kit) von RMS auch als Gruppenidentitätszertifikate (Group Identity Certificate oder GIC) bezeichnet.

**Rechteverwaltung**  
Eine Technologie, die dauerhaften Schutz für digitale Daten unter Verwendung von Verschlüsselung, Zertifikaten und Authentifizierung bietet. Autorisierte Empfänger oder Benutzer müssen eine Lizenz erwerben, um geschützte Dateien entsprechend der Rechte oder der Unternehmensregeln des Inhaltanbieters abzurufen.

**Client mit Diensten für die Rechteverwaltung (Client mit Rights Management Services; Client mit RMS)**  
Eine Gruppe von RMS-APIs, die auf jedem Clientcomputer in einem RMS-System installiert werden muss. Dies ist eine Voraussetzung für die Computeraktivierung und die Verwendung RMS-fähiger Anwendungen.

**Vorlage für Benutzerrechterichtlinien**  
Beschreibt eine Standardgruppe von Benutzern, Rechten und Bedingungen, die auf RMS-geschützte Inhalte angewendet werden kann. Wenn ein Benutzer eine Vorlage für Benutzerrechterichtlinien auf bestimmte Inhalte anwendet, werden die Rechte und Bedingungen der Vorlage Teil der Veröffentlichungslizenz.

**RMS-Aktivierung**  
Das Platzieren einer Lockbox auf den Computern von Endbenutzern in der RMS-Version 1.0. Dieser Vorgang kann ausschließlich durch einen RMS-Aktivierungsdienst erfolgen und ist für die Verwendung der RMS-Technologie wesentlich. Bei RMS Version 1.0 SP1 handelt es sich dabei um den Erhalt eines Computerzertifikats für einen Benutzer dieses Computers. Eine Verbindung zum RMS-Aktivierungsdienst ist dabei nicht erforderlich. RM-Aktivierung wird auch als Aktivierung bezeichnet.

**RMS-Zertifizierungsdienst**  
Ein von Microsoft gehosteter Webdienst, der Rechte-Kontozertifikate für Benutzer basierend auf deren Microsoft .NET Passport-Anmeldeinformationen ausstellt.

**Client mit RMS**  
Eine Gruppe von RMS-APIs, die auf jedem Clientcomputer in einem RMS-System installiert werden muss. Dies ist eine Voraussetzung für die Computeraktivierung und die Verwendung RMS-fähiger Anwendungen.

**RMS-Computerzertifikat**  
Das Zertifikat, das während der RMS-Aktivierung auf dem Computer von Endbenutzern gespeichert wird. Der öffentliche Schlüssel in diesem Zertifikat wird zur Verschlüsselung des privaten Schlüssels des Benutzers verwendet, der in den Rechtekontozertifikaten des Benutzers enthalten ist.

**RMS-fähige Anwendung**  
Eine Anwendung, die mithilfe des Software Development Kit (SDK) von RMS erweitert wurde, um es Benutzern zu ermöglichen, die Rechte anzugeben, die den von ihnen erstellten Inhalten zugeordnet sind.

**RMS-fähiger Computer**  
Ein Computer, auf dem die RMS-Clientkomponente installiert ist und die RMS-Computeraktivierung ausgeführt wurde, sodass RMS-geschützte Inhalte verarbeitet werden können.

**RMS-geschützter Inhalt**  
Digitale Informationen, die durch die RMS-Technologie geschützt sind.

**Stammzertifizierungscluster**  
Ein oder mehrere Server in einer RMS-Bereitstellung, auf dem oder auf denen Verwaltungs-, Registrierungs-, Kontozertifizierungs-, Aktivierungsproxy-, Lizenzierungs- und Veröffentlichungsdienste ausgeführt werden. Diese Server verwenden einen gemeinsamen Datenbank- und Verbindungs-URL und sollten hinter einem Lastenausgleich für Software oder Hardware bereitgestellt werden. Pro Active Directory-Gesamtstruktur darf nur ein Stammzertifizierungscluster vorhanden sein.

**Stammzertifizierungsserver**  
Der primäre Server in einer RMS-Bereitstellung, auf dem Verwaltungs-, Registrierungs-, Kontozertifizierungs-, Aktivierungsproxy-, Lizenzierungs- und Veröffentlichungsdienste ausgeführt werden. Pro Active Directory-Gesamtstruktur darf nur ein Stammzertifizierungsserver vorhanden sein.

**Vertrauensstamm**  
Eine vertrauenswürdige Entität, die die Basis für die Vertrauenswürdigkeit anderer Zertifikate darstellt. Alle Zertifikatsanbieter und der Endbenutzer müssen dem Stamm vertrauen.

**Sicherheits-ID (SID)**  
Eine Windows-Datenstruktur, durch die Benutzer-, Gruppen- und Computerkonten für Windows identifiziert werden. Für jedes Konto eines Netzwerks wird bei dessen Erstellung eine einmalige SID ausgegeben. In internen Prozessen in Windows wird vorzugsweise auf die SID eines Kontos verwiesen und nicht auf den Benutzer- oder Gruppennamen des Kontos.

**Server-Lizenzgeberzertifikat**  
Das Zertifikat, das die Anmeldeinformationen eines Servers mit RMS einrichtet und diesen zu einem gültigen und ausführbaren Zertifizierungs- und Lizenzierungsdienst macht. Das Lizenzgeberzertifikat enthält den öffentlichen Schlüssel, der zur Entschlüsselung von Inhaltsschlüsseln in Veröffentlichungslizenzen verwendet wird.

**Serverdienst**  
Ein RMS-Webdienst, der von einem anderen Dienst verwendet werden kann.

**Dienstverbindungspunkt (Service Connection Point oder SCP)**  
Ein Active Directory-Objekt, das auf den URL des Stammzertifizierungsclusters einer RMS-Bereitstellung verweist. Der RMS-Client verwendet diese Informationen zum Suchen von RMS-Diensten.

**Unterregistrierung**  
Teil des Bereitstellungsprozesses für einen Lizenzierungsserver, bei dem der Lizenzierungsserver ein Server-Lizenzgeberzertifikat vom Stammzertifizierungscluster erhält.

**Unterregistrierungsanforderung**  
Die Anforderung eines Server-Lizenzgeberzertifikats, die von einem Lizenzierungsserver an den Stammzertifizierungscluster gesendet wird.

**Unterregistrierungsdienst**  
Ein RMS-Webdienst auf dem Stammzertifizierungsserver, der auf Anforderungen von Server-Lizenzgeberzertifikaten antwortet, die von Lizenzierungsservern während der Bereitstellung gesendet werden.

**Administrator**  
Ein Mitglied der Administratorgruppe.

**Administratorgruppe**  
Eine optionale für administrative Zwecke definierte Benutzergruppe für jeden Cluster mit RMS, der Besitzerlizenzen durch den Server mit RMS erteilt werden, wenn von diesem Server veröffentlichte Inhalte abgerufen werden.

**Nutzungslizenz**  
Die Lizenz, die die Rechte und Bedingungen aufführt, unter denen ein Endbenutzer den geschützten Inhalt abrufen kann. Die Nutzungslizenz wird auch als Endbenutzerlizenz (End-user license oder EUL) bezeichnet.