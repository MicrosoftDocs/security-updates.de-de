---
TOCTitle: 'RMS-Kontozertifizierung'
Title: 'RMS-Kontozertifizierung'
ms:assetid: 'c9a385c5-6dbb-47f5-a80f-69718e6f9deb'
ms:contentKeyID: 18119007
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747750(v=WS.10)'
---

RMS-Kontozertifizierung
=======================

Beim Prozess der Kontozertifizierung wird ein Rechtekontozertifikat erstellt, das ein Benutzerkonto einem bestimmten Computer zuordnet und es dem Benutzer ermöglicht, RMS-geschützten Inhalt von diesem Computer abzurufen. Wenn ein Benutzer zum ersten Mal RMS-geschützten Inhalt veröffentlicht oder versucht, RMS-geschützten Inhalt von einem Clientcomputer abzurufen, sendet die RMS-fähige Anwendung eine Anforderung für ein Rechtekontozertifikat an den RMS-Kontozertifizierungsdienst.

Der Zertifizierungsdienst kann den Benutzer entweder über die Windows-Authentifizierung oder über ein x.509-Zertifikat authentifizieren, das in einem Gerät für Hardwareverschlüsselung, wie z. B. einer Smartcard gespeichert ist. Nach der Authentifizierung des Benutzers erstellt der RMS-Server ein Rechtekontozertifikat für den Benutzer, das auf dessen authentifizierten Anmeldeinformationen basiert. Er verschlüsselt den privaten Schlüssel des Benutzers mit dem öffentlichen Schlüssel des RMS-Computerzertifikats des Clientcomputers und fügt dabei den verschlüsselten Schlüssel in das Rechtekontozertifikat ein. Dann stellt er das Rechtekontozertifikat für die anfordernde Anwendung aus, die das Rechtekontozertifikat auf dem Computer oder Gerät speichert, so dass es für nachfolgende Anforderungen von Veröffentlichungs- oder Nutzungslizenzen verfügbar ist. Das Rechtekontozertifikat wird darüber hinaus auch in der Konfigurationsdatenbank gespeichert.

Die Kontozertifizierung wird erst nach dem Prozess zur Computeraktivierung ausgeführt, da das RMS-Computerzertifikat des Clientcomputers für die Anforderung des Rechtekontozertifikats erforderlich ist.

Benutzer müssen für jeden von ihnen verwendeten Computer ein Rechtekontozertifikat erwerben. Wenn ein Benutzer auf mehreren Computern arbeitet, wird für jeden dieser Computer ein eindeutiges Rechtekontozertifikat ausgestellt, obwohl auf allen Computern dasselbe Schlüsselpaar für diesen Benutzer verwendet wird.

Wenn eine RMS-fähige Anwendung eine Nutzungslizenz anfordert, wird das Rechtkontozertifikat in die Anforderung eingefügt. Der Lizenzierungsdienst verwendet den öffentlichen Schlüssel des Rechtekontozertifikats zum Verschlüsseln des Inhaltsschlüssels. Dadurch wird sichergestellt, dass nur der authentifizierte Benutzer die Lizenz verwenden kann.

Der Kontozertifizierungsprozess besteht aus folgenden Schritten:

1.  Wenn ein Benutzer zum ersten Mal RMS-geschützten Inhalt veröffentlicht oder versucht, RMS-geschützten Inhalt von einem bestimmten Computer abzurufen, sendet die RMS-fähige Anwendung eine Anforderung für ein Rechtekontozertifikat an den Kontozertifizierungsdienst, der auf dem Stammzertifizierungsserver ausgeführt wird.
2.  Der Kontozertifizierungsdienst authentifiziert den Benutzer mithilfe der Windows-Authentifizierung.
3.  Der Kontozertifizierungsdienst erstellt ein Rechtekontozertifikat für den Benutzer, das auf dessen authentifizierten Anmeldeinformationen basiert. Er verschlüsselt den privaten Schlüssel des Benutzers mit dem öffentlichen Schlüssel des RMS-Computerzertifikats und fügt den verschlüsselten Schlüssel in das Zertifikat ein. Dann stellt er der anfordernden Anwendung das Rechtekontozertifikat aus.
4.  Die Anwendung speichert das Rechtekontozertifikat auf dem Computer oder Gerät, so dass es für nachfolgende Anforderungen von Veröffentlichungs- oder Nutzungslizenzen verfügbar ist.

Der Kontozertifizierungsdienst, den der Client zum Anfordern des Rechtekontozertifikats verwendet, hängt von der Art des Computers ab, auf dem der RMS-Client installiert ist. Standardmäßige Desktopcomputer stellen eine Verbindung zum Kontozertifizierungsdienst (certification.asmx) her. Serverdienste, die für die Verwendung mit RMS SP1 aktiviert wurden, erhalten Rechtekontozertifikate vom Serverzertifizierungsdienst (ServeCertfication.asmx). Mobile Geräte, die für die Verwendung mit RMS SP1 aktiviert wurden, erhalten Rechtekontozertifikate vom Zertifizierungsdienst für mobile Geräte (MobileDeviceCertfication.asmx). In einer Standardinstallation von RMS SP1 ist nur der Kontozertifizierungsdienst aktiviert.

Weitere Informationen zur Verwendung von RMS SP1 mit mobilen Geräten und Serverdiensten finden Sie unter „Aktivieren der RMS-Serverunterstützung für mobile Geräte und Serverdienste“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.
