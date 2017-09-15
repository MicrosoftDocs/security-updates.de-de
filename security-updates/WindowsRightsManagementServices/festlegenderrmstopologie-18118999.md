---
TOCTitle: 'Festlegen der RMS-Topologie'
Title: 'Festlegen der RMS-Topologie'
ms:assetid: 'bf516f7d-b3a1-4e7f-971f-bfab1db41812'
ms:contentKeyID: 18118999
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747651(v=WS.10)'
---

Festlegen der RMS-Topologie
===========================

In der Standardtopologie von RMS werden alle RMS-Dienste für eine Organisation von einem RMS-Stammzertifizierungsserver oder -cluster innerhalb der Active Directory-Struktur zur Verfügung gestellt. Diese RMS-Topologie ist sowohl für große als auch kleine Organisationen geeignet. In einer dezentralisierten RMS-Topologie können spezielle Lizenzierungsserver – so genannte Abteilungslizenzierungsserver – manche oder auch alle der Lizenzierungsdienste für bestimmte Benutzer oder Gruppen innerhalb der Organisation zur Verfügung stellen. Auch wenn der Stammzertifizierungsserver bzw. -cluster weiterhin für alle Kontozertifizierungs- und Aktivierungsproxydienste der gesamten Organisation zuständig ist, ist die dezentrale RMS-Topologie so ausgelegt, dass Organisationen mit sehr speziellen Lizenzierungsbedürfnissen jederzeit die Kontrolle über RMS innerhalb der eigenen Organisation behalten.

Es gibt zwar nur zwei Standardtopologien für RMS, doch ihre Komponenten können sich stark unterscheiden. Wenn Sie die für die Anforderungen Ihrer Organisation erforderlichen Komponenten ermitteln und die geeignete Topologie bei der RMS-Bereitstellung dazu entwerfen möchten, sind folgende Aktionen durchzuführen:

-   Auswerten der Organisationsanforderungen und -ziele
-   Definieren der Verwendungsart der Rechteverwaltung
-   Analysieren der aufgezeichneten Datenverkehrsmuster und Belastungen zum Implementieren einer geeigneten Dienstebene

Das Definieren der Topologie und das Treffen der für ihre Umsetzung erforderlichen Entscheidungen geschieht in einem schrittweisen Prozess, der sich über die gesamte Planungsphase zur Bereitstellung von RMS erstreckt.

Dieses Thema umfasst Folgendes:

-   [Identifizieren von Kernkomponenten](https://technet.microsoft.com/c9ec225b-0e51-42f5-aff6-0aecb62e3b27)
-   [Festlegen der Topologieziele](https://technet.microsoft.com/8275a04d-3e5b-40b0-be9d-2f31b7aeca6b)
-   [Festlegen des Umfangs der RMS-Implementierung](https://technet.microsoft.com/4b5fe1be-643e-47c4-bf9b-50d1e97108fb)
-   [Beurteilen der Skalierungsanforderungen](https://technet.microsoft.com/89f0138c-946d-47d7-a286-041d4d9606a8)
-   [Bereitstellen von Redundanz und Lastenausgleich](https://technet.microsoft.com/162d547c-78a7-4848-b43e-58e481832af2)
-   [Beurteilen der Migrationsanforderungen](https://technet.microsoft.com/cec07f45-dc52-4004-860b-5cc33e5fc209)
-   [Planen der Datenbankserver-Infrastruktur](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
-   [Einplanen der Bereitstellung über mehrere Strukturen](https://technet.microsoft.com/2dfb40b7-95b1-4362-b32e-72867544b705)
-   [Einplanen externer RMS-Benutzer](https://technet.microsoft.com/107e1338-4dcf-4ed5-a49d-e875cc883db1)
-   [Planen einer RMS-Standardtopologie](https://technet.microsoft.com/fec3201e-201f-4faf-910e-fa44132af83d)
-   [Planen einer dezentralisierten RMS-Topologie](https://technet.microsoft.com/8773a1e0-6ac3-41f5-9866-5890cef08d04)
