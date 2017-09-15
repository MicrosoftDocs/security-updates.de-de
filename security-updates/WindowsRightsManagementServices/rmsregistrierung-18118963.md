---
TOCTitle: 'RMS-Registrierung'
Title: 'RMS-Registrierung'
ms:assetid: '999db3e1-e3ab-4513-87d9-d584ee334c00'
ms:contentKeyID: 18118963
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747698(v=WS.10)'
---

RMS-Registrierung
=================

Der Serverregistrierungsprozess erstellt und liefert ein Server-Lizenzgeberzertifikat. Mit Server-Lizenzgeberzertifikaten wird die Identität der Server in der Bereitstellung überprüft, und beim Abrufen RMS-geschützter Inhalte werden die Anmeldedaten geprüft. Der erste Server in jedem Lizenzierungscluster wird im Rahmen der Bereitstellung beim Stammzertifizierungscluster registriert. Die nachfolgenden Server im Cluster werden nicht separat registriert.

Der erste Server eines Stammzertifizierungsclusters (der Stammzertifizierungsserver) muss beim Microsoft-Registrierungsdienst registriert werden. Dieser Vorgang kann wahlweise automatisch im Rahmen der Bereitstellung erfolgen, sofern der Stammzertifizierungsserver mit dem Internet verbunden ist. Alternativ können Sie die Registrierung offline abwickeln; exportieren Sie hierzu eine Registrierungsanforderung in eine Datei, und senden Sie diese Datei über einen anderen Computer mit Internetverbindung an den Microsoft-Registrierungsdienst. Als Antwort auf die Registrierungsanforderung erhalten Sie ein Server-Lizenzgeberzertifikat für den Stammzertifizierungsserver, das dann mithilfe der RMS-Verwaltungswebseiten importiert werden kann.

Die Registrierungsanforderung enthält folgende Informationen:

-   Sperrinformationen. Geben an, ob die RMS-Installation standardmäßige oder benutzerdefinierte Sperrung (durch Dritte) verwendet. Wenn Sperrung durch Dritte eingesetzt wird, ist der öffentliche Schlüssel der Sperrstelle enthalten.
-   Öffentlicher Zertifikatschlüssel. Der öffentliche Schlüssel des Server-Lizenzgeberzertifikats. Dieser öffentliche Schlüssel wird auf dem RMS-Server erstellt und an den Microsoft-Registrierungsdienst gesendet, um das Server-Lizenzgeberzertifikat abzurufen.
-   SKU. Der offizielle SKU-Titel von RMS.
-   Version. Die Versionsnummer der RMS-Assemblierung.
-   URL. Der Basis-URL des RMS-Serverclusters.

Beim Beantworten der Registrierungsanforderung durch den Microsoft-Registrierungsdienst werden folgende Informationen im XML-Format an den RMS-Server zurückgegeben:

-   Server-Lizenzgeberzertifikat.
-   Zertifikatkette der Signaturstellen.

Es werden stets dieselben Informationen übermittelt, unabhängig davon, ob der RMS-Stammzertifizierungsserver im Online- oder Offline-Verfahren registriert wird. Bei keiner dieser Methoden werden weitere Informationen eingeholt.

Weitere Informationen zu den Schritten bei der Offline-Serverregistrierung finden Sie im Abschnitt „So registrieren Sie einen Stammzertifizierungsserver im Offline-Verfahren“ unter „Ausführen eines RMS-Servers“ in dieser Dokumentationssammlung.

Bei der Clientregistrierung wird ein Client-Lizenzgeberzertifikat erstellt und übermittelt, mit dem ein Autor RMS-geschützte Inhalte über einen Computer veröffentlichen kann, der nicht mit dem Unternehmensnetzwerk verbunden ist. Ein Autor kann jederzeit ein Client-Lizenzgeberzertifikat anfordern. Eine Clientregistrierung ist nicht erforderlich.

Alle Registrierungsanforderungen werden protokolliert.

Dieser Abschnitt behandelt die folgenden Themen:

-   [Registrierung des Stammzertifizierungsservers](https://technet.microsoft.com/f08bc919-f090-4843-b2ce-b40d558012ce)
-   [Unterregistrierung von Lizenzierungsservern](https://technet.microsoft.com/7bc63397-9186-464c-8824-867038adce9b)
-   [RMS-Clientregistrierung](https://technet.microsoft.com/9c1d07bf-7235-4694-8291-ac2e5b221f4a)
-   [RMS-Computeraktivierung](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)
-   [RMS-Kontozertifizierung](https://technet.microsoft.com/c9a385c5-6dbb-47f5-a80f-69718e6f9deb)
