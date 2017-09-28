---
TOCTitle: 'RMS-Serverinstallation mithilfe einer Eingabeaufforderung'
Title: 'RMS-Serverinstallation mithilfe einer Eingabeaufforderung'
ms:assetid: 'b55b1e2a-dd14-4168-a37f-9cdedbec660b'
ms:contentKeyID: 18118991
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747733(v=WS.10)'
---

RMS-Serverinstallation mithilfe einer Eingabeaufforderung
=========================================================

Sie können RMS (Rights Management Services oder Dienste für die Rechteverwaltung) mit Service Pack 2 (SP2) über eine Eingabeaufforderung installieren und so die Installation automatisieren. Eine Automatisierung der Installation ist auf zwei Arten möglich: durch Ausführen einer unbeaufsichtigten Installation mithilfe des heruntergeladenen EXE-Clients oder durch Verwenden der aus der heruntergeladenen EXE-Datei extrahierten MSI-Dateien zum Installieren des RMS-Clients. Für die Installation mithilfe der heruntergeladenen EXE-Datei verwenden Sie bitte folgende Syntax:

**WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q**

Für die Installation mithilfe der Windows® Installer (.msi) Dateien müssen Sie zuerst die MSI-Dateien aus den RMS mit der ausführbaren Datei des SP2 extrahieren. Der folgende Befehl kann über eine Eingabeaufforderung ausgeführt werden, um die Dateien msdrmclient.msi und RmClientBackCompat.msi zu extrahieren:

**WindowsRightsManagementServiceSP2-KB917275-Server-ENU.exe /X:C:\\RMS***Installationsort*

Nachdem Sie die MSI-Dateien extrahiert haben, können Sie folgende Befehle zur Installation von RMS verwenden:

**msiexec.exe /I MSDrmClient.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Installationsort*

**msiexec.exe /I RMClientBackCompat.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Installationsort*

In der untenstehenden Tabelle wird die Syntax für jeden Befehl erläutert.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parameter</th>
<th>Definition</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/I MSDrmClient.msi</strong> oder <strong>/I RMClientBackCompat.msi</strong></td>
<td style="border:1px solid black;">Erforderlich. Gibt das zu installierende Produkt an.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/qn</strong></td>
<td style="border:1px solid black;">Optional. Gibt eine Installation ohne Rückfrage an, bei der der Benutzer nicht eingreifen muss.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/lei</strong> <em>/lei logfile.log</em></td>
<td style="border:1px solid black;">Optional. Gibt die Datei an, in der Fehler- und Statusmeldungen protokolliert werden sollen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>DISPLAYPAGE=”NO”</strong></td>
<td style="border:1px solid black;">Optional. Gibt an, dass die Seite <strong>Globale Verwaltung</strong> nach der Installation nicht angezeigt wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>TARGETDIR=c:\</strong><em>Installationsort</em></td>
<td style="border:1px solid black;">Optional. Gibt das Verzeichnis an, in dem RMS mit Service Pack 2 installiert werden soll. Wenn Sie keinen Pfad angeben, wird der Standardinstallationspfad verwendet.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747733.note(WS.10).gif)Hinweis                                                                                                                                                                                            |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Unabhängig von der Installationsmethode sollten Sie sicherstellen, dass beide MSI-Dateien fehlerfrei installiert wurden. Falls ein Fehler auftritt, der die Installation von „MSDrmClient.msi“ verhindert, sollten Sie „RMClientBackCompat.msi“ nicht installieren. |
