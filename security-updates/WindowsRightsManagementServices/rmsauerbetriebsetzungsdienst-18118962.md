---
TOCTitle: 'RMS-Außerbetriebsetzungsdienst'
Title: 'RMS-Außerbetriebsetzungsdienst'
ms:assetid: '97677e3b-bc83-47ec-b6db-d326cd94566c'
ms:contentKeyID: 18118962
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747695(v=WS.10)'
---

RMS-Außerbetriebsetzungsdienst
==============================

Der Außerbetriebsetzungdienst ist ein angepasster Webdienst, der von RMS-Setup installiert wird. Er wird auf Stamm- und Lizenzierungsclustern ausgeführt. Wenn Sie diesen Dienst aktivieren, werden alle anderen RMS-Webdienste auf dem Server deaktiviert.

Dieser Dienst entschlüsselt den Inhaltsschlüssel in der Veröffentlichungslizenz von durch Rechte geschützten Inhalten und stellt diesen Schlüssel einem Client als Antwort auf eine Lizenzierungsanforderung bereit. Damit wird das Speichern der Inhalte ohne RMS-Schutz ermöglicht. Der Außerbetriebsetzungsdienst protokolliert alle an ihn gesendeten Clientanforderungen und sendet sie an den Protokollierungslistenerdienst, damit sie in der Protokollierungsdatenbank aufgezeichnet werden.

Sie können den Außerbetriebsetzungsdienst auf der Seite **Sicherheitseinstellungen** der Verwaltungswebsite aktivieren. Nach der Aktivierung dieses Dienstes können Sie den Server nicht auf eine RMS-Standardkonfiguration wiederherstellen.

Nachdem Sie den Dienst aktiviert haben, sollten Sie in der DACL (Discretionary Access Control List oder freigegebene Zugriffssteuerungsliste) der Datei decommission.asmx den Zugriff für Benutzer in Ihrem Unternehmen ermöglichen, die diesen Server zur Lizenzierung ihres Inhalts verwendet haben, und der DACL die RMS Service Group (RMS-Dienstgruppe) mit den Berechtigungen zum Lesen und Ausführen hinzufügen, damit RMS seine Operationen verwalten kann. Nachdem der Schutz für alle durch den Server veröffentlichten Inhalte aufgehoben wurde, sollten Sie die Informationen zum privaten Schlüssel sichern und RMS vom Server entfernen.

Die Standardzugriffsteuerungsliste bei diesem Dienst wird in folgender Tabelle gezeigt:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Benutzer oder Gruppe</th>
<th>Standardberechtigung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>SYSTEM</p></td>
<td style="border:1px solid black;"><p>Vollzugriff</p></td>
</tr>
</tbody>
</table>
