---
TOCTitle: 'RMS-Computeraktivierung'
Title: 'RMS-Computeraktivierung'
ms:assetid: '09a0d631-9860-477f-9d10-df61b3bfe125'
ms:contentKeyID: 18118743
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720182(v=WS.10)'
---

RMS-Computeraktivierung
=======================

Die Computeraktivierung ist Voraussetzung für die Veröffentlichung oder Nutzung von RMS-geschützten Inhalten auf einem Clientcomputer. Bei der Computeraktivierung gibt ein Clientcomputer eine eindeutige Lockbox und ein passendes RMS-Computerzertifikat aus. Die Lockbox enthält den privaten Schlüssel des Computers, das Computerzertifikat den zugehörigen öffentlichen Schlüssel des Computers. Da die Lockbox den privaten Schlüssel des Computers umfasst, bildet sie das wichtigste Sicherheits-Prinzipal für die Ver- und Entschlüsselung. Jeder Benutzer des Computers erhält ein eigenes Computerzertifikat, das im Rahmen der Computeraktivierung erstellt wird.

Die Vorgehensweise bei der Computeraktivierung des RMS-Clients für Service Pack 1 unterscheidet sich erheblich von den Schritten aus Version 1: Der RMS-Client für Service Pack 1 aktiviert sich selbst. Wird der RMS-Client durch einen angemeldeten Benutzer installiert oder wird eine RMS-Funktion durch einen angemeldeten Benutzer erstmalig verwendet, startet der Client automatisch den Aktivierungsvorgang. Hierbei werden mehrere Schlüssel-Sätze mithilfe der Verschlüsselungs-API aus Windows erzeugt. Diese Schlüssel dienen dann als Grundlage für die Ausführung mehrerer Verschlüsselungsschritte, mit denen ein Computerzertifikat erzeugt wird, das den Benutzer, den Computer und den RMS-Client gemeinsam in die RMS-Vertrauenshierarchie einbindet.
