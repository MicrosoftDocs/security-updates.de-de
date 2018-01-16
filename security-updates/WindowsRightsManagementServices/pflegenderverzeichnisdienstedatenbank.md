---
TOCTitle: 'Pflegen der Verzeichnisdienste-Datenbank'
Title: 'Pflegen der Verzeichnisdienste-Datenbank'
ms:assetid: '911a62f2-c1d6-4091-99b0-b53211be27a7'
ms:contentKeyID: 18118936
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747680(v=WS.10)'
---

Pflegen der Verzeichnisdienste-Datenbank
========================================

RMS umfasst auch eine Datenbank der Verzeichnisdienste, die sich auf dem Datenbankserver befindet. Sie enthält Daten zu Benutzern, IDs (z. B. E-Mail-Adressen), Sicherheits-IDs (SID), Gruppenzugehörigkeit und Alternativ-IDs. Diese Daten werden aus LDAP-Abfragen ermittelt, die beim globalen Katalog von Active Directory vom RMS-Lizenzierungsdienst eingehen. Nach der Erfassung werden sie in der Datenbank der Verzeichnisdienste zwischengespeichert, was die Antwortzeit des Servers für den Fall verkürzt, dass Benutzer Nutzungslizenzen anfordern.

Da die in dieser Datenbank enthaltenen Daten häufig neu gespeichert und gelöscht werden, besteht eine starke Neigung zur Fragmentierung. Daher sollte die Datenbank in regelmäßigen Abständen – täglich oder wöchentlich – über die Indizes aller Datenbanktabellen von DRMS\_DirectoryServices neu organisiert werden. Dies sorgt für eine Neuerstellung der Indizes, was die Datenfragmentierung beseitigt. Fragmentierte Daten können die Systemleistung beeinträchtigen und sogar zu einem Serverversagen führen, wenn keine Datenpflege durch den Administrator erfolgt.

Wenn SQL Server als Datenbankserver verwendet wird, kann die Reorganisation der Datenbanken mithilfe des Wartungsassistenten oder über ein mit dem SQL Server Agent selbst erstelltes Skript erfolgen.

Wenn festgestellt wird, dass das Transaktionsprotokoll beim Neuerstellen der Indizes der Datenbank eine inakzeptable Größe erreicht, kann dieses Wachstum dadurch eingeschränkt werden, dass von der vollständigen Protokollierung auf zusammenfassende Protokollierung umgestellt wird, bevor die Indizes bearbeitet werden.