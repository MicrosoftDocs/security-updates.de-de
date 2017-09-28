---
TOCTitle: 'Anhang B: Zu berücksichtigende Schlüsseleinstellungen'
Title: 'Anhang B: Zu berücksichtigende Schlüsseleinstellungen'
ms:assetid: 'ff6d4718-4179-4f5a-a09d-50d75e9f32e6'
ms:contentKeyID: 20075662
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443719(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Anhang B: Zu berücksichtigende Schlüsseleinstellungen

Aktualisiert: 27.12.2005

In diesem Handbuch werden viele Sicherheitsgegenmaßnahmen und Sicherheitseinstellungen erörtert, von denen einige besonders wichtig ist. Die Einstellungen werden in diesem Anhang vorgestellt. In dem entsprechenden Kapiteln finden Sie Informationen zur Funktion und zur Bedeutung der jeweiligen Einstellung.

Welche Einstellungen in dieser Liste enthalten sein sollten ist offen. Die Sicherheitsexperten von Microsoft haben sich eingehend mit diesem Thema befasst. Möglicherweise haben Sie den Eindruck, dass einige Einstellungen fehlen oder dass einige der aufgeführten Einstellungen nicht in der Liste enthalten sein müssten. Jede Organisation verfügt über eine spezielle Umgebung mit einzigartigen Geschäftsanforderungen. Unterschiedliche Meinungen in Bezug auf Sicherheitsrisiken sind deshalb zu erwarten. Mithilfe dieser Liste fällt es Ihnen jedoch leichter, bestimmte Prioritäten zu setzen, die die Absicherung von Computern unter Microsoft® Windows® zum Ziel haben.

Zu wichtigen Gegenmaßnahmen, bei denen es sich nicht um Sicherheitseinstellungen handelt, zählen die Folgenden:

-   Halten Sie Computer auf dem neuesten Stand: mithilfe von Service Packs und Hotfixes mit automatisierten Tools zum Prüfen und Bereitstellen.

-   Installieren und konfigurieren Sie Software für verteilte Firewalls oder organisationseigene IPSec-Richtlinien.

-   Stellen Sie Antivirussoftware bereit, und pflegen Sie diese.

-   Verwenden Sie Antispywaresoftware auf Computern, mit denen im Internet surfen.

-   Benutzen Sie ein Nicht-Administratorkonto für den normalen Betriebsalltag. Ein Konto mit Administratorrechten sollten Sie nur für Aufgaben verwenden, die erhöhte Berechtigungen erfordern.

Zu den in Microsoft Windows verfügbaren Sicherheitseinstellungen zählen u. a. Folgende:

-   Kennwortrichtlinien (in Kapitel 3, „Die Domänenrichtlinie“, beschrieben)

    -   Kennwortchronik erzwingen

    -   Maximales Kennwortalter

    -   Minimale Kennwortlänge

    -   Kennwörter müssen Komplexitätsanforderungen entsprechen

    -   Kennwörter für alle Domänenbenutzer mit umkehrbarer Verschlüsselung speichern

-   Benutzerrechte (siehe Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“)

    -   Auf diesen Computer vom Netzwerk aus zugreifen

    -   Einsetzen als Teil des Betriebssystems

    -   Lokal anmelden zulassen

    -   Anmeldung über Terminaldienste zulassen

-   Sicherheitsoptionen (siehe Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“)

    -   Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken

    -   Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)

    -   Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)

    -   Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)

    -   Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows* *2000 oder höher)

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

-   Zusätzliche Registrierungseinstellungen (siehe Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“)

    -   Sicherer DLL-Suchmodus

[](#mainsection)[Zum Seitenanfanq](#mainsection)

##### In diesem Beitrag

-   [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))
-   [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10))
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))
-   [Kapitel 6: Die Infrastrukturserverrolle](https://technet.microsoft.com/de-de/library/5914ba9b-2fe2-4886-8171-a908521836ec(v=TechNet.10))
-   [Kapitel 7: Die Dateiserverrolle](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))
-   [Kapitel 8: Die Druckserverrolle](https://technet.microsoft.com/de-de/library/a37f44cf-85b3-4ae6-8e32-0cd877c5e9ee(v=TechNet.10))
-   [Kapitel 9: Die Webserverrolle](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))
-   [Kapitel 10: Die IAS-Serverrolle](https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10))
-   [Kapitel 11: Die Zertifikatdienstserverrolle](https://technet.microsoft.com/de-de/library/7488b1dc-eb9b-4f4a-b597-b84d87717b57(v=TechNet.10))
-   [Kapitel 12: Die Bastion-Hostrolle](https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10))
-   [Kapitel 13: Zusammenfassung](https://technet.microsoft.com/de-de/library/4a4cf96c-802d-4aef-9478-da3242f961da(v=TechNet.10))
-   [Anhang A: Sicherheitstools und Formate](https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10))
-   Anhang B: Zu berücksichtigende Schlüsseleinstellungen
-   [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10))
-   [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](https://technet.microsoft.com/de-de/library/2698b276-4c42-4a18-9930-3d69974746f8(v=TechNet.10))
-   [Danksagungen](https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10))

**Download**

[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409)

**Benachrichtigung über Neuerungen**

[Melden Sie sich an, um sich über Updates und neue Versionen zu informieren](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx)

**Feedback**

[Senden Sie uns Ihre Kommentare oder Vorschläge](mailto:secwish@microsoft.com?subject=windows%20server%202003%20security%20guide)

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><div>
<a href="#mainsection"></a><a href="#mainsection">Zum Seitenanfanq</a>
</div></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10)"><img src="images/Dd443719.pageLeft(de-de,TechNet.10).gif" /></a> 16 von 19 <a href="https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10)"><img src="images/Dd443719.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
