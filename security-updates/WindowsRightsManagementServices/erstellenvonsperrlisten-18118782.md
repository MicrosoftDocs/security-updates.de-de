---
TOCTitle: Erstellen von Sperrlisten
Title: Erstellen von Sperrlisten
ms:assetid: '1ef75199-3344-4225-84de-a863a777696a'
ms:contentKeyID: 18118782
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720208(v=WS.10)'
---

Erstellen von Sperrlisten
=========================

Beim Implementieren der Sperrung ist das Bereitstellen einer Sperrliste erforderlich. Dabei handelt es sich um ein XML-Dokument, das die XrML-Sprache (eXtensible Rights Markup Language) verwendet und die Prinzipale auflistet, die keinen Zugriff mehr auf durch Rechte geschützte Inhalte haben sollen. Sie müssen Sperrlisten erstellen, die mit einem Zeitstempel versehen und entsprechend mit dem in RMS bereitgestellten Tool zum Signieren von Sperrlisten („RLsigner.exe“) signiert wurden.

| ![](images/Cc720208.Important(WS.10).gif)Wichtig                         |
|-------------------------------------------------------------------------------------------------------|
| Um die Sperrliste mit „RLsigner.exe“ signieren zu können, müssen Sie sie als Unicode-Datei speichern. |

Beispiel für eine Sperrliste
----------------------------

In diesem Thema wird ein umfassendes Sperrlistenbeispiel dargestellt, das alle möglichen Sperrmechanismen zeigt. Sie können dieses Beispiel als Modell zum Erstellen eigener Sperrlisten verwenden.

Eine Sperrliste ist eine XML-Datei, die die XrML-Sprache verwendet.

Das BODY-Element enthält vier untergeordnete Elemente:

-   **ISSUEDTIME**. Enthält das Datum und die Uhrzeit der Ausstellung der Sperrliste. Dieses Element wird von „RLsigner.exe“ in die Datei eingefügt. Im Beispiel hier wird es nur angegeben, um die Gesamtstruktur der Sperrlistendatei zu zeigen.
-   **DESCRIPTOR**. Enthält Daten, die die Datei als Sperrliste identifizieren.
-   **ISSUER**. Enthält Daten zum Identifizieren der Entität, die die Sperrliste ausstellt.
-   **REVOCATIONLIST**. Enthält untergeordnete REVOKE-Elemente, die von dieser Liste gesperrte Entitäten angeben.

Ein Beispiel für eine Sperrlistendatei ist unten dargestellt.

| ![](images/Cc720208.note(WS.10).gif)Hinweis                                                                           |
|----------------------------------------------------------------------------------------------------------------------------------------------------|
        ```
| ![](images/Cc720208.Caution(WS.10).gif)Vorsicht                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie in der Sperrliste eine URL angeben, darf in RMS mit SP1 und RMS mit SP2 nicht mehr ein UNC-Pfad verwendet werden. Sie müssen zwingend eine URL angeben. |

Nachdem Sie die REVOKE-Elemente definiert haben, kann die Sperrliste signiert werden.

Verwenden des REVOKE-Elements
-----------------------------

In der Beispielsperrliste im Abschnitt „Beispiel für eine Sperrliste“ gibt jedes REVOKE-Element einen Prinzipal an, der zu sperren ist. Das öffnende Tag verfügt über Kategorie- und Typattribute, die definieren, was gesperrt wird und welches Kriterium für die Sperrung verwendet wird. Welche Elemente dem REVOKE-Element jeweils untergeordnet sind, hängt von der durch die Kategorie und die Typattribute angegebenen Aktion ab.

Weitere Informationen zum Angeben von REVOKE-Elementen finden Sie in den folgenden Beispielen:

-   [Sperren von Prinzipalen anhand eines öffentlichen Schlüssels](#bkmk_1)
-   [Sperren von Zertifikaten und Lizenzen anhand der GUID](#bkmk_2)
-   [Sperren von Zertifikaten und Lizenzen anhand des Hashwerts](#bkmk_3)
-   [Sperren von Zertifikaten und Lizenzen anhand des öffentlichen Schlüssels des Ausstellers](#bkmk_4)
-   [Sperren von Zertifikaten und Lizenzen anhand der Aussteller-ID](#bkmk_5)
-   [Sperren von Inhalten anhand der Inhalts-ID](#bkmk_6)
-   [Sperren von Prinzipalen anhand der Prinzipal-ID](#bkmk_10)
-   [Sperren von Prinzipalen anhand der Windows Live-ID](#bkmk_7)

<span id="BKMK_1"></span>
#### Sperren von Prinzipalen anhand eines öffentlichen Schlüssels

        ```

