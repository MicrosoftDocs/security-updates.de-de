---
TOCTitle: 'Anhang A: Zu berücksichtigende Schlüsseleinstellungen'
Title: 'Anhang A: Zu berücksichtigende Schlüsseleinstellungen'
ms:assetid: '6b4fdfca-4c2c-47f6-8c92-de33a663ea03'
ms:contentKeyID: 20072359
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc163065(v=TechNet.10)'
---

Windows XP-Sicherheitshandbuch
==============================

### Anhang A: Zu berücksichtigende Schlüsseleinstellungen

Aktualisiert: 20.10.2005

In diesem Handbuch werden viele Sicherheitsgegenmaßnahmen und Sicherheitseinstellungen erörtert, von denen einige besonders wichtig ist. Die Einstellungen werden in diesem Anhang vorgestellt. In dem entsprechenden Kapiteln finden Sie Informationen zur Funktion und zur Bedeutung der jeweiligen Einstellung.

Die Einstellungen, die in dieser Liste enthalten sein sollten, könnten ausführlich erörtert werden. Die Sicherheitsexperten von Microsoft haben sich eingehend mit diesem Thema befasst. Möglicherweise haben Sie den Eindruck, dass einige Einstellungen fehlen oder dass einige der aufgeführten Einstellungen nicht in der Liste enthalten sein müssten. Jede Organisation verfügt über eine spezielle Umgebung mit einzigartigen Geschäftsanforderungen. Unterschiedliche Meinungen in Bezug auf Sicherheitsrisiken sind deshalb zu erwarten. Dennoch kann diese Liste Ihnen helfen, Prioritäten für Aufgaben zur Sicherung von Computer mit Microsoft® Windows® zu setzen.

##### Auf dieser Seite

[](#ebaa)[Wichtige Gegenmaßnahmen](#ebaa)
[](#eaaa)[Hauptsicherheitseinstellungen](#eaaa)

### Wichtige Gegenmaßnahmen

Wichtige Gegenmaßnahmen, die nicht mit Sicherheitseinstellungen in Zusammenhang stehen:

-   Halten Sie Computer auf dem neuesten Stand: mithilfe von Service Packs und Hotfixes mit automatisierten Tools zum Prüfen und Bereitstellen.

-   Installieren und konfigurieren Sie Software für verteilte Firewalls oder organisationseigene IPSec-Richtlinien.

-   Stellen Sie Antivirussoftware bereit, und pflegen Sie diese.

-   Stellen Sie Antispyware bereit, und pflegen Sie diese.

-   Verwenden Sie für alltägliche Aufgaben ein Konto ohne Berechtigungen. Ein Konto mit Administratorrechten sollten Sie nur für Aufgaben verwenden, die erhöhte Berechtigungen erfordern.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Hauptsicherheitseinstellungen

Die in Microsoft Windows verfügbaren Hauptsicherheitseinstellungen umfassen:

-   Kennwortrichtlinieneinstellungen, die in Kapitel 2, „Konfigurieren der Domäneninfrastruktur von Active Directory“, behandelt werden:

    -   Kennwortchronik erzwingen

    -   Maximales Kennwortalter

    -   Minimale Kennwortlänge

    -   Kennwörter müssen Komplexitätsanforderungen entsprechen

    -   Kennwörter für alle Domänenbenutzer mit umkehrbarer Verschlüsselung speichern

-   Einstellungen zum Zuweisen von Benutzerrechten, die in Kapitel 3, „Sicherheitseinstellungen für Windows XP-Clients“, erörtert werden:

    -   Auf diesen Computer vom Netzwerk aus zugreifen

    -   Einsetzen als Teil des Betriebssystems

    -   Lokal anmelden zulassen

    -   Anmeldung über Terminaldienste zulassen

-   Einstellungen der Sicherheitsoptionen, die in Kapitel 3, „Sicherheitseinstellungen für Windows XP-Clients“, beschrieben werden:

    -   Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken

    -   Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)

    -   Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)

    -   Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)

    -   Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows 2000 oder höher)

    -   Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen

    -   Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben

    -   Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten und Freigaben nicht erlauben

    -   Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen

    -   Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann

    -   Netzwerkzugriff: Anonymen Zugriff auf Named Pipes und Freigaben einschränken

    -   Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann

    -   Netzwerkzugriff: Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten

    -   Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern

    -   Netzwerksicherheit: LAN Manager-Authentifizierungsebene

-   Zusätzliche Registrierungseinstellungen, die in Kapitel 3, „Sicherheitseinstellungen für Windows XP-Clients“, behandelt werden, insbesondere die folgende Einstellung:

    -   Sicherer DLL-Suchmodus

##### In diesem Beitrag

-   [Überblick](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10))
-   [Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP](https://technet.microsoft.com/de-de/library/4eddb4e4-fd7b-444c-8484-bb8ee220c0e1(v=TechNet.10))
-   [Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory](https://technet.microsoft.com/de-de/library/620c0004-41a8-4d13-9a61-e6d879f9cc65(v=TechNet.10))
-   [Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients](https://technet.microsoft.com/de-de/library/bca34b8d-a1ca-42e4-b743-aa3ca12fd8f9(v=TechNet.10))
-   [Kapitel 4: Administrative Vorlagen für Windows XP](https://technet.microsoft.com/de-de/library/adb79ec2-691f-4a9f-b940-36d2d9807fd7(v=TechNet.10))
-   [Kapitel 5: Schützen eigenständiger Windows XP-Clients](https://technet.microsoft.com/de-de/library/a134d1cb-2ad1-4549-99c8-2a5e0128f2dc(v=TechNet.10))
-   [Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](https://technet.microsoft.com/de-de/library/548c007a-7c26-44fd-8723-563a1f72f21e(v=TechNet.10))
-   [Kapitel 7: Zusammenfassung](https://technet.microsoft.com/de-de/library/8001f9fb-f330-4ab4-a134-ff756091ea0d(v=TechNet.10))
-   [Anhang A: Weitere Anleitungen für Windows XP Service Pack 2](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapa.mspx)
-   Anhang A: Zu berücksichtigende Schlüsseleinstellungen
-   [Anhang B: Testen des Sicherheitshandbuchs für Windows XP](https://technet.microsoft.com/de-de/library/09c716f4-b167-49ec-8122-93e1b8c5f456(v=TechNet.10))
-   [Danksagungen](https://technet.microsoft.com/de-de/library/7e874ad0-7c5a-4f64-9349-760666ab3e61(v=TechNet.10))

##### Download

[![](images/Cc163065.icon_exe(de-de,TechNet.10).gif)Windows XP-Sicherheitshandbuch herunterladen (engl.)](http://go.microsoft.com/fwlink/?linkid=14840&clcid=0x409)

[](#mainsection)[Zum Seitenanfang](#mainsection)
