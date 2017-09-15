---
TOCTitle: 'Entfernen des Webdienstes (Beenden der Bereitstellung von RMS)'
Title: 'Entfernen des Webdienstes (Beenden der Bereitstellung von RMS)'
ms:assetid: '68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e'
ms:contentKeyID: 18118863
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747602(v=WS.10)'
---

Entfernen des Webdienstes (Beenden der Bereitstellung von RMS)
==============================================================

Nachdem der RMS-Server außer Betrieb gesetzt und der RMS-Schutz entfernt wurde, kann der Webdienst anhand folgender Schritte entfernt werden:

-   Klicken Sie auf der Seite **Globale Verwaltung** auf **RMS von dieser Website entfernen**.

Der nächste Schritt hängt von dem zu entfernenden Servertyp ab. RMS wird allerdings in allen Fällen vom IIS entfernt.

-   Ist der Server Teil eines Clusters, sind keine zusätzlichen Schritte erforderlich, es sei denn, es handelt sich um den letzten Server des Clusters.
-   Handelt es sich beim Server nur um einen Lizenzierungsserver, müssen Sie die Datenbank der Verzeichnisdienste entfernen, die Konfigurations- und Protokollierungsdatenbank jedoch beibehalten, da diese von dem weiterhin in Betrieb befindlichen Zertifizierungsserver verwendet werden.
-   Wenn der Server der letzte RMS-Server der Organisation ist, speichern Sie die Konfigurations- und Protokollierungsdatenbank, entfernen Sie jedoch den Dienstverbindungspunkt (Service Connection Point oder SCP) im Active Directory.
