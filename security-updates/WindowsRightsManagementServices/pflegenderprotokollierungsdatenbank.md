---
TOCTitle: Pflegen der Protokollierungsdatenbank
Title: Pflegen der Protokollierungsdatenbank
ms:assetid: 'de55058b-0d1a-4997-8a45-e14678ddd13f'
ms:contentKeyID: 18119055
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747691(v=WS.10)'
---

Pflegen der Protokollierungsdatenbank
=====================================

In Protokolleinträgen finden sich auch Kopien der Lizenzen, die für verschiedene RMS-Operationen ausgestellt wurden – beispielsweise zum Registrieren von Benutzern und Zuweisen von Nutzungslizenzen. Wenn all diese Protokolleinträge entweder erfolgreiche Benutzerregistrierungen oder erfolgreiche Anforderungen von Nutzungslizenzen sind, bedeutet jeder Protokolleintrag eine Vergrößerung der Protokollierungsdatenbank um etwa 200 KB.

Beispiel: Eine RMS-geschützte E-Mail-Nachricht wird an alle Mitarbeiter eines Unternehmens mit 50.000 Benutzern versendet, und alle Mitarbeiter öffnen sie. Wenn jeder Mitarbeiter diese Nachricht im Laufe desselben Tages öffnen würde, würde die Protokollierungsdatenbank um 10 GB anwachsen. Es ist möglich, den Listenerdienst so zu konfigurieren, dass die tatsächlichen XrML-Daten nicht protokolliert werden. Dies würde bedeuten, dass eine geringere Datenmenge erfasst wird.

