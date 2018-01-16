---
TOCTitle: Ermitteln von Schlüsselverwaltungsanforderungen
Title: Ermitteln von Schlüsselverwaltungsanforderungen
ms:assetid: 'f0e08fb8-bf5e-4278-a09f-daa57696e786'
ms:contentKeyID: 18119099
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747797(v=WS.10)'
---

Ermitteln von Schlüsselverwaltungsanforderungen
===============================================

RMS verwendet kryptografische Schlüssel für den Inhaltsschutz und das Erzwingen von Rechten. Bei kryptografischen Schlüssel handelt es sich um die grundlegenden Informationen, die eine nahtlose und sichere Funktionsweise des Systems ermöglichen. Administratoren müssen die richtige Verwaltung dieser Schlüssel sicherstellen, um Datenverluste, Systemausfälle und Diebstahl zu verhindern.

In der Standardkonfiguration speichert RMS das Serverschlüsselpaar und die zugehörige GUID in einer Tabelle in der Konfigurationsdatenbank. Das Serverschlüsselpaar wird über ein Kennwort verschlüsselt, das während des Bereitstellungsvorgangs von Ihnen bestimmt wird.

Wenn Sie Serverschlüsselpaar und zugehörige GUID weiter absichern möchten, sichern Sie die Konfigurationsdatenbank auf einem Speichermedium – beispielsweise einer CD –, und verwahren Sie solche Medien an einem sicheren Ort, z. B. in einem Safe außerhalb des Firmenstandorts. Der Zeitplan für Sicherungen hängt davon ab, wie häufig Änderungen auf der Verwaltungsebene vorgenommen werden, sowie vom akzeptablen Risikograd hinsichtlich Datenverlust aufgrund von Datenträgerverschleiß oder sonstiger Gefahren für diese Medien. Stellen Sie sicher, dass Sie das Kennwort für den privaten Schlüssel in Erfahrung bringen können, den für die gesicherte Konfigurationsdatenbank erforderlich ist. Ohne das korrekte Kennwort ist es nicht möglich, die Sicherung auf dem RMS-Server wiederherzustellen.

Wenn Sie SQL Server als Datenbankserver verwenden, können Sie mithilfe von SQL Server Enterprise Manager den Wert der verschlüsselten Daten des privaten Schlüssels und die GUID direkt auf eine Diskette oder ein anderes Speichermedium übertragen. Da der private Schlüssel geschützt ist, muss die RMS-Installation über das gleiche RMS-Dienstkonto wie die Sicherung ausgeführt werden, wenn eine Wiederherstellung von sicheren Speicherträgern in eine RMS-Installation durchgeführt werden soll.

Wenn für den Schutz des privaten Serverschlüssels entweder ein Software- oder Hardware-Kryptografieanbieter verwendet wird, müssen Schlüsselcontainer und Schlüssel manuell gesichert werden. In diesem Fall wird die Sicherheit der privaten Schlüssel erhöht, weil sie in der Hardware gespeichert und niemals in der Software offengelegt werden. Daten, die entschlüsselt oder signiert werden müssen, werden an das Hardwaresicherheitsmodul weitergeleitet, entschlüsselt oder signiert und dann ausgegeben.

Sowohl für Hardware- als auch Software-Kryptografieanbieter gibt es individuelle Vorgehensweisen für das zuverlässige Sichern des Schlüssels. Wenn Sie mit diesen Vorgehensweisen nicht vertraut sind, sollten Sie die Dokumentation zum Kryptografieanbieter lesen.