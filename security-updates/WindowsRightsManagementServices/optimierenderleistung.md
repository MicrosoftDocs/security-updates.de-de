---
TOCTitle: Optimieren der Leistung
Title: Optimieren der Leistung
ms:assetid: '24dc9ca4-652b-41a6-9a99-95fdeca9120b'
ms:contentKeyID: 18118785
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720220(v=WS.10)'
---

Optimieren der Leistung
=======================

Die Themen in diesem Abschnitt enthalten Informationen zum Optimieren der Leistung einer RMS-Bereitstellung.

Optimieren der Leistung der Verzeichnisdienste
----------------------------------------------

Sie können die im Lieferumfang von RMS (Rights Management Services oder Dienste für die Rechteverwaltung) enthaltenen Leistungsindikatoren für Verzeichnisdienste überwachen. Falls nötig, können Sie die Leistung durch Ändern der Registrierungseinstellungen optimieren, die die Attribute des Active Directory-Caches steuern.

Die Registrierungseinstellungen steuern die folgenden Attribute des Active Directory-Caches:

-   Die maximale Anzahl von zwischenzuspeichernden Prinzipalen
-   Den Gültigkeitszeitraum von Informationen, die für Prinzipale zwischengespeichert werden
-   Die maximale Anzahl von zwischenzuspeichernden Gruppen
-   Den Gültigkeitszeitraum von Informationen, die für Gruppen zwischengespeichert werden
-   Die maximale Anzahl von Gruppenmitgliedschaftseinträgen
-   Den Gültigkeitszeitraum von Informationen, die für die Gruppenmitgliedschaft zwischengespeichert werden

Im Allgemeinen gilt, je länger der Gültigkeitszeitraum für die zwischengespeicherten Informationen ist bzw. je mehr Einträge im Cache enthalten sind, desto schneller kann RMS auf Anforderungen antworten, für die das Abrufen von Verzeichnisdienstinformationen erforderlich ist. Wenn die Informationen im Active Directory-Cache gespeichert sind, ist kein Round-Trip zu Active Directory zum Durchführen einer Suche erforderlich. Damit wird die Antwortzeit für die Anforderung verkürzt.

Beim Speichern weiterer Informationen im Active Directory-Cache wird ein Kompromiss eingegangen, denn es sind mehr Systemspeicherressourcen erforderlich. Sie müssen beim Konfigurieren der Registrierungseinstellungen außerdem die Wahrscheinlichkeit berücksichtigen, dass einige vom Active Directory-Cache zurückgegebenen Ergebnisse möglicherweise ungültig sind, je länger der für ein bestimmtes Element angegebene Gültigkeitszeitraum ist. Dies kann vorkommen, wenn Informationen in Active Directory geändert wurden, die Änderung aber noch nicht im Active Directory-Cache widergespiegelt wird. Bei häufigen Änderungen an Active Directory sollten Sie einen kürzeren Gültigkeitszeitraum für zwischengespeicherte Informationen angeben. Dieser Gültigkeitszeitraum spiegelt diese Häufigkeit wider.

