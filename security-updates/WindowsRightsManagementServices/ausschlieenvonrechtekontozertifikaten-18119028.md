---
TOCTitle: Ausschließen von Rechtekontozertifikaten
Title: Ausschließen von Rechtekontozertifikaten
ms:assetid: 'cba5e901-942c-4d06-9865-e6c4648c95e6'
ms:contentKeyID: 18119028
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747670(v=WS.10)'
---

Ausschließen von Rechtekontozertifikaten
========================================

Wenn ein Benutzer zwar vertrauenswürdig ist, seine RMS-Anmeldeinformationen (Rights Management Services oder Dienste für die Rechteverwaltung) aber unsicher geworden sind, können Sie das Rechtekontozertifikat des Benutzers durch Ausschließen seines öffentlichen Schlüssels ausschließen. RMS lehnt daraufhin neue Nutzungslizenzanforderungen ab, bei denen dieses Kontozertifikat verwendet wird. Wenn ein Benutzer nach dem Ausschluss eines Rechtekontozertifikats versucht, eine Nutzungslizenz für neue Inhalte zu erwerben, wird die Anforderung abgelehnt. Der Benutzer muss in diesem Fall ein neues Rechtekontozertifikat mit einem neuen Schlüsselpaar abrufen, um eine Nutzungslizenz zu erwerben.

Rechtekontozertifikate können mithilfe der Seite **Ausschlussrichtlinien** der Verwaltungswebsite ausgeschlossen werden. Wenn Sie das Rechtekontozertifikat eines Benutzers ausschließen, fügt RMS den ausgeschlossenen Schlüssel, den Kontonamen des Benutzers sowie das Datum und die Uhrzeit des Ausschlusses der Tabelle DRMS\_GicExclusionList der Konfigurationsdatenbank des Stammzertifizierungsclusters hinzu. Diese Informationen werden auch auf der Seite **Ausschlussrichtlinien** der Verwaltungswebsite angezeigt. Darüber hinaus löscht RMS sowohl die öffentlichen als auch die dem ausgeschlossenen Kontozertifikat zugeordneten privaten Schlüssel aus der Tabelle UD\_Users der Konfigurationsdatenbank.

Geben Sie auf der Seite **Ausschlussrichtlinien** des Stammzertifizierungsservers das Domänenkonto des Benutzers an, um ein Rechtekontozertifikat auszuschließen, das sich auf dem Stammzertifizierungsserver oder -cluster befindet. Ein Rechtekontozertifikat muss auf den Servern der Unterregistrierung auf den Verwaltungswebsites der einzelnen Server ausgeschlossen werden. Geben Sie den Wert des öffentlichen Schlüssels des Rechtekontozertifikats auf der Seite **Ausschlussrichtlinien** der Verwaltungswebsite des Lizenzierungsservers ein, um einen Benutzer auf einem Lizenzierungsserver oder -cluster in der Unterregistrierung auszuschließen. Diesen Wert erhalten Sie auf der Seite **Ausschlussrichtlinien** der Verwaltungswebsite des Stammzertifizierungsclusters.

Um den Ausschluss von Rechtekontozertifikaten in einer aus mehreren Clustern bestehenden RMS-Bereitstellung zu vereinfachen, können Sie die Tabelle DRMS\_GicExclusionList aus der Konfigurationsdatenbank des Stammzertifizierungsclusters in die Konfigurationsdatenbank jedes Lizenzierungsclusters replizieren. Bei dieser Vorgehensweise müssen Sie den Wert des öffentlichen Schlüssels nicht manuell auf jedem Server eingeben.
