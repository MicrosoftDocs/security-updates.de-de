---
TOCTitle: Unterstützung der Internetinformationsdienste für RMS
Title: Unterstützung der Internetinformationsdienste für RMS
ms:assetid: 'bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c'
ms:contentKeyID: 18118987
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747649(v=WS.10)'
---

Unterstützung der Internetinformationsdienste für RMS
=====================================================

Die primären RMS-Dienste werden durch eine Reihe von ASP .NET Webdiensten bereitgestellt. Diese Webdienste werden unter Microsoft® Internetinformationsdienste (Internet Information Services oder IIS) ausgeführt. Während des Serverbereitstellungsprozesses erstellt RMS (Rights Management Services oder Dienste für die Rechteverwaltung) virtuelle Verzeichnisse in den Internetinformationsdiensten. In diesen Verzeichnissen werden die Anwendungsdateien für die Webdienste installiert.

Während der Serverbereitstellung können Sie die Website, unter der virtuelle Verzeichnisse eingerichtet werden sollen, aus einer Liste der auf dem Server vorhandenen Websites auswählen. Bevor Sie einen Server bereitstellen, sollten Sie eventuell eine spezielle Website für RMS erstellen. In diesem Fall können Sie speziell für Ihre RMS-Implementierung geltende Authentifizierung und Zugriffsbeschränkungen konfigurieren.

Standardmäßig werden die Webdienstdateien und virtuellen Verzeichnisse durch freigegebene Zugriffssteuerungslisten (Discretionary Access Control Lists oder DACLs) geschützt, um nicht autorisierten Zugriff auf ihre Funktionen zu verhindern. Die Einträge für die Zugriffssteuerung (Access Control Entries oder ACEs) für diese Elemente lauten wie folgt:

-   Die Administratorgruppe verfügt über Vollzugriff.
-   Das lokale System verfügt über Vollzugriff.
-   Die RMS Service Group (RMS-Dienstgruppe) verfügt über die Berechtigungen Lesen und Ausführen.
-   Gäste und Benutzer verfügen über die Berechtigungen Lesen und Ausführen, Ordnerinhalt auflisten sowie Lesen.
-   Anonymer Zugriff ist unzulässig.

In der folgenden Tabelle werden die in IIS erstellten virtuellen Verzeichnisse und die in diesen Verzeichnissen installierten Dienste aufgelistet.

<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Virtuelles Verzeichnis</th>
<th style="border:1px solid black;" >Dienst</th>
<th style="border:1px solid black;" >Webdienstdatei</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">_wmcs</td>
<td style="border:1px solid black;">Dies ist das virtuelle Verzeichnis für die RMS-Clusterverwaltung.</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certification</td>
<td style="border:1px solid black;">Dieses virtuelle Verzeichnis enthält die Dienste zur Unterstützung der RMS-Zertifizierung.</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Aktivierungsproxy</td>
<td style="border:1px solid black;">Activation.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Kontozertifizierung</td>
<td style="border:1px solid black;">Certification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Vorzertifizierung</td>
<td style="border:1px solid black;">Precertification.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Dienstlocator</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Server</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Serverzertifizierung</td>
<td style="border:1px solid black;">ServerCertification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Zertifizierung mobiler Geräte</td>
<td style="border:1px solid black;">MobileDeviceCertfication.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Registrierung</td>
<td style="border:1px solid black;">SubEnrollService.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licensing</td>
<td style="border:1px solid black;">Dieses virtuelle Verzeichnis enthält die Dienste zur Unterstützung der RMS-Lizenzierung.</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Lizenzierung</td>
<td style="border:1px solid black;">License.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Veröffentlichen</td>
<td style="border:1px solid black;">Publish.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Server</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Dienstlocator</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Admin</td>
<td style="border:1px solid black;">Dieses virtuelle Verzeichnis enthält die Dienste zur Unterstützung der RMS-Verwaltung.</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Verwaltung</td>
<td style="border:1px solid black;">AdminSvc.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">.NET Remoting-Schnittstelle</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DirectoryServices</td>
<td style="border:1px solid black;">Dies ist ein Unterverzeichnis von DrmRemote.</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Der Verwaltungsdienst ist stärker als die anderen Webdienste eingeschränkt, weil RMS über die vorgesehenen Schnittstellen konfiguriert werden kann. Aus diesem Grund können Mitglieder der Benutzergruppe auf den Verwaltungsdienst nicht zugreifen. Außerdem sind IP-Filter aktiviert, um den Zugriff nur auf den lokalen Computer zu gewähren. Das virtuelle Verzeichnis DirectoryServices gewährt anonymen Benutzern keinen Zugriff. Darüber hinaus gewährt der Dienstlocatordienst Vollzugriff auf das Konto Netzwerkdienst. Zum Bereitstellen eines Lizenzierungsservers müssen Sie die Standardeinträge für die Zugriffssteuerung ändern, um dem RMS-Administrator Zugriff zu erteilen. |