<span id="BKMK_2"></span>
#### Sperren von Zertifikaten und Lizenzen anhand der GUID

        ```
#### Sperren nach Anwendungsmanifest

Zum Sperren nach Anwendungsmanifest müssen Sie die Aussteller-ID, den öffentlichen Schlüssel des Ausstellers, die Lizenz-ID oder den Lizenz-Hash aus dem Anwendungsmanifest extrahieren. Anwendungsmanifeste sind jedoch Base-64-kodiert. Daher sind diese Informationen in einfacher Textform nicht verfügbar. Mit dem RMS-SDK kann ein Programm entwickelt werden, das die Methoden „DRMConstructCertificateChain“, „DRMDeconstructCertificateChain“ und „DRMDecode“ verwendet, um das Anwendungsmanifest zu dekodieren und die erforderlichen Informationen abzurufen.

Wenn Sie nicht möchten, dass eine bestimmte Anwendung durch Rechte geschützte Inhalte abrufen kann, sollten Sie mithilfe eines Anwendungsausschlusses verhindern, dass der RMS-Cluster dieser Anwendung Nutzungslizenzen erteilt. Ein Anwendungsausschluss kann jedoch nicht verhindern, dass ein Benutzer mit einer gültigen Nutzungslizenz durch Rechte geschützte Inhalte entschlüsselt. Weitere Informationen zum Anwendungsausschluss finden Sie weiter oben unter [Ausschließen von Anwendungen](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86).

<span id="BKMK_3"></span>
#### Sperren von Zertifikaten und Lizenzen anhand des Hashwerts

        ```
#### Sperren nach Anwendungsmanifest

Zum Sperren nach Anwendungsmanifest müssen Sie die Aussteller-ID, den öffentlichen Schlüssel des Ausstellers, die Lizenz-ID oder den Lizenz-Hash aus dem Anwendungsmanifest extrahieren. Anwendungsmanifeste sind jedoch Base-64-kodiert. Daher sind diese Informationen in einfacher Textform nicht verfügbar. Mit dem RMS-SDK kann ein Programm entwickelt werden, das die Methoden „DRMConstructCertificateChain“, „DRMDeconstructCertificateChain“ und „DRMDecode“ verwendet, um das Anwendungsmanifest zu dekodieren und die erforderlichen Informationen abzurufen.

Wenn Sie nicht möchten, dass eine bestimmte Anwendung durch Rechte geschützte Inhalte abrufen kann, sollten Sie mithilfe eines Anwendungsausschlusses verhindern, dass der RMS-Cluster dieser Anwendung Nutzungslizenzen erteilt. Ein Anwendungsausschluss kann jedoch nicht verhindern, dass ein Benutzer mit einer gültigen Nutzungslizenz RMS-geschützte Inhalte entschlüsselt. Weitere Informationen zum Anwendungsausschluss finden Sie weiter oben unter [Ausschließen von Anwendungen](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86).

<span id="BKMK_4"></span>
#### Sperren von Zertifikaten und Lizenzen anhand des öffentlichen Schlüssels des Ausstellers

        ```

<span id="BKMK_5"></span>
#### Sperren von Zertifikaten und Lizenzen anhand der Aussteller-ID

        ```
| ![](images/Cc720208.note(WS.10).gif)Hinweis                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Beim Angeben des ID-Typs muss dafür gesorgt werden, dass sich zwischen GUID und Schlusstag kein Zeilenumbruch befindet. Wird versehentlich ein Zeilenumbruch eingefügt, kann der RMS-Client die Sperrliste nicht analysieren. |

<span id="BKMK_6"></span>
#### Sperren von Inhalten anhand der Inhalts-ID

        ```
| ![](images/Cc720208.note(WS.10).gif)Hinweis                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Beim Angeben des ID-Typs muss dafür gesorgt werden, dass sich zwischen GUID und Schlusstag kein Zeilenumbruch befindet. Wird versehentlich ein Zeilenumbruch eingefügt, kann der RMS-Client die Sperrliste nicht analysieren. |

<span id="BKMK_10"></span>
#### Sperren von Prinzipalen anhand des Windows-Kontos

        ```
