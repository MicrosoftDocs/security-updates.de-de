---
TOCTitle: 'Veröffentlichung von RMS-Diensten'
Title: 'Veröffentlichung von RMS-Diensten'
ms:assetid: '3cca9325-6bd3-49ad-aa3f-e0693205d3f4'
ms:contentKeyID: 18118822
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720247(v=WS.10)'
---

Veröffentlichung von RMS-Diensten
=================================

Die URLs für Dienste der Windows-Rechteverwaltung (Windows Rights Management Services oder RMS) werden bei der Serverbereitstellung in Active Directory veröffentlicht. Während der Bereitstellung wird Active Directory von RMS-Setup danach abgefragt, ob andere RMS-Server in dieser Gesamtstruktur installiert sind. Wenn keine anderen RMS-Server installiert sind, konfiguriert RMS-Setup den Server als Stammzertifizierungsserver. Bevor Sie RMS verwenden können, müssen Sie den Dienstverbindungspunkt (Service Connection Point oder SCP) in Active Directory registrieren, damit Clients nach dem URL des Stammzertifizierungsservers suchen können. Clients, die Verbindungen mit den auf dem Stammzertifizierungsserver ausgeführten Diensten anfordern, fragen zuerst Active Directory nach diesem URL ab. Weitere Informationen hierzu finden Sie unter „Registrieren des Dienstverbindungspunktes“ im Abschnitt "Betreiben eines RMS-Servers" in dieser Dokumentationssammlung.

| ![](images/Cc720247.note(WS.10).gif)Hinweis                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn die Topologie mehrere Server in einem Stammzertifizierungsserver-Cluster einschließt, verweist der URL auf den Lastenausgleichsserver für den Cluster, den der Administrator während der Bereitstellung angibt. |