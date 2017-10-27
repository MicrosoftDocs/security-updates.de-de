---
TOCTitle: Beurteilen der Migrationsanforderungen
Title: Beurteilen der Migrationsanforderungen
ms:assetid: 'cec07f45-dc52-4004-860b-5cc33e5fc209'
ms:contentKeyID: 18119019
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747759(v=WS.10)'
---

Beurteilen der Migrationsanforderungen
======================================

Organisationen, die RMS einsetzen, müssen einen Migrationsplan erstellen, der die Serverausfallzeit minimiert, sodass Serververwaltung und Aktualisierungsszenarios umgesetzt werden können, ohne dass der Benutzerzugriff auf RMS-geschützte Inhalte beeinträchtigt wird. Da bestehende Konfigurations- und Protokollierungsdatenbanken von RMS verwendet werden können, sollte die Migration von RMS zwischen Servern nur minimale Auswirkungen auf die Organisation haben, wenn die richtige Vorgehensweise gewählt wurde. Für das Migrationsszenario wird davon ausgegangen, dass vorhandene Datenbanken verwendet werden sollen; anderenfalls käme die Migration einer Neuinstallation gleich.

Wenn der zu ersetzende RMS-Server ein Hardwaresicherheitsmodul (HSM) – beispielsweise nCipher – verwendet, müssen Sie die HSM-Konfiguration auf den neuen Server übertragen, bevor Sie RMS auf diesem installieren und bereitstellen. Anleitungen hierzu finden Sie in der Dokumentation zu Ihrem Hardwaresicherheitsmodul.

Folgendes ist vor der Migration zu beachten:

-   Stellen Sie sicher, dass die Datenbanken verfügbar sind.
-   Entscheiden Sie, welche Computer in der neuen Installation verwendet werden.

Führen Sie die folgenden Schritte aus, um eine RMS-Installation zu migrieren:

1.  Sichern Sie alle Komponenten vor dem Beginn der Migration. Dies bedeutet auch eine Sicherung der Datenbanken, privaten Schlüssel und des Systemstatus.
2.  Stellen Sie sicher, dass die Datenbanken der vorherigen RMS-Installation auf dem Datenbankserver vorliegen, der für die neue Bereitstellung verwendet werden soll.
3.  Installieren Sie RMS, und stellen Sie es auf den geeigneten Servern bereit. Geben Sie den Speicherort der Datenbanken an.

Ein typisches Szenario, das eine Migration des RMS-Servers beinhaltet, wäre der Wechsel einer Testbereitstellung von RMS hin zur vollständigen Implementierung. Weitere Informationen für das Nutzungsszenario finden Sie in dieser Dokumentationssammlung im Abschnitt „Bereitstellen von RMS“ unter „Migration von einer Testbereitstellung zu einer vollständigen Implementierung“.