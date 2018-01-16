---
TOCTitle: Registrieren des Dienstverbindungspunktes
Title: Registrieren des Dienstverbindungspunktes
ms:assetid: '446d83ec-3224-45e2-9697-625e7db338f3'
ms:contentKeyID: 18118826
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720260(v=WS.10)'
---

Registrieren des Dienstverbindungspunktes
=========================================

Der Dienstverbindungspunkt (Service Connection Point oder SCP) für RMS (Rights Management Services oder Dienste für die Rechteverwaltung) identifiziert den Verbindungs-URL des Dienstes für die RMS-fähigen Clients in einer Organisation. Clients sind ohne einen gültigen SCP nicht in der Lage, RMS zu erkennen, um Nutzungslizenzen, Veröffentlichungslizenzen oder Rechtekontozertifikate anzufordern.

Sie können den SCP-URL des Stammzertifizierungsclusters auf der Seite **RMS-Dienstverbindungspunkt** der Verwaltungswebsite registrieren. Sie können die Registrierung des SCP-URLs auf der Seite **RMS-Dienstverbindungspunkt** auch wieder aufheben, falls Sie ihn aus irgendeinem Grund zurücksetzen müssen. Sie müssen mit einem gültigen Domänenbenutzerkonto, das über ausreichende Berechtigungen zum Erstellen eines Containerobjekts unterhalb des Containers Dienste verfügt, angemeldet sein, um einen SCP-URL zu registrieren oder seine Registrierung aufzuheben.

In Active Directory wird unterhalb des Containers Dienste ein neues Containerobjekt mit dem Titel RightsManagementServices erstellt. Unterhalb dieses Containers wird ein SCP-Objekt mit dem Namen MSRMRootCluster erstellt. Dieses SCP-Objekt besitzt zwei Werte für sein Schlüsselwortattribut:

-   MSRMRootCluster
-   1.0

Hierbei handelt es sich um die Attribute, mit denen Clients und andere Server nach dem Stammcluster-URL in Active Directory suchen. Das Attribut *serviceBindingInformation* des SCP-Objekts enthält den Stammcluster-URL in folgender Form: http://clustername/\_wmcs/Certification.