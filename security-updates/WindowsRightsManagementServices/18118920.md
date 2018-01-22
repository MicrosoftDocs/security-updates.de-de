---
TOCTitle: 'Konfigurieren eines Extranet-URLs'
Title: 'Konfigurieren eines Extranet-URLs'
ms:assetid: '88fec9ff-c96c-4d20-8856-0485e7507572'
ms:contentKeyID: 18118920
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747661(v=WS.10)'
---

Konfigurieren eines Extranet-URLs
=================================

Wenn in der RMS-Installation (Rights Management Services oder Dienste für die Rechteverwaltung) Extranetbenutzer unterstützt werden sollen, können Sie einen Lizenzierungsserver oder Cluster hinzufügen, der für die Extranetnutzung dediziert ist.

Wenn Sie einen Extranetlizenzierungsserver bereitstellen, geben Sie für diesen genau wie für einen beliebigen Server mit RMS einen Cluster-URL an. Der angegebene URL ist normalerweise ein interner URL, auf den Extranetbenutzer nicht zugreifen können. Hierbei handelt es sich um den URL, den RMS zum Suchen nach Diensten verwendet. Dabei muss es sich um einen in der Organisation gültigen URL handeln.

Wenn Sie einen Extranet-Cluster-URL zu einem RMS-Server hinzufügen, der bereits in Verwendung ist, müssen die aktuellen RMS-Clients neue Client-Lizenzgeberzertifikate anfordern, damit zwecks Lizenzierung auf die Extranet-Cluster zugegriffen werden kann.

Weitere Informationen hierzu finden Sie nachstehend unter [So fügen Sie einen Extranet-Cluster-URL hinzu](https://technet.microsoft.com/12c83186-ce9e-4100-bbd1-d87a885331c7).