Die Leistungsindikatoren für Verzeichnisdienste werden nachstehend unter „[RMS: „DirectoryServices“ (Leistungsindikatoren)](https://technet.microsoft.com/37afea1d-f320-4040-96d8-57c0b45e6d46)” erläutert. Weitere Informationen zum Verwenden dieser Leistungsindikatoren finden Sie oben unter „[Verwenden von Leistungsindikatoren](https://technet.microsoft.com/096c3b17-c082-46c4-939c-4373af0c9dec)“ weiter oben in diesem Thema. Die zu überwachenden Indikatoren sind die „Treffer“ („Hits“), nicht die „Fehler“ („Misses“). RMS muss für jeden Fehler eine Active Directory-Suche durchführen.

Detaillierte Informationen zu den Registrierungseinstellungen und Anweisungen zu deren Änderung finden Sie nachstehend unter „[Ändern der Active Directory-Cacheeinstellungen](https://technet.microsoft.com/8789a7a5-2065-4fae-9104-e0a70f1f2fb6)“.

Optimieren der Einstellungen für den Active Directory-Verbindungspool
---------------------------------------------------------------------

Zur Verbesserung der Systemleistung können Sie Registrierungsschlüssel, die die Einstellungen für den Active Directory-LDAP-Verbindungspool steuern, hinzufügen und ändern. Das Konfigurieren der Registrierungsschlüssel ist nachstehend unter „[Ändern der Registrierungseinstellungen für den Verbindungspool](https://technet.microsoft.com/c61d91db-a1ad-4ca5-a492-015da629afbc)“ beschrieben.

RMS soll LDAP-Verbindungen optimieren. Es stellt für jeden globalen Katalog von Active Directory eine Verbindung her. Dabei kann jede Verbindung mehrere Threads bedienen. Zum Bereitstellen von Stabilität verwaltet es einen Pool von Verbindungen, die Anforderungen bedienen. RMS verwendet einen Algorithmus zum Verteilen von Anforderungen, um zu verhindern, dass ein einzelner globaler Katalog einer zu hohen Belastung ausgesetzt wird. Dabei wird unter den globalen Katalogen, die in der Liste der abzufragenden globalen Kataloge enthalten sind, ein Lastenausgleich vorgenommen. RMS verarbeitet außerdem LDAP-Fehler und leitet Anforderungen ggf. an andere globale Kataloge weiter.

Das Programm erstellt mithilfe des Algorithmus für die Topologiesuche eine Liste der abzufragenden globalen Kataloge. Sie können die Mindest- und Höchstanzahl der verfügbaren globalen Kataloge angeben, die von der Topologiesuche gefunden werden müssen, bevor die RMS-Dienste starten können. Die Topologiesuche sucht zuerst die globalen Kataloge am aktuellen Standort. Sind weitere globale Kataloge erforderlich, sucht es an anderen Standorten nach diesen. Zudem geben Sie die maximale Anzahl von Verbindungen an, deren Verfügbarkeit enden kann, bevor RMS keine weiteren Anforderungen mehr akzeptiert. Wenn einer oder mehrere Kataloge in der Abfrageliste später nicht mehr zur Verfügung stehen, sucht die Topologiesuche nach globalen Ersatzkatalogen, die zur Abfrageliste hinzugefügt werden können.

Sie können die von RMS zu verwendenden globalen Kataloge stattdessen aber auch auflisten. In diesem Fall sucht die Topologiesuche nicht nach globalen Katalogen, um diese zur Abfrageliste hinzuzufügen.

Darüber hinaus können Sie Einstellungen für die Vorgehensweise von RMS beim Durchführen des Lastenausgleichs unter den globalen Katalogen konfigurieren. Sie können die relative Bedeutung der folgenden Überlegungen bei der Entscheidung angeben, ob eine bestimmte Anforderung an einen bestimmten globalen Katalog gesendet wird:

-   **Round robin (WtRoundRobin)**. Dieser Parameter gibt die relative Bedeutung des Lastenausgleichs an, bei dem die Round-Robin-Logik verwendet wird. Die Standardeinstellung ist 1. Diese Überlegung ist für den Server beim Auswählen des globalen Katalogs also am wenigsten wichtig.
-   **Thread count during connection (WtThreadCount)**. Dieser Parameter gibt die relative Bedeutung der Anzahl von Threads an, die einer Verbindung zugeordnet sind. Die Standardeinstellung ist 100. Es ist also 100-mal wichtiger, dass die Threadanzahl eines globalen Katalogs für eine auszuwählende Verbindung niedrig ist, als einen Lastenausgleich mit der Round-Robin-Logik durchzuführen.
-   **Slow connection (WtSlow)**. Dieser Parameter gibt die relative Bedeutung einer langsamen Verbindung an. Die Standardeinstellung ist 1000. Es ist also 10-mal wichtiger, dass eine für einen globalen Katalog auszuwählende Verbindung nicht langsam ist, als dass die Threadanzahl niedrig ist.