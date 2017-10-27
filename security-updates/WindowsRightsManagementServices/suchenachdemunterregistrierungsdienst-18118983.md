---
TOCTitle: Suche nach dem Unterregistrierungsdienst
Title: Suche nach dem Unterregistrierungsdienst
ms:assetid: 'b159953a-af38-4a9e-8c87-1aff5fb4e366'
ms:contentKeyID: 18118983
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747641(v=WS.10)'
---

Suche nach dem Unterregistrierungsdienst
========================================

Ein einzelner Lizenzierungsserver bzw. der erste Lizenzierungsserver in einem Cluster muss eine Unterregistrierungsanforderung an den RMS-Stammzertifizierungsserver senden, um ein Server-Lizenzgeberzertifikat zu erhalten. Dazu ruft der Lizenzierungsserver wie folgt den URL des Unterregistrierungsdienstes auf dem Stammzertifizierungsserver ab.

Während der Bereitstellung eines Lizenzierungsservers sendet RMS-Setup eine Anfrage an Active Directory, um den Dienstverbindungspunkt (Service Connection Point oder SCP) des Stammzertifizierungsclusters zu ermitteln. RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwendet den in diesem Dienstverbindungspunkt gespeicherten URL, um nach dem Stammzertifizierungscluster zu suchen, und sendet anschließend eine Anforderung für ein Server-Lizenzgeberzertifikat vom Unterregistrierungsdienst des Stammzertifizierungsservers.

Um die Unterregistrierungsdienstanforderung senden zu können, ruft der Lizenzierungsserver zuerst von Active Directory den URL des virtuellen Verzeichnisses „Certification“ auf dem Stammzertifizierungsserver ab, in dem sich der Unterregistrierungsdienst befindet. Dann fügt er den Pfad des Unterregistrierungsdienstes an.

Beispiel: Der URL für das virtuelle Verzeichnis Certification auf dem Stammzertifizierungsserver wird in Active Directory in folgender Form gespeichert:

http://*Servername*/\_wmcs/Certification

Wenn ein Lizenzierungsserver den Unterregistrierungsdienst anfordert, fügt er den Namen der Dienstdatei wie folgt an den URL an:

http://Servername/\_wmcs/Certification/SubEnrollService.asmx

| ![](images/Cc747641.note(WS.10).gif)Hinweis                              |
|-------------------------------------------------------------------------------------------------------|
| Wenn Sie SSL auf dem RMS-Server aktiviert haben, verwenden diese URLs das HTTPS-Verbindungsprotokoll. |