---
TOCTitle: Bereitstellen von Redundanz und Lastenausgleich
Title: Bereitstellen von Redundanz und Lastenausgleich
ms:assetid: '162d547c-78a7-4848-b43e-58e481832af2'
ms:contentKeyID: 18118777
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720199(v=WS.10)'
---

Bereitstellen von Redundanz und Lastenausgleich
===============================================

Wenn sichergestellt werden soll, dass Benutzer jederzeit Lizenzen erwerben und Inhalte veröffentlichen können, empfiehlt es sich in jedem Fall, redundante RMS-Server mithilfe von Clustern bereitzustellen. Dies bedeutet, dass ein Stammzertifizierungscluster bereitgestellt wird, der aus mindestens zwei Servern besteht. Wenn Sie darüber hinaus einen separaten Lizenzierungsserver bereitstellen, der die jeweiligen Lizenzierungsanforderungen einer bestimmten Gruppe innerhalb Ihrer Organisation unterstützt, sollten Sie auch den Lizenzierungsserver als Cluster aus mindestens zwei Servern bereitstellen.

Die verschiedenen physischen Server des Stammzertifizierungsclusters oder des Lizenzierungsclusters teilen sich als so genannte „Webfarm“ einen URL, eine virtuelle Adresse. Wenn eine Organisation eine Webfarm verwendet, kann RMS in die jeweils für die Nutzung virtueller Adressen verwendete Praxis integriert werden, beispielsweise in Round-Robin-DNS, den Lastenausgleichsdienst des Netzwerks oder eine dedizierte Hardwarelösung.

Neben dem Lastenausgleich ist eine Nutzung virtueller Adressen auch von Vorteil, wenn sie mit RMS zum Einsatz kommt, da auf diesem Wege die Abhängigkeit von einem einzelnen physischen Server bei der Zertifizierung oder bei Lizenzierungsdiensten vermieden werden kann. Kein Endbenutzercomputer erfordert direkten Zugriff auf einen einzelnen Server im Cluster.