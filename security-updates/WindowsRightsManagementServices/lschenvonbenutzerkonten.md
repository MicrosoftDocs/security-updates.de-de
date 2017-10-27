---
TOCTitle: Löschen von Benutzerkonten
Title: Löschen von Benutzerkonten
ms:assetid: 'bf73b141-d4d1-4807-a773-3aaff58b0db6'
ms:contentKeyID: 18119003
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747653(v=WS.10)'
---

Löschen von Benutzerkonten
==========================

Wenn Sie ein Benutzerkonto aus Active Directory löschen, wird der Eintrag für das Rechtekontozertifikat des Benutzers, der in der Benutzerschlüsseltabelle der Konfigurationsdatenbank des Stammzertifizierungsclusters enthalten ist, nicht automatisch gelöscht. Aus diesem Grund kann die Benutzerschlüsseltabelle unbegrenzt anwachsen, wenn neue Benutzerschlüssel hinzugefügt, aber keine alten Schlüssel gelöscht werden.

Sie können zum Verwalten der Konfigurationsdatenbank eine gespeicherte Prozedur ausführen, die einen Benutzerschlüssel beim Entfernen des zugehörigen Benutzerkontos aus Active Directory jedes Mal mithilfe seiner Sicherheits-ID (Security Identifier oder SID) löscht. Stattdessen können Sie auch in regelmäßigen Abständen ein Skript ausführen, das alle Benutzerschlüssel aus der Konfigurationsdatenbank löscht, wenn es die zugehörigen SIDs nicht mehr in Active Directory gibt. Beachten Sie, dass dies sowohl in SQL Server als auch in Active Directory zu einer hohen Belastung führt.