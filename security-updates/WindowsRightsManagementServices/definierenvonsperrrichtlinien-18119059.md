---
TOCTitle: Definieren von Sperrrichtlinien
Title: Definieren von Sperrrichtlinien
ms:assetid: 'e2fffe9f-def7-439b-a8aa-43f8a065813d'
ms:contentKeyID: 18119059
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747782(v=WS.10)'
---

Definieren von Sperrrichtlinien
===============================

Gehen Sie beim Definieren und Planen von Sperrrichtlinien für eine Organisation mit besonderer Sorgfalt vor. Durch das Implementieren der Sperrung wird zwar einerseits eine höhere Sicherheit der geschützten Inhalte bereitgestellt, andererseits kann sich die Sperrung aber nachteilig auf das Abrufen von Inhalten durch Benutzer auswirken. Sperrrichtlinien für die Bereitstellung von RMS (Rights Management Services oder Dienste für die Rechteverwaltung) können auf der Verwaltungswebsite definiert werden.

Sperrung durch Drittanbieter
----------------------------

Da das Server-Lizenzgeberzertifikat des Stammzertifizierungsservers einer RMS-Bereitstellung vom Microsoft-Registrierungsdienst ausgestellt wird, kann Microsoft das Server-Lizenzgeberzertifikat sperren. Microsoft sperrt ein Server-Lizenzgeberzertifikat jedoch nur auf Anordnung eines Gerichts.

Zusätzlich zum Microsoft-Registrierungsdienst können Sie einen Drittanbieter angeben, der das Server-Lizenzgeberzertifikat des Servers mit RMS sperrt. Bei diesem Drittanbieter kann es sich entweder um eine externe Entität oder ein öffentliches oder privates Schlüsselpaar handeln, das der Administrator im Namen der Organisation generiert. Der private Schlüssel des angegebenen Drittanbieters kann eine Sperrliste signieren, die das Server-Lizenzgeberzertifikat sperrt. Dieser Drittanbieter wird bei der Bereitstellung von RMS durch seinen öffentlichen Schlüssel angegeben. Die Vorlagen für Benutzerrechterichtlinien des Servers können ebenfalls so konfiguriert werden, dass Drittanbieter Inhalte, Anwendungsmanifeste, Lizenzen und Zertifikate sperren können, die von der RMS-Installation ausgestellt wurden. Weitere Informationen hierzu finden Sie nachtstehend unter [Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).

| ![](images/Cc747782.Important(WS.10).gif)Wichtig                                                                                                               |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie ein eigenes Schlüsselpaar zum Sperren des Server-Lizenzgeberzertifikats des Stammzertifizierungsservers generieren, müssen Sie dieses unbedingt an einem sicheren Ort aufbewahren. |

Durch Sperren eines Server-Lizenzgeberzertifikats wird eine wichtige Entscheidung getroffen, da alle von der RMS-Installation ausgestellten Zertifikate und Lizenzen beim Sperren dieses Zertifikats gesperrt werden. Weitere Informationen zum Sperren von Server-Lizenzgeberzertifikaten finden Sie nachstehend unter [Sperren von Server-Lizenzgeberzertifikaten](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616).

Überlegungen zum Inkrafttreten von Sperrlisten
----------------------------------------------

Sobald die Sperrung für einen bestimmten Teil der geschützten Inhalte erforderlich ist, werden alle auf dem Clientcomputer registrierten Sperrlisten verwendet. Diese werden wirksam, wenn eine bestimmte Bedingung erfüllt wird. Gehen Sie daher beim Implementieren einer Sperrung umsichtig vor, denn dieser Vorgang hat ein Registrieren von Sperrlisten auf Clientcomputern und möglicherweise eine weitreichendere Anwendung dieser Liste als beabsichtigt zur Folge. Weitere Informationen zum Konfigurieren dieser Option finden Sie nachstehend unter [Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).

Kompromiss zwischen Sicherheit und Verwendbarkeit
-------------------------------------------------

Wenn Sie eine Sperrrichtlinie in einer Vorlage für Benutzerrechterichtlinien angeben, wägen Sie den Bedarf an höherer Sicherheit für Dokumente im Vergleich zu der Möglichkeit ab, dass beim Abrufen von Inhalten Probleme für Benutzer auftreten. Dies wird im folgenden Beispiel beschrieben.

Beim Einrichten einer Sperrliste in einer Vorlage für Benutzerrechterichtlinien geben Sie auch ein Aktualisierungsintervall für die Sperrliste an. Damit ein Benutzer Inhalte abrufen kann, die mithilfe dieser Vorlage für Benutzerrechterichtlinien veröffentlicht wurden, muss auf dem Computer des Benutzers eine Sperrliste vorhanden sein, die nicht älter als das angegebene Aktualisierungsintervall sein darf. Beträgt das Aktualisierungsintervall beispielsweise 10, muss die Sperrliste innerhalb der letzten 10 Tage erstellt worden sein. Wenn es auf dem Clientcomputer keine Sperrliste gibt bzw. das Erstellungsdatum der Liste älter als das Aktualisierungsintervall ist, erhält die RMS-fähige Anwendung die letzte Sperrliste von dem in der Nutzungslizenz angegebenen Speicherort. Allerdings kann ein Benutzer, der nicht mit dem Netzwerk verbunden ist, die aktuelle Sperrliste nicht beziehen und somit die Inhalte nicht abrufen.

Die folgenden Vorschläge sollen Ihnen helfen, dieses Problem zu umgehen:

-   Gehen Sie beim Angeben des Aktualisierungsintervalls einer Sperrliste vorsichtig vor, und stellen Sie sicher, dass Benutzer immer problemlos auf eine aktuelle Sperrliste zugreifen können.
-   Speichern Sie Sperrlisten unter URLs, auf die sowohl im Firmennetzwerk als auch von außerhalb des Firmennetzwerks zugegriffen werden kann.
-   Verteilen Sie aktualisierte Exemplare von Sperrlisten in regelmäßigen Abständen, z. B. jede Nacht, an alle Clientcomputer, mithilfe von Microsoft® Systems Management Server (SMS) oder einem ähnlichen Verfahren.
-   Verwenden Sie Sperrlisten nur für die vertraulichsten Dokumenttypen.