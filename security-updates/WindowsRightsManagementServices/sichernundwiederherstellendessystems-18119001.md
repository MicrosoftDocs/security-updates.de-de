---
TOCTitle: Sichern und Wiederherstellen des Systems
Title: Sichern und Wiederherstellen des Systems
ms:assetid: 'c11f3ac1-e512-402b-bf13-9ff21f5fe745'
ms:contentKeyID: 18119001
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747745(v=WS.10)'
---

Sichern und Wiederherstellen des Systems
========================================

Wenn Sie Vorkehrungen für eine möglicherweise erforderliche Systemwiederherstellung treffen, sollten Sie sowohl das Versagen des Datenbankservers einerseits und das eines RMS-Servers andererseits berücksichtigen. Wenn es zu einem Ausfall des Datenbankservers kommen sollte, können Sie die Funktionalität eines RMS-Servers oder -Clusters über eine Sicherungskopie der Konfigurationsdatenbank wiederherstellen. Dazu ist weder ein neues Server-Lizenzgeberzertifikat noch ein neuer privater Schlüssel für den RMS-Server erforderlich, denn diese Elemente sind in der Konfigurationsdatenbank gespeichert.

Planen der Sicherung des RMS-Systems
------------------------------------

Neben dem Serverschlüssel werden Benutzerdaten, darunter Informationen zum öffentlichen Schlüssel, in der Konfigurationsdatenbank gespeichert. Sichern Sie die Konfigurationsdatenbank auf Medien, und bewahren Sie diese an einem sicheren Ort auf, um wertvolle Schlüsseldaten zu schützen. Da sich die Konfigurationsdatenbank des Stammzertifizierungsclusters häufig ändert, sollten Sie regelmäßig Sicherungskopien erstellen. Je öfter neue Benutzer zu einer Organisation hinzugefügt werden, desto häufiger sollten Sicherungen durchgeführt werden. Wenn eine Sicherung des Stammzertifizierungsservers erfolgt, sollte sichergestellt werden, dass auch die Tabelle **sysmessages** der Hauptdatenbank in die Sicherung eingeschlossen wird. Wenn die Tabelle keine RMS-spezifischen Nachrichten enthält, ist der Stammzertifizierungsserver nicht funktionsfähig und eine Fehlermeldung wird ausgegeben. Wenn die Tabelle nicht in der Sicherung enthalten ist, kann sie durch Wiederholen des Bereitstellungsvorgangs mithilfe einer bestehenden Datenbank neu erstellt werden.

Die RMS-Protokollierungsdatenbank enthält Protokolle, die möglicherweise hilfreiche Daten zur Fehlerbehebung und statistischen Auswertung beisteuern können, jedoch ist sie für das Funktionieren des RMS-Systems nicht essenziell. Die Verzeichnisdienstdatenbank stellt einen lokalen Cache der Active Directory-Datenbank dar, d. h. sie wird automatisch neu erstellt, wenn das RMS-System wiederhergestellt wird. Wenden Sie sich an den SQL Server-Administrator, um einen Plan zum Sichern der RMS-Datenbanken zu entwickeln.

Wenn Sie die privaten Schlüssel von RMS mithilfe eines Hardwaresicherheitsmoduls schützen, müssen Sie auch dessen Konfiguration sichern. Weitere Informationen zum Sichern und Wiederherstellen des Hardwaresicherheitsmoduls finden Sie in der zugehörigen Dokumentation.

| ![](images/Cc747745.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie die privaten Schlüssel von RMS mit einem softwarebasierten Kryptographiedienstanbieter (Cryptographic Service Provider oder CSP) verschlüsseln, bei dem es sich nicht um den softwarebasierten Standard-Kryptographiedienstanbieter handelt, stellen Sie sicher, dass für diesen organisatorische Schlüsselverwaltungsmethoden (z. B. Sicherungs- und Wiederherstellungsverfahren) installiert wurden, bevor Sie ihn für RMS verwenden. |

Planen der Wiederherstellung eines RMS-Systems
----------------------------------------------

Wenn Sie einen Datenbankserver mithilfe einer Sicherung wiederherstellen, sollten Sie sicherstellen, dass die ausgeführte Version von RMS mit der identisch ist, die bei der Erstellung der Sicherung in Betrieb war. Teilen Sie den Benutzern des RMS-Systems mit, dass sie ein neues Rechtekontozertifikat beantragen müssen, sollten sie erst nach dem Datum der letzten Sicherung mit der Nutzung begonnen haben. Dies hat den Vorteil, dass keine geschützten Daten verloren gehen.

Wenn ein einzelner RMS-Server eines Clusters wiederhergestellt werden soll, muss der Server neu erstellt, dann RMS neu installiert und anschließend der Server mithilfe der bestehenden Datenbank mit dem Cluster verknüpft werden. Dieser Vorgang hat keine Auswirkung auf Benutzer des RMS-Systems, da die Gesamtheit der Clusterserver wie eine Einheit funktioniert.
