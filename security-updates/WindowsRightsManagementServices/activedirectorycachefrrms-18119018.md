---
TOCTitle: 'Active Directory-Cache für RMS'
Title: 'Active Directory-Cache für RMS'
ms:assetid: 'c721a2eb-2fe9-4346-b426-3cc169b97265'
ms:contentKeyID: 18119018
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747662(v=WS.10)'
---

Active Directory-Cache für RMS
==============================

Jeder RMS-Stammzertifizierungsserver bzw. -cluster und Lizenzierungsserver hat einen lokalen Active Directory-Cache, der die Ergebnisse der Abfragen zur Gruppenmitgliedschaft im globalen Katalog von Active Directory enthält. Zusätzlich zu dem Cache auf jedem Server gibt es einen gemeinsam verwendeten Cache für jeden Cluster, der in der Datenbank der Verzeichnisdienste gespeichert ist. Diese Caches sollen die Anzahl der an den globalen Katalog gesendeten Abfragen reduzieren sowie die Antwortzeit bei Lizenzierungsanforderungen verkürzen.

Wenn ein Benutzer eine Nutzungslizenz anfordert, muss der antwortende Server überprüfen, ob diesem Benutzer die erforderlichen Rechte in der Veröffentlichungslizenz erteilt wurden. Im einfachsten Fall wird der Benutzer, der eine Lizenz anfordert, in der Veröffentlichungslizenz explizit mit Namen genannt. In vielen Szenarien erteilt der Autor bestimmte Rechte jedoch nicht einzelnen Benutzern, sondern einer Gruppe.

Wenn die Veröffentlichungslizenz den anfordernden Benutzer nicht explizit nennt, sondern stattdessen einer Gruppe Rechte erteilt, muss der Server die Gruppenmitgliedschaften des Benutzers überprüfen und so ermitteln, ob er Mitglied einer Gruppe ist, der Rechte erteilt wurden. Zu diesem Zweck sendet der Server eine LDAP-Abfrage (Lightweight Directory Access Protocol) an den globalen Katalog.

RMS-Server (Rights Management Services oder Dienste für die Rechteverwaltung) speichern die Ergebnisse aller Abfragen zur Gruppenmitgliedschaft sowohl im Active Directory-Cache als auch in der Datenbank der Verzeichnisdienste für den Cluster zwischen. Dann können die Server Informationen zur Gruppenmitgliedschaft aus diesen Caches erhalten, so dass sie weniger Abfragen an den globalen Katalog senden müssen. Standardmäßig wird der nächste Server abgefragt. Sie können jedoch bei der Konfiguration des Registrierungsschlüssels für den globalen Katalog (GC) angeben, welche Server für den globalen Katalog abgefragt werden sollen. Weitere Informationen zu dieser Einstellung finden Sie unter „Ändern der Registrierungseinstellungen für den Verbindungspool“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.

Zur Auswertung der Gruppenmitgliedschaften eines Benutzers überprüft der Server zunächst im eigenen Cache, ob dort bereits Gruppenmitgliedschaftsinformationen für ihn gespeichert sind. Falls dies nicht zutrifft, überprüft der Server die Datenbank der Verzeichnisdienste für den Cluster. Wenn die Gruppenmitgliedschaftsinformationen nicht in dieser Datenbank gespeichert sind, fragt der Server den globalen Katalog ab.

Für Benutzer und Gruppen werden folgende Active Directory-Attribute zwischengespeichert:

-   mail
-   ProxyAddresses (nur SMTP-E-Mail-Adressen)
-   objectSID
-   sidHistory
-   memberOf (GUIDs von Gruppen, denen der Benutzer oder die Gruppe angehört)

Die Einträge im lokalen Active Directory-Cache sind mit einem Zeitstempel versehen. Die Registrierungseinstellungen geben den Gültigkeitszeitraum für Einträge im Cache sowie die Gesamtanzahl der Einträge an, die dort zwischengespeichert werden können. Diese Einstellungen können Auswirkungen auf die Leistung Ihres Servers haben. Weitere Informationen hierzu finden Sie unter „Ändern der Active Directory-Cacheeinstellungen“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.
