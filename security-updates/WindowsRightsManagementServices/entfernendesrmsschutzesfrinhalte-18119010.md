---
TOCTitle: 'Entfernen des RMS-Schutzes für Inhalte'
Title: 'Entfernen des RMS-Schutzes für Inhalte'
ms:assetid: 'c30361e3-50d2-4474-a87d-d38de502cf9e'
ms:contentKeyID: 18119010
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747658(v=WS.10)'
---

Entfernen des RMS-Schutzes für Inhalte
======================================

Bestimmen Sie im Voraus, welche Dateien von wem und wann wiederhergestellt werden sollen, so dass wichtige Informationen nach Abschluss des Außerbetriebsetzungsvorgangs erhalten bleiben. Wurde der RMS-Schutz von allen erforderlichen RMS-geschützten Dateien entfernt, kann der Server aus der Infrastruktur entfernt werden.

Das Entfernen des RMS-Schutzes für Inhalte geht folgendermaßen vor sich:

1.  Der Benutzer sollte alle bestehenden Nutzungslizenzen vom Computer löschen. Dadurch wird sichergestellt, dass der RMS-Client eine Lizenz zum Öffnen des Inhalts vom Server anfordern muss. Nutzungslizenzen werden im Ordner %USERPROFILE%\\Lokale Einstellungen\\Anwendungsdaten\\Microsoft\\DRM auf dem Clientcomputer gespeichert und verfügen über das Präfix EUL für den Dateinamen.
2.  Ein Benutzer mit Zugriff auf den Außerbetriebsetzungsserver versucht eine RMS-geschützte Datei zu öffnen.
3.  Die Anwendung stellt eine Verbindung mit dem Außerbetriebsetzungsserver her und erhält den Inhaltsschlüssel.
4.  Der Inhalt wird verschlüsselt und kann bearbeitet, gespeichert, weitergeleitet oder gedruckt werden.
5.  Der Benutzer speichert den Inhalt ohne RMS-Schutz. Alle Benutzer können nun den Inhalt öffnen, ohne eine Verbindung mit dem RMS-Server herzustellen.
