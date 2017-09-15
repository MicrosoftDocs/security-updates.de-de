---
TOCTitle: 'RMS – Häufig gestellte Fragen: Zertifikate, Schlüssel und Verschlüsselung'
Title: 'RMS – Häufig gestellte Fragen: Zertifikate, Schlüssel und Verschlüsselung'
ms:assetid: 'ad8cc088-1dea-44c2-be68-9091129f0f12'
ms:contentKeyID: 18118994
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747725(v=WS.10)'
---

RMS – Häufig gestellte Fragen: Zertifikate, Schlüssel und Verschlüsselung
=========================================================================

RMS-Zertifikate, -Schlüssel und -Verschlüsselung – Häufig gestellte Fragen
--------------------------------------------------------------------------

-   [Welche Verschlüsselungsalgorithmen werden in RMS verwendet?](#bkmk_10)
-   [Arbeitet RMS mit FIPS-Verschlüsselung?](#bkmk_11)
-   [Werden Nutzungslizenzen für Veröffentlichungslizenzen oder Vorlagen, die Berechtigungen nicht für einzelne Benutzer, sondern für Verteilerlisten ausstellen, anders gehandhabt, damit die Mitglieder dynamisch überprüft werden können?](#bkmk_12)
-   [Bei Verwendung von RMS im Kioskmodus wird ein temporäres Rechtekontozertifikat (Rights Account Certificate, RAC) ausgestellt. Wie unterscheidet sich ein temporäres Rechtekontozertifikat von einem normalen Rechtekontozertifikat? Wie stellt RMS fest, dass es im Kioskmodus verwendet wird?](#bkmk_13)
-   [Wann wird ein temporäres Rechtekontozertifikat verwendet?](#bkmk_14)
-   [Stellt RMS X.509v3-Zertifikate aus?](#bkmk_15)
-   [Wo werden XrML-Zertifikate gespeichert?](#bkmk_16)
-   [Wo wird das Computerschlüsselpaar (privat/öffentlich) gespeichert?](#bkmk_17)
-   [Wo wird das Clientschlüsselpaar (privat/öffentlich) gespeichert?](#bkmk_18)
-   [AES (Advanced Encryption Standard, erweiterter Verschlüsselungsstandard) ist ein symmetrischer Algorithmus. Wie werden die Schlüssel zwischen dem Server und dem Benutzer auf sichere Weise ausgetauscht?](#bkmk_19)

<span id="BKMK_10"></span>
#### Welche Verschlüsselungsalgorithmen werden in RMS verwendet?

In RMS werden 2048-Bit-RSA-Schlüssel für den RMS-Server und 1024-Bit-RSA-Schlüssel für die Computer- und Clientschlüsselpaare verwendet.

<span id="BKMK_11"></span>
#### Arbeitet RMS mit FIPS-Verschlüsselung?

In RMS mit Service Pack 1 und später wird für die von RMS-Clientanwendungen erstellten Lockboxes die FIPS-zertifizierte AES-Verschlüsselung verwendet, wenn der Client auf einem Computer mit Windows XP oder Windows Server 2003 installiert ist. Ist der RMS-Client dagegen auf einem Computer mit Windows 2000 installiert, ist keine FIPS-zertifizierte AES-Bibliothek installiert, sodass diese Lockboxes nicht FIPS-konform sind.

<span id="BKMK_12"></span>
#### Werden Nutzungslizenzen für Veröffentlichungslizenzen oder Vorlagen, die Berechtigungen nicht für einzelne Benutzer, sondern für Verteilerlisten ausstellen, anders gehandhabt, damit die Mitglieder dynamisch überprüft werden können?

Nutzungslizenzen werden immer für einzelne Benutzer ausgestellt. Wenn in einer Veröffentlichungslizenz oder einer Vorlage eine Gruppe angegeben ist, überprüft RMS die Gruppenmitgliedschaft zum Zeitpunkt der Nutzungslizenzerteilung. Wenn der Benutzer, der die Lizenz anfordert, ein Mitglied der angegebenen Gruppe ist, wird die Nutzungslizenz für die Benutzer-ID ausgestellt.

<span id="BKMK_13"></span>
#### Bei Verwendung von RMS im Kioskmodus wird ein temporäres Rechtekontozertifikat (Rights Account Certificate, RAC) ausgestellt. Wie unterscheidet sich ein temporäres Rechtekontozertifikat von einem normalen Rechtekontozertifikat? Wie stellt RMS fest, dass es im Kioskmodus verwendet wird?

Die RMS-fähige Anwendung muss bestimmen, ob der RMS-Client ein temporäres oder ein normales Rechtekontozertifikat für den Benutzer anfordern soll. Es gibt kein bestimmtes Verfahren, um dies zu ermitteln. Microsoft Office 2003 ist ein Beispiel für eine RMS-fähige Anwendung, die dem Benutzer die Auswahl des entsprechenden Rechtekontozertifikats ermöglicht.

Der Hauptunterschied zwischen einem temporären und einem normalen Rechtekontozertifikat ist das Vorhandensein der Sicherheits-ID (SID) des Benutzers und die Angabe der Gültigkeitsdauer. Temporäre Rechtekontozertifikate enthalten keine Benutzer-SID und haben eine Gültigkeitsdauer, die in Minuten angegeben ist. Die standardmäßige Gültigkeitsdauer eines temporären Rechtekontozertifikats ist 15 Minuten. Normale Rechtekontozertifikate hingegen enthalten die SID des Benutzers und haben eine Gültigkeitsdauer, die in Tagen angegeben ist. Die standardmäßige Gültigkeitsdauer eines normalen Rechtekontozertifikats ist 365 Tage.

<span id="BKMK_14"></span>
#### Wann wird ein temporäres Rechtekontozertifikat verwendet?

Ein temporäres Rechtekontozertifikat soll einem Benutzer das Abrufen von RMS-geschütztem Inhalt auf Computern ermöglichen, die eines der folgenden Kriterien erfüllen:

-   Computer ist nicht Mitglied derselben Gesamtstruktur wie die RMS-Installation, von der das Rechtekontozertifikat erworben wurde
-   Computer ist nicht Mitglied derselben Gesamtstruktur, in der sich das Benutzerkonto befindet.
-   Es kann nicht sichergestellt werden, dass der Benutzer denselben Computer später erneut verwenden kann.

Diese Kriterien treffen beispielsweise auf Computer in Flughafenterminals, öffentlichen Bibliotheken und Internetcafés zu.

<span id="BKMK_15"></span>
#### Stellt RMS X.509v3-Zertifikate aus?

Nein, RMS stellt XrML-Zertifikate (eXtensible Rights Markup Language) aus. Die dadurch ermöglichte Benutzerdarstellung und Richtlinienstruktur geht über den Rahmen von X.509v3-Zertifikaten hinaus.

<span id="BKMK_16"></span>
#### Wo werden XrML-Zertifikate gespeichert?

Die folgenden von einem RMS-System verwendeten Zertifikate und Lizenzen werden in XrML auf dem Clientcomputer gespeichert.

-   Computerzertifikat
    Dateiname: CERT-Machine.drm
    Speicherort: %USERPROFILE%\\Lokale Einstellungen\\Anwendungsdaten\\Microsoft\\DRM\\
-   Rechtekontozertifikat
    Dateinamenpräfix: GIC
    Speicherort: %USERPROFILE%\\Lokale Einstellungen\\Anwendungsdaten\\Microsoft\\DRM
-   Client-Lizenzgeberzertifikat
    Dateinamenpräfix: CLC
    Speicherort: %USERPROFILE%\\Lokale Einstellungen\\Anwendungsdaten\\Microsoft\\DRM
-   Nutzungslizenz
    Dateinamenpräfix: EUL
    Speicherort: %USERPROFILE%\\Lokale Einstellungen\\Anwendungsdaten\\Microsoft\\DRM

| ![](images/Cc747725.note(WS.10).gif)Hinweis                                                                                        |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ein Benutzerkonto hat jeweils ein Computerzertifikat, eine GIC-Datei und eine CLC-Datei, jedoch mehrere EUL-Dateien für jeden Inhalt, auf den zugegriffen wird. |

| ![](images/Cc747725.note(WS.10).gif)Hinweis                                                  |
|---------------------------------------------------------------------------------------------------------------------------|
| Für den in Windows Vista® integrierten RMS-Client lautet der Speicherort „%USERPROFILE%\\AppData\\Local\\Microsoft\\DRM“. |

<span id="BKMK_17"></span>
#### Wo wird das Computerschlüsselpaar (privat/öffentlich) gespeichert?

Der private Computerschlüssel wird auf sichere Weise gespeichert, indem er durch kryptografische Schlüssel geschützt wird, die auf den Anmeldeinformationen des Benutzers und der Computerkonfiguration basieren.

<span id="BKMK_18"></span>
#### Wo wird das Clientschlüsselpaar (privat/öffentlich) gespeichert?

Das Schlüsselpaar für ein Benutzerkonto wird im Rechtekontozertifikat (RAC) gespeichert.

<span id="BKMK_19"></span>
#### AES (Advanced Encryption Standard, erweiterter Verschlüsselungsstandard) ist ein symmetrischer Algorithmus. Wie werden die Schlüssel zwischen dem Server und dem Benutzer auf sichere Weise ausgetauscht?

Es werden sowohl symmetrische als auch öffentliche und private Schlüssel im System verwendet. Der Inhalt wird mit einem symmetrischen Schlüssel verschlüsselt, bei den anderen Schlüsseln (für Benutzer, Computer und Server) handelt es sich jedoch um öffentliche und private RSA-Schlüssel. Der symmetrische Inhaltsschlüssel wird immer in den jeweiligen Lizenzen verschlüsselt: entweder mit dem öffentlichen RSA-Schlüssel des RMS-Servers in der Veröffentlichungslizenz oder mit dem öffentlichen RSA-Schlüssel des Benutzers in der Nutzungslizenz.
