---
TOCTitle: 'Ausschließen von Lockbox-Versionen'
Title: 'Ausschließen von Lockbox-Versionen'
ms:assetid: 'e287f026-aab2-43ab-93bc-48087da82f36'
ms:contentKeyID: 18119047
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747700(v=WS.10)'
---

Ausschließen von Lockbox-Versionen
==================================

Durch Verwenden der Lockbox-Version, die dem Client zugeordnet wurde, um frühere Versionen der RMS-Clientsoftware auszuschließen, können Sie sicherstellen, dass die Clients mindestens eine bestimmte Version der RMS-Clientsoftware verwenden. Wenn Sie dieses Feature aktivieren, geben Sie die letzte minimale Lockbox-Version an, die vom Microsoft-Aktivierungsdienst signiert wurde. Sie können den Lockbox-Ausschluss dann auf der Verwaltungswebsite für jeden Cluster aktivieren, für den dieser gelten soll. Alle Zertifizierungs- und Lizenzierungsanforderungen werden überprüft, um sicherzustellen, dass die Lockbox die Kriterien der minimalen Version erfüllt.

Wenn Sie den Ausschluss auf der Basis der Lockbox-Version aktiviert haben, können Clients, die eine frühere Version der Lockbox-Software verwenden, keine Kontozertifikate erwerben oder Nutzungslizenzen verwenden, weil ihre Anforderungen abgelehnt werden. Auf diesen Clients muss eine neue Version der RMS-Clientsoftware installiert werden, um eine neue Lockbox zu erhalten, die die aktuelle Version der Software verwendet.

Der RMS-Client für Service Pack 1 (SP1) verwendet Lockbox-Version 5.0.0.0 oder höher. Durch Einrichten des Lockbox-Ausschlusses auf diese minimale Version erzwingen Sie eine Aktualisierung der RMS-Clients in Ihrer Organisation auf den RMS-Client für SP1 zum Abrufen RMS-geschützter Inhalte.

Wenn für Benutzer, die über eine ausgeschlossene Lockbox verfügen, zuvor Lizenzen für Inhalte ausgestellt wurden, können sie diese auch weiterhin abrufen, ohne eine neue Lockbox zu erwerben.
