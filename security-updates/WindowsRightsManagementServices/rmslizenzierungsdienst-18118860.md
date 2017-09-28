---
TOCTitle: 'RMS-Lizenzierungsdienst'
Title: 'RMS-Lizenzierungsdienst'
ms:assetid: '5cad1baf-0304-4e82-b62d-83a4aac2140b'
ms:contentKeyID: 18118860
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720278(v=WS.10)'
---

RMS-Lizenzierungsdienst
=======================

Der Lizenzierungsdienst, mit dem Nutzungslizenzen ausgegeben werden, wird auf dem RMS-Stammcluster sowie auf allen Lizenzierungsclustern ausgeführt. Nutzungslizenzen ermöglichen Benutzern das Abrufen von durch Rechte geschützte Inhalte.

Die Anwendungsdatei für den Lizenzierungsdienst, License.asmx, befindet sich im virtuellen Verzeichnis Licensing von IIS (Internet Information Services oder Internetinformationsdienste).

| ![](images/Cc720278.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sie können einen separaten Lizenzierungscluster bereitstellen, um Lizenzierungsanforderungen vom Stammcluster zu verschieben. Außerdem können Sie einen separaten Lizenzierungsserver oder -cluster für eine Abteilung bereitstellen, damit diese beispielsweise eigene Benutzerrechterichtlinien einrichten kann. Weitere Informationen zu diesen Möglichkeiten finden Sie unter „Identifizieren von Kernkomponenten“ im Abschnitt „Planen einer RMS-Bereitstellung“ in dieser Dokumentationssammlung. |

Die Standardzugriffsteuerungsliste bei diesem Dienst wird in folgender Tabelle gezeigt:

###  

 
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
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Vollzugriff</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS-Dienstgruppe</td>
<td style="border:1px solid black;">Lesen und Ausführen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Vollzugriff</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Benutzer</td>
<td style="border:1px solid black;">Lesen und Ausführen</td>
</tr>
</tbody>
</table>