| ![](images/Cc720208.note(WS.10).gif)Hinweis                                                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Beim Angeben des ID-Typs muss dafür gesorgt werden, dass sich zwischen Sicherheitskennung (SID) des Windows-Kontos und Schlusstag kein Zeilenumbruch befindet. Wird versehentlich ein Zeilenumbruch eingefügt, kann der RMS-Client die Sperrliste nicht analysieren. |

<span id="BKMK_7"></span>
#### Sperren von Prinzipalen anhand der Windows Live-ID

        ```
| ![](images/Cc720208.note(WS.10).gif)Hinweis                                                                                                                                                                                    |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Beim Angeben des ID-Typs muss dafür gesorgt werden, dass sich zwischen PUID (Principal Unique Identifier) und Schlusstag kein Zeilenumbruch befindet. Wird versehentlich ein Zeilenumbruch eingefügt, kann der RMS-Client die Sperrliste nicht analysieren. |

<span id="BKMK_8"></span>
Einfügen einer Signatur in eine Sperrliste
------------------------------------------

Wenn Sie eine Sperrliste erstellt haben, müssen Sie in diese eine Signatur einfügen, wie in diesem Thema beschrieben. Dann können Sie die Sperrliste über die URL, die Sie in der zugehörigen Vorlage für Benutzerrechterichtlinien angegeben haben, den Benutzern zur Verfügung stellen.

Zum Einfügen einer Signatur müssen Sie zunächst mit dem „Sn.exe“ (Strong Name, Starker Name) ein Schlüsselpaar und eine Schlüsseldatei für die Sperrliste generieren. „Sn.exe“ ist Teil des Microsoft .NET Framework SDK 1.1, das auf der Microsoft-Website [http://go.microsoft.com/fwlink/?LinkId=104796](http://go.microsoft.com/fwlink/?linkid=104796) (möglicherweise in englischer Sprache) zum Herunterladen bereitsteht.

Ihre Sperrlistendatei muss als Unicode-Datei gespeichert worden sein, um sie mit „RLsigner.exe“ signieren zu können.

**So verwenden Sie „Sn.exe“, um ein neues Schlüsselpaar zu erzeugen und es in eine Datei zu schreiben**
1.  Erstellen Sie den privaten Schlüssel. Geben Sie dazu an einer Eingabeaufforderung den folgenden Befehl ein, und drücken Sie dann die EINGABETASTE:

    **sn -k** *Privater-Schlüssel-Datei***.snk**

    wobei *Privater-Schlüssel-Datei* der Name der Schlüsseldatei ist.

2.  Extrahieren Sie mithilfe von „Sn.exe“ aus der in Schritt 1 erstellten Schlüsselpaardatei den öffentlichen Schlüssel, und exportieren Sie ihn in eine separate Datei. Geben Sie den folgenden Befehl ein, und drücken Sie dann die EINGABETASTE:

    **sn -p** *Privater-Schlüssel-Datei Öffentlicher-Schlüssel-Datei*

    wobei *Privater-Schlüssel-Datei* der Name der in Schritt 1 erstellten Datei mit dem privaten Schlüssel und *Öffentlicher-Schlüssel-Datei* der Name der Datei ist, in der der exportierte öffentliche Schlüssel gespeichert wird.

3.  Ändern Sie die Erweiterung der (in Schritt 1) erstellten Datei mit dem privaten Schlüssel von SNK in DAT, damit die Datei für „RLsigner.exe“ verwendbar wird.

4.  Fügen Sie mit „RLsigner.exe“ eine Signatur in eine Sperrlistendatei ein. Dieses Tool ist in RMS enthalten. Standardmäßig befindet es sich im Verzeichnis „%systemdrive%\\Programme\\Windows Rights Management Services\\Tools“.

| ![](images/Cc720208.note(WS.10).gif)Hinweis |
|--------------------------------------------------------------------------|
| „RLsigner.exe“ unterstützt keine Dateinamen mit Leerzeichen.             |

<span id="BKMK_9"></span>
Verwenden von „RLsigner.exe“
----------------------------

Beim Ausführen von „RLsigner.exe“ erstellt das Tool zunächst unter Verwendung des privaten Schlüssels aus der Schlüsseldatei eine Signatur. Dann erstellt es eine Ausgabedatei, die auf der von Ihnen bereitgestellten Sperrlistendatei basiert.

| ![](images/Cc720208.Important(WS.10).gif)Wichtig   |
|---------------------------------------------------------------------------------|
| Dazu muss die Sperrlistendatei zuvor als Unicode-Datei gespeichert worden sein. |

Wenn Sie die Sperrliste mit „RLsigner.exe“ signieren möchten, geben Sie an einer Eingabeaufforderung den folgenden Befehl ein:

**rlsigner.exe** *Eingabedatei* **{-f** *Schlüsseldatei* **| -h** *Containername* **CSP}** *Ausgabedatei*

Verwenden Sie zur Vervollständigung der Eingabeparameter des Befehls die folgenden Informationen:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parameter</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><em>Eingabedatei</em></p></td>
<td style="border:1px solid black;"><p>Name der von Ihnen vorbereiteten XrML-konformen Sperrlistendatei</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><em>Schlüsseldatei</em></p></td>
<td style="border:1px solid black;"><p>Name der Datei, die den von Ihnen generierten öffentlichen und privaten Schlüssel enthält</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><em>Containername</em></p></td>
<td style="border:1px solid black;"><p>Name des Schlüsselcontainers</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><em>Ausgabedatei</em></p></td>
<td style="border:1px solid black;"><p>Name der signierten Sperrlistendatei, die mit dem Tool erstellt wird</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720208.note(WS.10).gif)Hinweis |  
|--------------------------------------------------------------------------|  
| „RLsigner.exe“ unterstützt keine Dateinamen mit Leerzeichen.             |
  
In den folgenden Beispielen wird beschrieben, wie Sie „RLsigner.exe“ an einer Eingabeaufforderung mit anderen Kryptographiedienstanbietern verwenden können:
  
-   Beispiel für eine Befehlszeilensyntax bei Verwendung einer Schlüsseldatei:  
    **rlsigner.exe rl.xml -f schluessel.dat ausgabe.xml**  
-   Beispiel für eine Befehlszeilensyntax bei Verwendung eines Hardwaresicherheitsmoduls:  
    **rlsigner.exe rl.xml -h Container CSP ausgabe.xml**
  
„RLsigner.exe“ stellt in seinem Rückgabecode grundlegende Informationen zu Fehlern und Erfolgen bereit. In der folgenden Tabelle werden die möglichen Rückgabecodes beschrieben.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Rückgabecode</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>0</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>-1</p></td>
<td style="border:1px solid black;"><p>Lesen der Quelldatei nicht möglich</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>-2</p></td>
<td style="border:1px solid black;"><p>Lesen der Schlüsseldatei nicht möglich</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>-3</p></td>
<td style="border:1px solid black;"><p>Ungültige Schlüsseldatei</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>-4</p></td>
<td style="border:1px solid black;"><p>Ungültige Quelldatei</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>-5</p></td>
<td style="border:1px solid black;"><p>Schreiben der Ausgabedatei nicht möglich</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>-6</p></td>
<td style="border:1px solid black;"><p>Unbekannter Fehler</p></td>
</tr>
</tbody>
</table>
  
Es empfiehlt sich möglicherweise, das automatische Signieren von Sperrlisten auf der Basis der von Ihnen für Ihren Server angegebenen Aktualisierungsrate einzurichten.
  
Sie können das Signieren von Sperrlisten mithilfe eines Skripts automatisieren. Das folgende VBScript-Beispielskript ruft „RLsigner.exe“ auf und schreibt die Ergebnisse in das Systemereignisprotokoll.
  
<codesnippet asp="http://msdn2.microsoft.com/asp" language displaylanguage="Visual Basic">const EVT\_SUCCESS = 0 const EVT\_ERROR = 1 const EVT\_WARNING = 2 const EVT\_INFORMATION = 4 const EVT\_AUDIT\_SUCCESS = 8 const EVT\_AUDIT\_FAILURE = 16 Dim WshShell, oExec Set WshShell = CreateObject( "WScript.Shell" ) Set oExec = WshShell.Exec("rlsigner.exe input\_file key\_file output\_file") Do While oExec.Status = 0 WScript.Sleep 100 Loop if WshShell.ExitCode &lt;&gt; 0 Then WshShell.LogEvent EVT\_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """" else WshShell.LogEvent EVT\_SUCCESS, "RLsigner completed successfully" end if  
```
