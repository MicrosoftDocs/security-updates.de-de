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
<th>Virtuelles Verzeichnis</th>
<th>Dienst</th>
<th>Webdienstdatei</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>_wmcs</p></td>
<td style="border:1px solid black;"><p>Dies ist das virtuelle Verzeichnis für die RMS-Clusterverwaltung.</p></td>
<td style="border:1px solid black;"><p>Nicht zutreffend</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Certification</p></td>
<td style="border:1px solid black;"><p>Dieses virtuelle Verzeichnis enthält die Dienste zur Unterstützung der RMS-Zertifizierung.</p></td>
<td style="border:1px solid black;"><p>Nicht zutreffend</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Aktivierungsproxy</p></td>
<td style="border:1px solid black;"><p>Activation.asmx</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Kontozertifizierung</p></td>
<td style="border:1px solid black;"><p>Certification.asmx</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Vorzertifizierung</p></td>
<td style="border:1px solid black;"><p>Precertification.asmx</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Dienstlocator</p></td>
<td style="border:1px solid black;"><p>ServiceLocator.asmx</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Server</p></td>
<td style="border:1px solid black;"><p>Server.asmx</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Serverzertifizierung</p></td>
<td style="border:1px solid black;"><p>ServerCertification.asmx</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Zertifizierung mobiler Geräte</p></td>
<td style="border:1px solid black;"><p>MobileDeviceCertfication.asmx</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Registrierung</p></td>
<td style="border:1px solid black;"><p>SubEnrollService.asmx</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Licensing</p></td>
<td style="border:1px solid black;"><p>Dieses virtuelle Verzeichnis enthält die Dienste zur Unterstützung der RMS-Lizenzierung.</p></td>
<td style="border:1px solid black;"><p>Nicht zutreffend</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Lizenzierung</p></td>
<td style="border:1px solid black;"><p>License.asmx</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Veröffentlichen</p></td>
<td style="border:1px solid black;"><p>Publish.asmx</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Server</p></td>
<td style="border:1px solid black;"><p>Server.asmx</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Dienstlocator</p></td>
<td style="border:1px solid black;"><p>ServiceLocator.asmx</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Admin</p></td>
<td style="border:1px solid black;"><p>Dieses virtuelle Verzeichnis enthält die Dienste zur Unterstützung der RMS-Verwaltung.</p></td>
<td style="border:1px solid black;"><p>Nicht zutreffend</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Verwaltung</p></td>
<td style="border:1px solid black;"><p>AdminSvc.asmx</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DrmRemote</p></td>
<td style="border:1px solid black;"><p>.NET Remoting-Schnittstelle</p></td>
<td style="border:1px solid black;"><p>Nicht zutreffend</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DirectoryServices</p></td>
<td style="border:1px solid black;"><p>Dies ist ein Unterverzeichnis von DrmRemote.</p></td>
<td style="border:1px solid black;"><p>Nicht zutreffend</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Der Verwaltungsdienst ist stärker als die anderen Webdienste eingeschränkt, weil RMS über die vorgesehenen Schnittstellen konfiguriert werden kann. Aus diesem Grund können Mitglieder der Benutzergruppe auf den Verwaltungsdienst nicht zugreifen. Außerdem sind IP-Filter aktiviert, um den Zugriff nur auf den lokalen Computer zu gewähren. Das virtuelle Verzeichnis DirectoryServices gewährt anonymen Benutzern keinen Zugriff. Darüber hinaus gewährt der Dienstlocatordienst Vollzugriff auf das Konto Netzwerkdienst. Zum Bereitstellen eines Lizenzierungsservers müssen Sie die Standardeinträge für die Zugriffssteuerung ändern, um dem RMS-Administrator Zugriff zu erteilen. |
