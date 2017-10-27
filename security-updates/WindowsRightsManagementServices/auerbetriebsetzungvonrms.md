---
TOCTitle: Außerbetriebsetzung von RMS
Title: Außerbetriebsetzung von RMS
ms:assetid: 'dbcacce7-434d-48a7-a11d-ef9690d78b44'
ms:contentKeyID: 18119040
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747767(v=WS.10)'
---

Außerbetriebsetzung von RMS
===========================

Die Außerbetriebsetzung bezieht sich auf das vollständige Entfernen des RMS-Servers und seiner damit verbundenen Datenbanken aus einer Organisation. Dadurch kann RMS aus der Infrastruktur entfernt werden, ohne dass der Zugriff auf die RMS-geschützten Informationen verloren geht. Im Folgenden werden Gründe dafür angeführt, warum eine Organisation einen RMS-Server möglicherweise aus ihrer Infrastruktur entfernen muss:

-   Migration eines zu Konzeptzwecken erstellten RMS-Servers aus einer Testumgebung in eine Produktionsumgebung
-   Vereinfachung der architektonischen Designs durch Entfernen und Konsolidieren der Lizenzierungsserver in den Stamm-RMS-Cluster
-   Zusammenführen von RMS-Servern – beispielsweise aufgrund einer Unternehmenszusammenführung oder des Ankaufs eines Unternehmens – mittels Integration zweier RMS-Infrastrukturen in eine
-   Entscheidung, RMS nicht länger zum Inhaltsschutz zu verwenden

Da ein aktiver RMS-Server mit einem Datenbankserver und Active Directory ausgestattet ist und umfassende, durch einen Schlüssel geschützte Inhalte im RMS-Server zurückbehält, sind für das Entfernen von RMS aus der Organisation mehr Schritte erforderlich, als lediglich das Programm vom Server zu löschen. In diesem Abschnitt werden die Schritte zur gegebenenfalls erforderlichen Außerbetriebsetzung des RMS-Server erläutert.

Dieser Abschnitt behandelt die folgenden Themen:

-   [Der Außerbetriebsetzungsvorgang](https://technet.microsoft.com/57bd9949-9433-437b-93ed-ffb2dff9992e)
-   [Aktivieren des Außerbetriebsetzungsdienstes](https://technet.microsoft.com/45226e85-b50d-41cc-aca7-0f603f8509d5)
-   [Einrichten der Berechtigungen für das virtuelle Verzeichnis](https://technet.microsoft.com/45112111-9608-45b1-9a86-7b313d0a1579)
-   [Entfernen des RMS-Schutzes für Inhalte](https://technet.microsoft.com/c30361e3-50d2-4474-a87d-d38de502cf9e)
-   [Entfernen des Webdienstes (Beenden der Bereitstellung von RMS)](https://technet.microsoft.com/68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e)
-   [Entfernen der RMS-Programmdateien](https://technet.microsoft.com/d1dc8a8b-f8de-487f-87b4-2174d449f0bc)
-   [Alternativen zur Außerbetriebsetzung von RMS](https://technet.microsoft.com/4d32f35e-997d-4d10-ab66-efe217e853f7)