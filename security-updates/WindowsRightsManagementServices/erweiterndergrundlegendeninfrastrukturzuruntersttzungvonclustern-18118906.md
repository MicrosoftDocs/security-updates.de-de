---
TOCTitle: Erweitern der grundlegenden Infrastruktur zur Unterstützung von Clustern
Title: Erweitern der grundlegenden Infrastruktur zur Unterstützung von Clustern
ms:assetid: '78f0f2f0-a075-409c-9f46-26eb62d1d05b'
ms:contentKeyID: 18118906
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747567(v=WS.10)'
---

Erweitern der grundlegenden Infrastruktur zur Unterstützung von Clustern
========================================================================

Stellen Sie beim Implementieren von Clustern für größere Bereitstellungen sicher, dass die Konfiguration der Infrastruktur Clusteranforderungen unterstützt. Die folgenden Elemente sollten in den Bereitstellungsplänen enthalten sein.

DNS-Registrierung
-----------------

Stellen Sie sicher, dass alle DNS-Registrierungen zur Darstellung der virtuellen IP-Adresse auf dem Extranet auch den Pfad zum Intranet darstellen.

Wird die DNS-Registrierung für das Intranet unterlassen, schlagen interne Clientlizenzanforderungen fehl. Wenn die DNS-Einstellungen nicht verändert werden können, ist es möglich, die Hosttabelle aller Server des Clusters zu verändern. Auf diesem Wege kann der URL des Clusters der entsprechenden virtuellen IP-Adresse zugeordnet werden. Die DNS-Registrierung muss vor der Bereitstellung des Dienstes erfolgen. Wenn Sie den Dienst schon bereitgestellt haben, müssen Sie RMS vom Server entfernen, und danach den Bereitstellungsvorgang wiederholen.

Lastenausgleich
---------------

Richten Sie die erforderliche Hard- und Software so ein, dass die Bereitstellung von Lastenausgleichsservern, der Netzwerklastenausgleichsdienst bzw. der Hardwarelastenausgleich erforderlichenfalls zur Verteilung der Anforderungen über den Cluster hinweg ermöglicht werden.