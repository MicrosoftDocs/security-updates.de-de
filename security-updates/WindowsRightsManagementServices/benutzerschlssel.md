---
TOCTitle: Benutzerschlüssel
Title: Benutzerschlüssel
ms:assetid: '12dad6e2-64e7-4bab-bde7-b72f90f5cb05'
ms:contentKeyID: 18118756
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720202(v=WS.10)'
---

Benutzerschlüssel
=================

Ein Benutzer von RMS verfügt über ein Paar von 1024-Bit-RSA-Schlüsseln. Dieses Schlüsselpaar wird in der RMS-Konfigurationsdatenbank gespeichert; dies stellt sicher, dass jedem Benutzer im gesamten RMS-System nur genau ein Schlüsselpaar zugeordnet ist.

Ein Rechtekontozertifikat enthält den öffentlichen Benutzerschlüssel. Mit diesem Schlüssel wird der Inhaltsschlüssel verschlüsselt, der sich in der Nutzungslizenz befindet. Damit wird gewährleistet, dass nur ein bestimmter Benutzer die RMS-geschützten Inhalte mit dieser Nutzungslizenz einsehen kann.

Dasselbe Rechtekontozertifikat enthält zudem den privaten Benutzerschlüssel, der mit einem öffentlichen Schlüssel des Clientcomputers verschlüsselt wird. Dies stellt sicher, dass ein Rechtekontozertifikat nur von dem Computer aus verwendet werden kann, für den es ausgestellt wurde, zugleich aber jedes Rechtekontozertifikat eines Benutzers ein gleichbleibendes Schlüsselpaar enthält. Der private Benutzerschlüssel ist für das Einsehen RMS-geschützter Inhalte erforderlich.