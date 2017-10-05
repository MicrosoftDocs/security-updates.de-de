---
TOCTitle: Für RMS erforderliche Konten und Berechtigungen
Title: Für RMS erforderliche Konten und Berechtigungen
ms:assetid: '07a51daa-6823-41e6-b453-92f1a0592361'
ms:contentKeyID: 18118741
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720178(v=WS.10)'
---

Für RMS erforderliche Konten und Berechtigungen
===============================================

In der folgenden Tabelle werden die zum Bereitstellen und Verwalten von RMS erforderlichen Benutzerrechte und Berechtigungen angegeben.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Aktion</th>
<th style="border:1px solid black;" >Benutzerkonto und Berechtigungen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Installieren von RMS</td>
<td style="border:1px solid black;">Melden Sie sich unter Verwendung eines Domänenkontos an, das ein Mitglied der lokalen Administratorgruppe ist.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bereitstellen von RMS</td>
<td style="border:1px solid black;">Melden Sie sich unter Verwendung eines Domänenkontos an, das ein Mitglied der lokalen Administratorgruppe ist. Außerdem muss das verwendete Konto über eine SQL-Anmeldung verfügen, dem die Rolle „Systemadministrator“ für die SQL Server-Datenbank zugewiesen wurde, so dass RMS die Datenbank einrichten kann.
Während der Bereitstellung müssen Sie das bereits erstellte RMS-Dienstkonto angeben. Bei dem Konto sollte es sich um ein Standard-Domänenbenutzerkonto ohne zusätzliche Berechtigungen handeln. Dieses Konto wird als Mitglied zur RMS Service Group (RMS-Dienstgruppe) hinzugefügt und dient als Konto für RMS während der Ausführung von Standardoperationen.
Für Einzelserverbereitstellungen, bei denen sich die Datenbank auf demselben Computer befindet wie der Stammzertifizierungsserver, können Sie auch das Konto „Lokales System“ angeben. Aus Sicherheitsgründen sollte statt des Kontos „Lokales System“ jedoch immer das RMS-Dienstkonto angegeben werden. Wenn sich die Datenbank auf einem separaten Server befindet, müssen Sie das RMS-Dienstkonto angeben.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Verwalten von RMS</td>
<td style="border:1px solid black;">Melden Sie sich unter Verwendung eines Domänenkontos an, das ein Mitglied der lokalen Administratorgruppe ist. Sie können Sicherheitseinstellungen anpassen, um den Zugriff auf die Verwaltungswebseiten zu verwalten.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720178.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Das Konto, das zur Anmeldung am RMS-Server dient, erfordert keine Mitgliedschaft in anderen Domänengruppen, wie z. B. der Gruppe „Domänen-Admins“. Einige besondere Verwaltungsaufgaben, wie etwa das Registrieren des Dienstverbindungspunkts und das Ändern der Sicherheitsrichtlinien, erfordern jedoch die Verwendung eines Kontos mit zusätzlichen Berechtigungen. |