Sie sollten unter Umständen Skripte zur Archivierung älterer Daten aus der Protokollierungsdatenbank in eine andere Datenbank erstellen. Beispiele für Protokollierungsskripte finden sich im RMS-Toolkit, das kostenfrei von der [Microsoft Website](http://go.microsoft.com/fwlink/?linkid=26724)(http://go.microsoft.com/fwlink/?LinkId=26724) heruntergeladen werden kann.

Faktoren, die das Wachstum der Protokollierungsdatenbank beeinflussen
---------------------------------------------------------------------

Eine Vorhersage über die Größe einer Protokollierungsdatenbank kann nur in Abhängigkeit von der vorhandenen Umgebung getroffen werden. Eine Anzahl von Einträgen in Folge der Inbetriebnahme können als gegeben vorausgesetzt werden. Beispiele:

-   RMS-Serverregistrierung
-   Benutzerregistrierung (eine einzelne Anforderung für jeden Computer, der von einem Benutzer verwendet wird)
-   Automatisierte Benutzeranforderungen von Offline-Veröffentlichungszertifikaten

Der Großteil der Einträge in der Protokollierungsdatenbank nach der ursprünglichen Startphase hängt mit dem Ausstellen von Nutzungslizenzen für geschützte Inhalte zusammen. Mehrere Faktoren beeinflussen das Wachstum der Datenbank:

-   Die Erfordernis einer neuen Lizenz für jeden Benutzerzugriff auf geschützte Inhalte Dies stellt nicht die Standardmethode für geschützte Dokumente dar, ist jedoch als Option wählbar. Wenn diese Anforderung umgesetzt werden sollte, wachsen die Datenbanken schneller.
-   Geschätzte Anzahl geschützter E-Mail-Nachrichten pro Person pro Tag
-   Geschätzte Anzahl individueller Benutzer, die diese geschützten Nachrichten lesen werden
-   Geschätzte Anzahl geschützter Dokumente, die täglich von allen Teilnehmern mit Microsoft Office 2003 (Word, PowerPoint und Excel) erstellt werden
-   Geschätzte Empfängeranzahl dieser geschützten Dokumente

Zu Beginn wird die Größe der Protokollierungsdatenbank im Bereich von 1,7 MB liegen; dies schließt die Anforderung eines Zertifikats durch den RMS-Server mit ein. Wenn sich ein neuer Benutzer anmeldet, erhält er ein Rechtekontozertifikat und ein Client-Lizenzgeberzertifikat. Diese beiden Vorgänge werden protokolliert, was zu einer Vergrößerung der Protokollierungsdatenbank um 0,06 MB führt. Jedes Mal, wenn ein Benutzer eine Lizenz für geschützte Inhalte erwirbt, wächst die Datenbank um 0,19 MB.

Zur Verdeutlichung: Beispielsweise stellt eine Organisation RMS für ihre 5000 Benutzer bereit. Jeder Benutzer verfügt über einen Computer, und die Organisation verwendet zwei RMS-Server. Nach der Bereitstellung erstellt jeder Benutzer durchschnittlich eine RMS-geschützte E-Mail-Nachricht täglich, die an fünf andere Benutzer versendet wird. Darüber hinaus erstellt jeder Benutzer im Laufe eines Tages ein RMS-geschütztes Dokument, auf das drei andere Benutzer zugreifen. Die folgende Tabelle enthält geschätzte Zahlen, die verdeutlichen, wie sich diese Aktivitäten auf das Wachstum der Protokollierungsdatenbank auswirken.

<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Vorgang</th>
<th style="border:1px solid black;" >Protokollwachstum</th>
<th style="border:1px solid black;" >Gesamtgröße Protokoll</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS-Server wird erfolgreich bereitgestellt</td>
<td style="border:1px solid black;">1,7 MB</td>
<td style="border:1px solid black;">1,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Registrierung von 5000 Mitarbeitern (5000*0,06)</td>
<td style="border:1px solid black;">300 MB</td>
<td style="border:1px solid black;">301,7 MB</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zugriff auf geschützte E-Mails (25.000*0,19)</td>
<td style="border:1px solid black;">4,750 MB</td>
<td style="border:1px solid black;">5.051,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zugriff auf geschützte Dokumente (15.000*0,19)</td>
<td style="border:1px solid black;">2,850 MB</td>
<td style="border:1px solid black;">7.901,7 MB</td>
</tr>
</tbody>
</table>
  
Dies bedeutet, dass die Protokollierungsdatenbank nach der Registrierung eine Größe von etwa 300 MB hat. Das tägliche Wachstum im vorliegenden Beispiel beträgt jedoch 7,6 GB – dies entspricht fast der Begrenzung von 8 GB für die Standardinstallation von Message Queuing. Wenn die Protokollierungsdatenbank für mehr als einen Tag nicht zur Verfügung stünde, würden Protokolleinträge verloren gehen.
  
Kontrollieren der Größe der Protokollierungsdatenbank  
-----------------------------------------------------
  
Die Bereitstellungsplanung muss auch eine Methode umfassen, mit der die Größe der Protokollierungsdatenbank kontrolliert wird. Die folgenden Methoden sind dabei die verbreitetsten Ansätze.
  
-   **Auslesen und archivieren**  
    Bei dieser Vorgehensweise werden mithilfe von Skripten unter SQL Server zuvor festgelegte Daten aus der Protokollierungsdatenbank in eine untergeordnete Datenbank übertragen, sobald sie ein bestimmtes Alter erreichen. Darüber hinaus werden unwichtige Daten aus der Datenbank herausgefiltert, sodass kein Speicherplatz verschwendet wird.  
-   **Beschränken der protokollierten Daten**  
    Die Protokollierungsdatenbank setzt sich aus drei Haupttabellen zusammen. Eine davon ist **DRMS\_Log\_Filter**, über die ermittelt wird, welches Feld in der Haupttabelle protokolliert werden soll, wenn ein Protokollfilter verwendet wird.  
    Über die Einträge unter „on/off“ wird festgelegt, welche Felder der Haupttabelle vom Protokollierungslistenerdienst des RMS-Servers für das Protokoll erfasst werden. Zwei dieser Felder (mit XrML-Bezug) wurden bereits auf 0 gesetzt, d. h. für sie erfolgt keine Protokollierung, da sie etwa 99 % des Umfangs der Zellen für Lizenzanforderungen ausmachen.  
    Eine weitere Tabelle in der Datenbank **DRMS\_Config\_ServerName\_Port** namens **DRMS\_ClusterPolicies** enthält den **PolicyName** (Richtliniennamen) **LoggingFiltering**. **LoggingFiltering** ist standardmäßig nicht aktiviert. Wenn der Wert für **LoggingFiltering** auf 1 gesetzt und der Protokollierungslistenerdienst neu gestartet wird, würde sich das tägliche Wachstum der Datenbank aus dem obigen Beispiel von 7,6 GB auf etwa 160 MB verringern.  
-   **Verschieben der Protokollierungsdatenbank**  
    Eine weitere Verwaltungsoption für schnell wachsende Protokollierungsdatenbanken wäre es, sie auf einen Server mit mehr Speicherplatz zu verschieben. Die Protokollierungsdatenbank muss sich nicht auf demselben Datenbankserver wie die Konfigurationsdatenbank befinden. Wenn Sie die Datenbank auf einen anderen Server verschieben möchten, gehen Sie wie folgt vor:  
    1.  Beenden Sie den Protokollierungslistenerdienst auf den RMS-Servern.  
    2.  Kopieren Sie die Datenbank auf den anderen Server oder erstellen Sie dort eine neue.  
    3.  Bearbeiten Sie die Datenbank **DRMS\_Config\_ServerName\_Port** durch Auswählen der Tabelle **DRMS\_ClusterPolicies** und Anpassen der Werte unter **LoggingDatabaseName** (Name der Datenbank) und **LoggingDatabaseServer** (Name des Datenbankservers).  
    4.  Starten Sie IIS über die Befehlszeile durch Ausführen von „IISRESET.exe“ neu.