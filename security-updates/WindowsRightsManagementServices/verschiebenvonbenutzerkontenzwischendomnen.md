---
TOCTitle: Verschieben von Benutzerkonten zwischen Domänen
Title: Verschieben von Benutzerkonten zwischen Domänen
ms:assetid: '0010b0ea-07c0-41c9-81f7-5881343d1d55'
ms:contentKeyID: 18118737
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720179(v=WS.10)'
---

Verschieben von Benutzerkonten zwischen Domänen
===============================================

Wenn Sie einen Stammzertifizierungsserver in einer Organisation einrichten und bereitstellen, wird dieser in Active Directory in einer Einstellung für die Gesamtstruktur als RMS-Dienstanbieter registriert. Pro Active Directory-Gesamtstruktur darf nur ein Stammzertifizierungscluster vorhanden sein.

Wenn Sie ein Benutzerkonto von einer Domäne zu einer anderen Domäne in der gleichen Gesamtstruktur verschieben, wird im Allgemeinen eine neue SID für das Benutzerkonto in der neuen Domäne erstellt. Wenn ein Benutzer dann versucht, ein neues Rechtekontozertifikat vom Server zu erwerben, wird der Benutzer für den Server aufgrund der neuen SID als neuer Benutzer angezeigt. Der Server generiert neue Schlüssel für den Benutzer und stellt das neue Rechtekontozertifikat mithilfe der ursprünglichen E-Mail-Adresse des Benutzers aus. Wenn der Benutzer versucht, das neue Rechtekontozertifikat mit einer vorhandenen Lizenz zu verwenden, stimmen SID und Schlüssel nicht überein. Der Benutzer muss deshalb eine neue Lizenz erwerben. Dies ist auch beim Verschieben des Benutzerkontos in eine Domäne in einer anderen Gesamtstruktur der Fall.