---
TOCTitle: Sicherheit während der Bereitstellung
Title: Sicherheit während der Bereitstellung
ms:assetid: '9f1282c5-5642-4870-a9a4-c3a485f8ff76'
ms:contentKeyID: 18118953
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747616(v=WS.10)'
---

Sicherheit während der Bereitstellung
=====================================

Sie können die RMS-Verwaltungswebsite dazu verwenden, RMS-Ressourcen auf einer vorhandenen Website bereitzustellen. Während der Bereitstellung werden virtuelle Verzeichnisse und Anwendungspools auf dieser Website sowie RMS-Datenbanken auf einem Datenbankserver erstellt und konfiguriert. Wenn Ihr Server eine Verbindung zum Internet hat, kann er während des Bereitstellungsprozesses optional beim Microsoft-Registrierungsdienst registriert werden.

Während der Bereitstellung verwendet RMS (Rights Management Services oder Dienste für die Rechteverwaltung) die Konten, die in der folgenden Tabelle beschrieben werden.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Konto</th>
<th>Zweck</th>
<th>Berechtigungen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Konto des angemeldeten Benutzers</p></td>
<td style="border:1px solid black;"><p>Erstellt virtuelle Verzeichnisse und Anwendungspools. Für IIS (Internet Information Services oder Internetinformationsdienste) ist eine Windows-Authentifizierung erforderlich, und RMS verkörpert dabei den angemeldeten Benutzer, der lokal angemeldet sein muss.</p></td>
<td style="border:1px solid black;"><p>Vollzugriff (der angemeldete Benutzer muss ein lokaler Administrator sein).</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Systemkonto</p></td>
<td style="border:1px solid black;"><p>Erstellt die temporäre Assemblierung für Serialisierung.</p></td>
<td style="border:1px solid black;"><p>Berechtigungen Lesen und Schreiben für den temporären Windows-Ordner C:\Windows\Temp.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>ASPNET-Konto</p></td>
<td style="border:1px solid black;"><p>Erstellt die temporäre Assemblierung der *.aspx-Dateien.</p></td>
<td style="border:1px solid black;"><p>Zugriff auf das temporäre Assemblierungscacheverzeichnis, standardmäßig C:\Windows\Microsoft.NET\Framework\v1.1.4322\Temporary ASP.NET Files.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Konto Netzwerkdienste</p></td>
<td style="border:1px solid black;"><p>Registriert den Dienstverbindungspunkt in Active Directory.</p></td>
<td style="border:1px solid black;"><ul>
<li>Berechtigungen Nur lesen für die Site für den Bereitstellungsprozess (normalerweise C:\Inetpub\Wwwroot\Provisioning).<br />  
<br />  
</li>  
<li>Berechtigungen „Lesen“ und „Schreiben“ für den Registrierungsschlüssel <strong>DRMS</strong> . Die Berechtigungen werden von RMS-Setup erteilt, das auch folgende Registrierungsschlüssel erstellt.<br />  
<br />  
Auf Computern mit der 32-Bit-Version von Windows Server 2003<br />  
<br />  
<code>HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0</code><br />  
<br />  
Auf Computern mit der 64-Bit-Version von Windows Server 2003<br />  
<br />  
<code>HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0</code><br />  
<br />  
</li>
</ul></td>
</tr>
</tbody>
</table>
<p> </p>

Während der Bereitstellung führt RMS folgende Aufgaben aus:

-   Auf dem Datenbankserver:
    -   Erstellt die Konfigurations- und Protokollierungsdatenbank sowie die Datenbank der Verzeichnisdienste.
    -   Erteilt Berechtigungen zum Anmelden für die RMS Service Group (RMS-Dienstgruppe).
    -   Installiert gespeicherte Prozeduren in den Datenbanken und erteilt Berechtigungen zum Ausführen für die RMS Service Group.
    -   Führt Abfragen in der Masterdatenbank aus.
-   Fügt zu der Gruppe IIS\_WPG die RMS Service Group hinzu.
-   Erstellt unter C:\\Inetpub\\Wwwroot\\\_wmcs eine Hierarchie virtueller Verzeichnisse, Dateien und Anwendungspools für die Webdienste und die RMS-Verwaltungswebsite.
-   Legt freigegebene Zugriffssteuerungslisten (Discretionary Access Control Lists oder DACLs) für die virtuellen Verzeichnisse, Dateien und Anwendungspools fest.
-   Gewährt der RMS Service Group Zugriff auf den temporären Ordner.
-   Verschlüsselt bei angegebenem softwarebasiertem Schutz des Schlüssels den privaten Server-Lizenzgeberschlüssel, bevor es ihn in der Datenbank speichert. RMS fordert während der Bereitstellung ein Kennwort an und erhält Zugriff auf DPAPI auf Maschinenebene.
-   Installiert den Protokollierungslistenerdienst.
-   Erstellt eine Warteschlange für Protokollierungsnachrichten.
-   Legt beim Bereitstellen des Stammzertifizierungsservers den Dienstverbindungspunkt in Active Directory fest.
