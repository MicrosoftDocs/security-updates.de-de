---
Title: Kapitel 6 - Richtlinie für Softwareeinschränkungen auf Windows XP-Clients
TOCTitle: Kapitel 6 - Richtlinie für Softwareeinschränkungen auf Windows XP-Clients
ms:assetid: 548c007a-7c26-44fd-8723-563a1f72f21e
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Cc163080(v=TechNet.10)
ms:contentKeyID: 20072366
---

# Windows XP-Sicherheitshandbuch


### Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients
Aktualisiert: 20.10.2005
 

#### Auf dieser Seite

[Überblick](#eeaa)  
[Architektur der Richtlinie für Softwareeinschränkungen](#edaa)  
[Optionen der Richtlinie für Softwareeinschränkungen](#ecaa)  
[Entwerfen und Bereitstellen von Richtlinien für Softwareeinschränkungen](#ebaa)  
[Zusammenfassung](#eaaa)  


### Überblick

Richtlinien für Softwareeinschränkungen bieten Administratoren die Möglichkeit, Software zu identifizieren und ihre Ausführung auf dem lokalen Computer zu kontrollieren. Mit diesem Programm können Computer, auf denen Microsoft® Windows® XP Professional ausgeführt wird, vor bekannten Problemen sowie schädlichen Programmen wie z. B. Viren und Trojanern geschützt werden. Richtlinien für Softwareeinschränkungen passen sich vollständig in den Active Directory®-Verzeichnisdienst und die Gruppenrichtlinien ein. Sie können auch auf eigenständigen Computern verwendet werden.

Aufgrund der Funktionsweise der Richtlinien für Softwareeinschränkungen ist dieses Kapitel anders aufgebaut als die vorherigen Kapitel dieses Handbuchs. Die vorherigen Kapitel enthalten Empfehlungen zur Konfiguration von Gruppenrichtlinieneinstellungen. Bei Richtlinien für Softwareeinschränkungen muss ein Administrator die Anwendungen definieren, die auf den Clientcomputern in Ihrer Umgebung ausgeführt werden dürfen. Anschließend wird die Richtlinie bestimmt, die auf die Clients angewendet wird.

Wenn Sie Richtlinien für Softwareeinschränkungen implementieren, müssen Sie zunächst entscheiden, ob Sie als Standardsicherheitsstufe **Nicht eingeschränkt** oder **Nicht erlaubt** wählen möchten. Wenn die Standardsicherheitsstufe **Nicht eingeschränkt** ist, wird jede Software zur Ausführung zugelassen, und Sie müssen zusätzliche Regeln konfigurieren, um bestimmte Anwendungen zu blockieren. Die sicherere Ansatz ist, die Standardsicherheitsstufe auf **Nicht erlaubt** zu setzen. Dies bedeutet, dass keine Software zur Ausführung zugelassen wird. Anschließend werden zusätzliche Regeln konfiguriert, um bestimmte Anwendungen zuzulassen. Mithilfe der domänenbasierten Gruppenrichtlinien können Sie Richtlinien zur Softwareeinschränkung auf mehrere Computer anwenden, und mithilfe der lokalen Gruppenrichtlinie können Sie die Einschränkungen auf einzelne Computer anwenden.

**Wichtig**: Sie sollten alle Richtlinieneinstellungen, die in diesem Handbuch erörtert werden, sorgfältig prüfen, bevor Sie sie in Produktionssystemen bereitstellen. Dies gilt insbesondere für Einstellungen für Richtlinien zur Softwareeinschränkung. Fehler im Entwurf oder der Implementierung dieser Funktion können für die Benutzer beträchtliche Probleme verursachen.

Die Richtlinie für Softwareeinschränkungen bietet verschiedene Verfahren zur Identifizierung von Software und eine auf Richtlinien beruhende Infrastruktur zur Durchsetzung der Regeln, mit denen die Art der Ausführung der identifizierten Software festgelegt wird. Computerbenutzer müssen sich an die Richtlinien halten, die vom Administrator in ihrer Umgebung in den Richtlinien für Softwareeinschränkungen eingerichtet werden.

Richtlinien für Softwareeinschränkungen können für folgende Aufgaben verwendet werden:
* Steuern der Möglichkeit, Software auf Clientcomputern in der Umgebung auszuführen

* Einschränken des Benutzerzugriffs auf bestimmte Dateien auf Computern mit mehreren Benutzern

* Festlegen der Personen, die Clientcomputern vertrauenswürdige Herausgeber hinzufügen dürfen

* Definieren des Gültigkeitsbereichs der Richtlinien – alle Benutzer oder eine Teilmenge der Benutzer oder Clientcomputer

* Verhindern der Ausführung ausführbarer Dateien auf den lokalen Computern mithilfe von Richtlinien, die auf einem Computer, einer Organisationseinheit, einer Website oder einer Domänenebene festgelegt sind

 
[Zum Seitenanfang](#mainsection)  



### Architektur der Richtlinie für Softwareeinschränkungen

Richtlinien für Softwareeinschränkungen bieten die folgenden leistungsfähigen Funktionen:
* **Erzwingen von Richtlinien, das entweder auf Domänen oder lokalen Computern beruht.** Administratoren erstellen die Richtlinie und definieren dann die vertrauenswürdigen und nicht vertrauenswürdigen Anwendungen. Die Richtlinie wird zur Laufzeit erzwungen, und Benutzer erhalten keine Aufforderungen, die es ihnen erlauben würden auszuwählen, ob ausführbare Dateien ausgeführt werden sollen.

* **Richtlinien, die nicht nur für binäre ausführbare Dateien gelten.**   Der Begriff der Software ist nicht eindeutig. Die Richtlinie für Softwareeinschränkungen ermöglicht die Steuerung von Microsoft Visual Basic® Scripting Edition (VBScript), JScript® und anderen Skriptsprachen. Sie ist zudem in die Windows Installer-Funktion integriert, um die Steuerung von Paketen zu ermöglichen, die auf Clientcomputern installiert werden können. Diese Funktion enthält eine API (Application Programming Interface, Anwendungsprogrammierschnittstelle), die zum Koordinieren der Richtlinienlaufzeit mit anderen Laufzeitmodulen verwendet werden kann.

* **Eine skalierbare Richtlinie.**   Da sie durch die Gruppenrichtlinie implementiert werden, können Richtlinien für Softwareeinschränkungen effektiv in Domänen implementiert und verwaltet werden, die zehntausende Computer umfassen.

* **Eine flexible Richtlinie.**   Administratoren haben die Möglichkeit, die Ausführung nicht autorisierter Skripts zu untersagen, Microsoft ActiveX®-Steuerelemente zu steuern oder Clientcomputer zu sperren.

* **Eine Richtlinie, die starke Kryptografie beim Identifizieren von Software verwendet.**   Richtlinien für Softwareeinschränkungen können Software mithilfe von Hashwerten oder digitalen Signaturen identifizieren.


Die Implementierung einer Richtlinie für Softwareeinschränkungen umfasst drei Phasen:
1. Der Administrator oder ein autorisierter Stellvertreter erstellt die Richtlinie mithilfe des Gruppenrichtlinien-Snap-Ins der MMC (Microsoft Management Console) für den Containerstandort, die Domäne oder Organisationseinheit in Active Directory. Microsoft empfiehlt, ein getrenntes Gruppenrichtlinienobjekt (GPO) für Richtlinien für Softwareeinschränkungen zu erstellen.

    **Hinweis**: Zum Erstellen einer neuen Richtlinie für Softwareeinschränkungen für einen lokalen eigenständigen Computer müssen Sie Mitglied der Gruppe **Administratoren** auf dem lokalen Computer sein. Um diese Richtlinieneinstellungen zu konfigurieren, klicken Sie auf **Windows-Einstellungen**, auf **Sicherheitseinstellungen** und dann auf **Richtlinie für Softwareeinschränkungen.**  

2. Die Richtlinie auf Computerebene wird heruntergeladen und tritt in Kraft, sobald Sie den Computer starten. Benutzerrichtlinien werden bei der Anmeldung des Benutzers am System oder an der Domäne wirksam. Führen Sie den Befehl **gpupdate.exe /force** aus, um die Richtlinie zu aktualisieren.

3. Wenn ein Benutzer eine ausführbare Datei wie z. B. eine Anwendung oder ein Skript startet, wird durch die Richtlinie bestimmt, ob die Ausführung entsprechend den Vorrangsregeln zulässig ist.

#### Einstellungen für nicht eingeschränkte oder nicht erlaubte Ausführung

Eine Richtlinie für Softwareeinschränkungen besteht aus zwei Teilen:
* Einer Standardregel für die Programme, die ausgeführt werden dürfen

* Einer Liste der Ausnahmen von dieser Standardregel


Sie können die Standardregel für die Identifizierung von Software auf **Nicht eingeschränkt** (d. h. wird ausgeführt) oder **Nicht erlaubt** (d. h. wird nicht ausgeführt) setzen.

Wenn die Standardregel auf **Nicht eingeschränkt** gesetzt wird, kann ein Administrator Ausnahmen definieren, d. h. eine Gruppe von Programmen, die nicht ausgeführt werden dürfen. Verwenden Sie die Standardeinstellung **Nicht eingeschränkt** in einer Umgebung mit weniger streng verwalteten Clientcomputern. Beispielsweise können Sie Benutzer daran hindern, ein Programm zu installieren, das zu Konflikten mit vorhandenen Programmen führt, indem Sie eine Blockierungsregel erstellen.

Eine höhere Sicherheit erreichen Sie, wenn Sie die Standardregel auf **Nicht erlaubt** setzen und dann nur die Ausführung einer bestimmten Gruppe von Programmen zulassen. Bei **Nicht erlaubt** als Standardeinstellung muss der Administrator alle Regeln für die einzelnen Anwendungen definieren und sicherstellen, dass Benutzer auf den Computern über die korrekten Sicherheitseinstellungen verfügen, um auf die zugelassenen Anwendungen zugreifen zu können. Die Standardeinstellung **Nicht erlaubt** ist der sicherere Ansatz für Organisationen, die Windows XP-Clientcomputer schützen möchten.


#### Vier Regeln zum Identifizieren von Software

Die Regeln in einer Richtlinie für Softwareeinschränkungen identifizieren eine oder mehrere Anwendungen und geben an, ob diese ausgeführt werden dürfen. Das Modul für das Erzwingen in Windows XP fragt die Regeln der Richtlinie ab, bevor Anwendungen ausgeführt werden dürfen. Zur Erstellung einer Richtlinie müssen Sie Anwendungen identifizieren und diese dann als Ausnahmen zur Standardeinstellung **Nicht erlaubt** angeben. Teil der Regeln können Kommentare sein, die den Zweck beschreiben.

Eine Richtlinie für Softwareeinschränkungen verwendet die folgenden vier Regeln für die Identifizierung von Software:
* **Hashregel.**   Verwendet einen kryptografischen Fingerabdruck der ausführbaren Datei.

* **Zertifikatsregel.**   Verwendet das digital signierte Zertifikat eines Softwareherausgebers für die.exe-Datei.

* **Pfadregel.**   Verwendet den lokalen, UNC- (Universal Naming Convention) oder Registrierungspfad des Speicherortes der.exe-Datei.

* **Zonenregel.**   Verwendet die Internetursprungszone der ausführbaren Datei (wenn die Datei mit Microsoft Internet Explorer heruntergeladen wurde).


##### Die Hashregel

Ein Hashwert ist ein digitaler Fingerabdruck, der ein Softwareprogramm oder eine ausführbare Datei eindeutig identifiziert, selbst wenn das Programm oder die ausführbare Datei verschoben oder umbenannt wird. Mithilfe eines Hashwertes können Administratoren eine bestimmte Version einer ausführbaren Datei oder eines Programms überwachen, die Benutzer nicht ausführen sollen.

Mithilfe einer Hashregel können Softwareprogramme eindeutig identifiziert werden, da die Prüfung durch die Hashregel auf einer kryptografischen Berechnung beruht, die den Inhalt der Datei berücksichtigt. Die Dateitypen, auf die sich Hashregeln auswirken, sind Abschnitt **Designierte Dateitypen** des Detailbereichs von **Richtlinien für Softwareeinschränkungen** aufgeführt.

Hashregeln sind in statischen Umgebungen effektiv. Wenn Software in Ihrer Umgebung aktualisiert wird, muss der Hashwert für jede aktualisierte ausführbare Datei neu berechnet werden. Hashregeln funktionieren sehr gut in Umgebungen, in denen die Software nur gelegentlich geändert oder aktualisiert wird.

Eine Hashregel besteht aus den folgenden drei Datenangaben, die durch Doppelpunkt getrennt werden:
* MD5- oder SHA-1-Hashwert

* Dateilänge

* ID des Hashalgorithmus


Digital signierte Dateien verwenden den in der Signatur enthaltenen MD5- oder SHA-1-Hashwert. Ausführbare Dateien, die nicht digital signiert sind, verwenden einen MD5-Hashwert.

Hashregeln werden wie folgt formatiert:

```
[MD5- oder SHA-1-Hashwert]:[Dateilänge]:[Hashalgorithmus-ID]

Die folgende Beispielhashregel bezeichnet eine Datei mit einer Länge von 126 Byte und einem Inhalt, der dem MD5-Hashwert (7bc04acc0d6480af862d22d724c3b049) und dem Hashalgorithmus mit der Hashalgorithmus-ID 32771 entspricht:

7bc04acc0d6480af862d22d724c3b049:126:32771
```

Für jede Datei, die der Administrator zulassen oder nicht zulassen möchte, muss eine Hashregel vorhanden sein. Wenn Software aktualisiert wird, muss der Administrator eine neue Hashregel für die einzelnen Anwendungen erstellen, da die Hashwerte der ursprünglichen ausführbaren Dateien nicht mit jenen der neuen Dateien übereinstimmen.

Führen Sie die im Folgenden beschriebenen Schritte aus, um eine Hashregel für eine ausführbare Datei zu erstellen.

**So erstellen Sie eine Hashregel für eine vorhandene ausführbare Datei**
1. Klicken Sie in der Symbolleiste des Gruppenrichtlinienobjekt-Editors auf **Windows-Einstellungen**, **Sicherheitseinstellungen**, **Richtlinien für Softwareeinschränkung**, und klicken Sie dann mit der rechten Maustaste auf **Zusätzliche Regeln.**  

2. Klicken Sie im Kontextmenü auf **Neue Hashregel.**  

    ![](images/cc163080.xpsg0601(de-de,technet.10).gif)

    **Abbildung 6.1: Dialogfeld „Neue Hashregel“**  
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0601_big(de-de,technet.10).gif)  

3. Klicken Sie auf **Durchsuchen**, um die Datei auszuwählen, für die Sie eine Hashregel erstellen möchten. Die ausführbare Datei in diesem Beispiel ist **Excel.exe.**   Der neue Dateihashwert wird im Feld **Dateihash:** angezeigt, und die Anwendungsversion im Feld **Dateiinformationen:.**  

4. Wählen Sie die für diese Regel gewünschte Standardeinstellung für die Sicherheitsstufe aus. Folgende Optionen stehen zur Auswahl:
    - **Nicht erlaubt**

    - **Nicht eingeschränkt**


##### Die Zertifikatsregel

Eine Zertifikatsregel gibt an, dass das Zertifikat eines Softwareherausgebers (das für die Codesignierung verwendet wird) vorhanden sein muss, bevor das Programm ausgeführt werden darf. Ein Administrator kann beispielsweise für alle Skripts und ActiveX-Steuerelemente signierte Zertifikate verlangen. Folgenden Quellen sind u. a. für die Zertifikatsregel zulässig:
* Eine kommerzielle Zertifizierungsstelle (Certificate Authority, CA), z. B. VeriSign

* Eine Microsoft Windows 2000- oder Windows Server 2003-PKI (Public Key Infrastructure, Infrastruktur öffentlicher Schlüssel)

* Ein selbstsigniertes Zertifikat


Eine Zertifikatsregel stellt ein starkes Verfahren der Softwareidentifizierung dar, da zum Prüfen der Dateien unabhängig vom Namen und Speicherort signierte Hashwerte verwendet werden, die in der Signatur der signierten Datei enthalten sind. Leider verwenden nur wenige Softwareanbieter Codesignierung. Selbst diejenigen, die es tun, signieren in der Regel nur einen kleinen Prozentsatz der von ihnen verteilten ausführbaren Dateien. Aus diesen Gründen werden Zertifikatsregeln im Allgemeinen für einige wenige spezielle Anwendungstypen wie z. B. ActiveX-Steuerelemente oder intern entwickelte Anwendungen verwendet. In diesem Handbuch wird Organisationen z. B. empfohlen, Skripts zur Verwaltung von Computern und Benutzern digital zu signieren, damit alle nicht signierten Skripts blockiert werden können. Mit einer Hashregel können Ausnahmen von einer Zertifikatsregel identifiziert werden.

##### Aktivieren von Zertifikatsregeln

Zertifikatsregeln sind standardmäßig nicht aktiviert. Führen Sie zum Aktivieren von Zertifikatsregeln die im Folgenden beschriebenen Schritte aus.

**So aktivieren Sie Zertifikatsregeln**
1. Öffnen Sie das Gruppenrichtlinienobjekt im Gruppenrichtlinienobjekt-Editor.

2. Klicken Sie in der Konsolenstruktur auf **Sicherheitsoptionen.**  

3. Doppelklicken Sie im Detailbereich auf **Systemeinstellungen: Zertifikatsregeln zur Durchsetzung von Softwareeinschränkungsrichtlinien auf Windows-Programme anwenden.**  

4. Klicken Sie auf **Aktiviert**, um die Zertifikatsregeln verfügbar zu machen.


Ausführliche Anweisungen zum digitalen Signieren von Dateien finden Sie im Abschnitt „Handbuch zum Digitalen Signieren von Dateien mit Testzertifikaten“ in „[Verwendung von Richtlinien für Softwareeinschränkungen zum Schutz vor nicht autorisierter Software](http://www.microsoft.com/technet/prodtechnol/winxppro/maintain/rstrplcy.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/winxppro/maintain/rstrplcy.mspx.

Viele kommerzielle Websites lassen ihren Softwarecode von einer kommerziellen Zertifizierungsstelle signieren. Die Gültigkeit dieser Zertifikate liegt meist zwischen einem und mehreren Jahren. Achten Sie bei der Verwendung von Zertifikatsregeln auf das Ablaufdatum der Zertifikate. Möglicherweise können Sie sich an den Softwareherausgeber wenden, um weitere Informationen zum Gültigkeitszeitraum der herausgegebenen Zertifikate zu erhalten. Wenn Sie ein Zertifikat von einer kommerziellen Zertifizierungsstelle erhalten, können Sie es zum Erstellen einer Zertifikatsregel in eine Datei exportieren. Führen Sie zum Exportieren eines Zertifikats die im Folgenden beschriebenen Schritte aus.

**So exportieren Sie ein Zertifikat**
1. Wählen Sie den vertrauenswürdigen Herausgeber aus, der das Zertifikat herausgibt. In diesem Beispiel lautet der Herausgeber des Zertifikats Microsoft MSN®.

    ![](images/cc163080.xpsg0602(de-de,technet.10).jpg)

    **Abbildung 6.2: Dialogfeld „Sicherheitswarnung“, in dem der vertrauenswürdige Herausgeber angezeigt wird**  
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0602_big(de-de,technet.10).jpg)  

2. Klicken Sie auf die Registerkarte **Details** und dann auf **In Datei kopieren...**, um dieses Zertifikat in eine Datei zu kopieren und damit eine Zertifikatsregel zu erstellen.

    ![](images/cc163080.xpsg0603(de-de,technet.10).jpg)

    **Abbildung 6.3: Registerkarte „Details“ im Dialogfeld „Zertifikat“**  
    Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0603_big(de-de,technet.10).jpg)  

3. Die Willkommensseite des **Zertifikatsexport-Assistenten** wird angezeigt. Klicken Sie auf **Weiter**, um den Vorgang fortzusetzen.

    ![](images/cc163080.xpsg0604(de-de,technet.10).jpg)

    **Abbildung 6.4: Willkommenseite des Zertifikatexport-Assistenten**    
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0604_big(de-de,technet.10).jpg)  

4. Wählen Sie auf der Seite **Exportdateiformat** die Option **DER-codiert-binär X.509 (.CER)** aus, und klicken Sie auf **Weiter**, um die Zertifikatdatei mit der Erweiterung.cer zu erstellen.

    ![](images/cc163080.xpsg0605(de-de,technet.10).jpg)

    **Abbildung 6.5: Seite „Exportdateiformat“ des Zertifikatexport-Assistenten mit der ausgewählten Codierungsmethode**  
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0605_big(de-de,technet.10).jpg)  

5. Geben Sie auf der Seite **Exportdatei** einen beschreibenden Namen für die Zertifikatsregeldatei ein. Sie können das Zertifikat an einem beliebigen Speicherort unter einem beliebigen Dateinamen speichern.

    ![](images/cc163080.xpsg0606(de-de,technet.10).jpg)

    **Abbildung 6.6: Seite „Exportdatei“ des Zertifikatexport-Assistenten mit einem Beispieldateinamen**  
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0606_big(de-de,technet.10).jpg)  

6. Die Seite **Fertigstellen des Assistenten** wird mit den ausgewählten Einstellungen der Zertifikatdatei angezeigt. Überprüfen Sie die Einstellungen, und klicken Sie zum Exportieren der Datei auf **Fertig stellen.**  

    ![](images/cc163080.xpsg0607(de-de,technet.10).jpg)

    **Abbildung 6.7: Seite „Fertigstellen des Assistenten“ mit den ausgewählten Einstellungen**  
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0607_big(de-de,technet.10).jpg)  


##### Die Pfadregel

Eine Pfadregel gibt entweder einen Ordner oder den vollständigen Pfad zu einem Programm an. Wenn durch eine Pfadregel ein Ordner angegeben wird, trifft sie auf alle Programme zu, die sich in diesem Ordner und den entsprechenden Unterordnern befinden. Pfadregeln unterstützen lokale Pfade und UNC-Pfade.

Der Administrator muss in der Pfadregel alle Verzeichnisse definieren, von denen aus eine bestimmte Anwendung gestartet werden kann. Wenn eine Anwendung z. B. mit einer Desktopverknüpfung gestartet wird, muss die Pfadregel sowohl die ausführbare Datei als auch die Verknüpfungspfade für das Ausführen der Anwendung angeben. Wenn ein Benutzer versucht, eine Anwendung mit einer unvollständigen Pfadregel auszuführen, wird die Warnung **Software eingeschränkt** angezeigt.

Bei der Installation von Dateien auf der Festplatte von Windows XP-basierten Computern verwenden viele Anwendungen die Variable *%ProgramFiles%*. Leider sind einige Anwendungen darauf programmiert, Dateien in das Unterverzeichnis **C:\Programme** zu kopieren, und tun dies selbst dann, wenn diese Variable auf ein anderes Verzeichnis in einem anderen Laufwerk gesetzt wird. Denken Sie an diese Beschränkung, wenn Sie Pfadregeln erstellen und testen.

##### Verwenden von Umgebungsvariablen in Pfadregeln

Bei der Definition einer Pfadregel können Sie Umgebungsvariablen verwenden. Da Pfadregeln in der Clientumgebung ausgewertet werden, ermöglicht die Verwendung von Umgebungsvariablen, eine Regel an die Umgebung eines bestimmten Benutzers anzupassen.

Die folgenden beiden Beispiele veranschaulichen die Anwendung von Umgebungsvariablen auf eine Pfadregel.
* „%UserProfile%“ entspricht **C:\Dokumente und Einstellungen\*****&lt;Benutzer&gt;*** und allen Unterordnern dieses Verzeichnisses.

* „%ProgramFiles%\*&lt;Anwendung&gt;*“ entspricht **C:\Programme\*****&lt;Anwendung&gt;*** und allen Unterordnern dieses Verzeichnisses.

    **Hinweis**: Umgebungsvariablen werden nicht durch Zugriffssteuerungslisten (Access Control Lists, ACLs) geschützt. Es werden zwei Arten von Umgebungsvariablen unterschieden: **Benutzervariablen** und **Systemvariablen.**   Benutzer, die eine Eingabeaufforderung öffnen dürfen, können die Umgebungsvariable **Benutzer** mit einem anderen Pfad neu definieren. Die Umgebungsvariable **System** können nur Benutzer ändern, die Mitglied der Gruppe **Administratoren** sind.


Obwohl die beiden obigen Beispiele sehr nützlich sind, sollten Sie auch andere verfügbare Umgebungsvariablen in Erwägung ziehen. Eine vollständige Liste finden Sie in „[Überblick über Command Shell](http://www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/ntcmds_shelloverview.mspx)“ (in englischer Sprache) unter www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/ntcmds_shelloverview.mspx.

##### Verwenden von Platzhaltern in Pfadregeln

In einer Pfadregel können die Platzhalter „?“ und „*“ verwendet werden. Die folgenden Beispiele veranschaulichen die Anwendung von Platzhaltern auf verschiedene Pfadregeln:
* **\\DC – ??\login$** entspricht **\\DC – 01\login$**, **\\DC – 02\login$** und so weiter.

* ***\Windows** entspricht **C:\Windows**, **D:\Windows**, **E:\Windows** und allen Unterordnern der jeweiligen Verzeichnisse.

* **C:\win*** entspricht **C:\winnt**, **C:\windows**, **C:\windir** und allen Unterordnern der jeweiligen Verzeichnisse.

* *.**  vbs** entspricht allen Anwendungen in Windows XP Professional mit dieser Erweiterung.

* **C:\Anwendungsdateien\*.*** entspricht allen Anwendungsdateien im angegebenen Unterverzeichnis.


Registrierungspfadregeln

Viele Anwendungen speichern Pfade zu ihren Installationsordnern oder Anwendungsverzeichnissen in der Microsoft Windows-Registrierung. Einige Anwendungen können an beliebigen Speicherorten im Dateisystem installiert werden. Um diese zu suchen, können Sie eine Pfadregel zur Ermittlung der entsprechenden Registrierungsschlüssel erstellen.

Diese Speicherorte können möglicherweise nicht einfach mithilfe bestimmter Ordnerpfade wie **C:\Programme\Microsoft Platform SDK** oder Umgebungsvariablen wie **%ProgramFiles%\Microsoft Platform SDK** bestimmt werden. Wenn das Programm seine Anwendungsverzeichnisse in der Registrierung speichert, können Sie eine Pfadregel speichern, die den in der Registrierung gespeicherten Wert verwendet, wie z. B.:

**%HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\PlatformSDK\Directories\**  
**Install Dir%**

Diese Art von Pfadregel, die als Registrierungspfadregel bezeichnet wird, hat folgendes Format:

*%&lt;Registrierungsstruktur&gt;\\ &lt;Registrierungsschlüssel&gt;\\ &lt;Wertname&gt;*%

**Hinweis**: Das Suffix einer Registrierungspfadregel darf innerhalb der Regel unmittelbar nach dem letzten %-Zeichen kein \-Zeichen aufweisen. Für die Registrierungsstruktur muss der vollständige Name angegeben werden, Abkürzungen funktionieren nicht.

Wenn die Standardregel auf **Nicht erlaubt** gesetzt ist, werden vier Registrierungspfadregeln eingerichtet, sodass das Betriebssystem Zugriff auf Systemdateien hat. Diese Registrierungspfadregeln werden als Sicherheitsvorkehrung erstellt – damit Sie sich selbst und andere Benutzer nicht aus dem System aussperren können – und sind auf **Nicht eingeschränkt** gesetzt. Diese Regeln sollten nur von fortgeschrittenen Benutzern geändert oder gelöscht werden. Die Einstellungen für die Registrierungspfadregeln lauten wie folgt:
* %HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\  
CurrentVersion\SystemRoot%

* %HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\  
CurrentVersion\SystemRoot%\*.exe

* %HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\  
CurrentVersion\SystemRoot%\System32\*.exe

* %HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\  
CurrentVersion\ProgramFilesDir%


##### Vorrang bei Pfadregeln

Wenn mehrere Pfadregeln zutreffen, hat die am engsten gefasste Regel Vorrang vor den anderen Regeln. Die folgende Gruppe von Pfaden ist in der Reihenfolge vom höchsten Vorrang (genaueste Übereinstimmung) zum niedrigsten Vorrang (allgemeinste Übereinstimmung) angeordnet:
* Laufwerk:\Ordner1\Ordner2\Dateiname.Erweiterung

* Laufwerk:\Ordner1\Ordner2\*.Erweiterung

* *.Erweiterung

* Laufwerk:\Ordner1\Ordner2\

* Laufwerk:\Ordner1\


##### Zonenregel

Mit einer Zonenregel können Sie Software identifizieren, die aus einer der folgenden in Internet Explorer definierten Zonen heruntergeladen wurde:
* Internet

* Intranet

* Eingeschränkte Sites

* Vertrauenswürdige Sites

* Arbeitsplatz


Die aktuelle Version der Internetzonenregel gilt nur für Windows Installer-Pakete (*.msi). Außerdem gilt diese Regel nicht für über Internet Explorer heruntergeladene Software. Alle anderen Dateitypen, auf die sich Zonenregeln auswirken, sind in der Tabelle mit designierten Dateitypen weiter unten in diesem Kapitel aufgeführt. Es gibt nur eine Liste designierter Dateitypen, die von allen Zonenregeln verwendet wird.

##### Empfehlungen für Regeln

Bestimmen Sie anhand der Informationen in der folgenden Tabelle, welche Pfadregel sich am besten für die Benutzer und die Umgebung einer Anwendung eignet.

**Tabelle 6.1: Bestimmen der besten Regel für eine bestimmte Anwendung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Aufgabe

</th>

<th style="border:1px solid black;">

Empfohlene Regel

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Zulassen oder nicht zulassen einer bestimmten Programmversion.

</td>

<td style="border:1px solid black;">


**Hashregel**  
Wählen Sie die Datei zum Erstellen eines Hashwertes aus.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Identifizieren eines Programms, das immer am gleichen Speicherort installiert ist.

</td>

<td style="border:1px solid black;">


**Pfadregel mit Umgebungsvariablen**  
%ProgramFiles%\Internet Explorer\iexplore.exe

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Identifizieren eines Programms, das an einem beliebigen Speicherort auf Clientcomputern installiert werden kann.

</td>

<td style="border:1px solid black;">


**Registrierungspfadregeln**  
%HKEY_LOCAL_MACHINE\SOFTWARE\ ComputerAssociates\InoculateIT\6.0\Path\HOME%

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Identifizieren einer Gruppe von Skripts auf einem zentralen Server.

</td>

<td style="border:1px solid black;">


**Pfadregel**  
\\\SERVER_NAME\Share

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Identifizieren einer Gruppe von Skripts auf einer Gruppe von Servern. Beispielsweise DC01, DC02 und DC03.

</td>

<td style="border:1px solid black;">


**Pfadregel mit Platzhalter**  
\\\DC??\Share

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Keine.vbs-Dateien erlauben, mit Ausnahme der Dateien in einem Anmeldeskriptverzeichnis.

</td>

<td style="border:1px solid black;">


**Pfadregel mit Platzhalter**  

\*.VBS auf **Nicht erlaubt** gesetzt

\\\LOGIN_SRV\Share\*.VBS auf **Nicht eingeschränkt** gesetzt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Eine Datei mit dem Namen Flcss.exe nicht erlauben, da diese nur von einem Virus installiert wird.

</td>

<td style="border:1px solid black;">


**Pfadregel**

Flcss.exe auf **Nicht erlaubt** gesetzt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Identifizieren einer Gruppe von Skripts, die an beliebigen Speicherorten ausgeführt werden können.

</td>

<td style="border:1px solid black;">


**Zertifikatsregel**

Verwenden Sie ein Zertifikat, um die Skripts digital zu signieren.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zulassen von Software, die von Websites in der vertrauenswürdigen Internetzone installiert wird.

</td>

<td style="border:1px solid black;">


**Zonenregel**

**Vertrauenswürdige Sites** auf **Nicht eingeschränkt** setzen.

</td>

</tr>

</table>


##### Vorrang von Regeln der Richtlinie für Softwareeinschränkungen

Regeln werden in einer bestimmten Reihenfolge ausgewertet. Regeln, denen ein Programm genauer entspricht, haben gegenüber Regeln Vorrang, denen das gleiche Programm weniger exakt entspricht. Wenn zwei identische Regeln mit unterschiedlichen Sicherheitsstufen für die gleiche Software festgelegt wurden, hat die Regel mit der höchsten Sicherheitsstufe Vorrang. Wenn z. B. zwei Hashregeln, von denen eine die Sicherheitsstufe **Nicht erlaubt** und die andere die Sicherheitsstufe **Nicht eingeschränkt** aufweist, auf das gleiche Softwareprogramm angewendet werden, hat die Regel mit der Sicherheitsstufe **Nicht erlaubt** Vorrang, und das Programm wird nicht ausgeführt. In der folgenden Liste wird die Vorrangsreihenfolge für Regeln von der genauesten zur am wenigsten genauen Regel definiert:

1. Hashregel

2. Zertifikatsregel

3. Pfadregel

4. Zonenregel

5. Standardregel

[Zum Seitenanfang](#mainsection)  

### Optionen der Richtlinie für Softwareeinschränkungen

In diesem Abschnitt werden die unterschiedlichen Erzwingungsoptionen behandelt, die Einfluss auf die Funktionsweise einer Richtlinie für Softwareeinschränkungen haben. Diese Optionen ändern die Art und Weise der Erzwingung von Microsoft Authenticode®-Vertrauenseinstellungen für digital signierte Dateien. Zwei Erzwingungsoptionen sind verfügbar: DLL-Prüfung (Dynamic Link Library) und Überspringen von Administratoren.


#### DLL-Prüfung

Viele Programme bestehen aus einer ausführbaren Datei und vielen Hilfs-DLLs. Standardmäßig werden Regeln einer Richtlinie für Softwareeinschränkungen nicht für DLLs erzwungen. Diese Option wird für die meisten Kunden aus den folgenden drei Gründen empfohlen:
* Wenn die Ausführung der ausführbaren Hauptdatei nicht erlaubt ist, kann das Programm nicht ausgeführt werden. Es ist also nicht erforderlich, die Ausführung der zugehörigen DLLs zu verweigern.

* Durch die DLL-Prüfung verringert sich die Systemleistung, da alle Bibliotheken überprüft werden müssen, die mit der Anwendung verknüpft sind. Wenn ein Benutzer z. B. während einer Anmeldesitzung zehn Programme ausführt, wertet die Richtlinie für Softwareeinschränkungen jedes einzelne Programm aus. Bei aktivierter DLL-Prüfung wertet die Richtlinie für Softwareeinschränkungen jede DLL aus, die in die einzelnen Programme geladen wird. Wenn jedes Programm 20 DLLs verwendet, ergeben sich daraus 10 Prüfungen von ausführbaren Programmen plus 200 DLL-Prüfungen. Die Richtlinie für Softwareeinschränkungen muss somit 210 Auswertungen durchführen.

    Ein Programm wie Internet Explorer besteht aus der ausführbaren Datei iexplore.exe und vielen Hilfs-DLLs.

* Wenn die Standardsicherheitsstufe auf **Nicht erlaubt** gesetzt ist, wird das System gezwungen, nicht nur die ausführbare Hauptdatei zu identifizieren, bevor diese ausgeführt werden darf, sondern auch alle zugehörigen DLLs der.exe-Datei, wodurch das System zusätzlich belastet wird.


Viren greifen zwar hauptsächlich ausführbare Dateien an, manche sind sich jedoch gegen DLLs gerichtet. Aus diesem Grund wird die Option „DLL-Prüfung“ empfohlen, wenn die höchstmögliche Sicherheit für die in der Umgebung ausgeführten Programme gewünscht wird.

Um sicherzustellen, dass ein Programm keine Viren enthält, können Sie eine Gruppe von Hashregeln verwenden, die die ausführbare Datei und alle zugehörigen DLLs identifizieren.

**So deaktivieren Sie die Option für die DLL-Prüfung**
* Wenn Sie eine Richtlinie für Softwareeinschränkungen bearbeiten, wählen Sie im Dialogfeld **Eigenschaften von Erzwingen** die Option **Alle Softwaredateien außer Bibliotheken (z. B. DLLs)** aus, wie in der folgenden Abbildung dargestellt:

    ![](images/cc163080.xpsg0608(de-de,technet.10).jpg)

    **Abbildung 6.8: Dialogfeld „Eigenschaften von Erzwingen“ mit Datei- und Benutzererzwingungsoptionen**  
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0608_big(de-de,technet.10).jpg)  



#### Überspringen von Administratoren

Unter Umständen möchte ein Administrator die Ausführung von Programmen für die meisten Benutzer verhindern, Administratoren aber die Ausführung aller Programme erlauben. Ein Administrator verfügt z. B. über einen freigegebenen Computer, mit dem mehrere Benutzer über den Terminalserver eine Verbindung herstellen. Der Administrator möchte Benutzer nur die Ausführung bestimmter Anwendungen auf dem Computer erlauben, Mitglieder der lokalen Gruppe **Administratoren** sollen jedoch beliebige Anwendungen ausführen dürfen. Verwenden Sie hierzu die Erzwingungsoption zum **Überspringen von Administratoren.**  

Wenn die Richtlinie für Softwareeinschränkungen in einem Gruppenrichtlinienobjekt erstellt wird, das mit einem Objekt in Active Directory verknüpft ist, empfiehlt Microsoft, nicht die Option zum **Überspringen von Administratoren** zu verwenden und der Gruppe **Administratoren** die Berechtigung **Gruppenrichtlinie übernehmen** für das Gruppenrichtlinienobjekt zu verweigern. Hierdurch wird weniger Netzwerkbandbreite in Anspruch genommen, da die Einstellungen des Gruppenrichtlinienobjekts, die nicht für Administratoren gelten, nicht heruntergeladen werden.

**Hinweis**: In lokalen Sicherheitsrichtlinien definierte Richtlinien für Softwareeinschränkungen können keine Benutzergruppen filtern. Aus diesem Grund ist die Option **Überspringen von Administratoren** erforderlich.

**So aktivieren Sie die Option zum Überspringen von Administratoren**
* Wählen Sie in dem in Abbildung 6.8 dargestellten Dialogfeld **Eigenschaften von Erzwingen** die Option **Alle Benutzer außer den lokalen Administratoren** aus.


##### Definieren von ausführbaren Dateien

In dem in der folgenden Abbildung dargestellten Dialogfeld **Eigenschaften von Designierte Dateitypen** werden die Dateitypen aufgeführt, die durch die Richtlinie für Softwareeinschränkungen gesteuert werden. Diese Dateitypen werden als ausführbare Dateien betrachtet. Beispielsweise gilt eine Bildschirmschonerdatei (.scr) als ausführbare Datei, da sie als Programm geladen wird, wenn Sie in Windows Explorer darauf doppelklicken.

Die Regeln der Richtlinie für Softwareeinschränkungen gelten nur für die Dateitypen, die im Dialogfeld **Eigenschaften von Designierte Dateitypen** aufgeführt werden. Wenn in der Umgebung ein Dateityp verwendet wird, auf den Sie die Regeln anwenden möchten, fügen Sie ihn der Liste hinzu. Beispielsweise würden Sie bei Perl-Skriptdateien den Dateityp .pl und weitere Dateitypen, die dem Perl-Modul zugeordnet sind, der Liste **Designierte Dateitypen:** auf der Registerkarte **Allgemein** des Dialogfelds **Eigenschaften von Designierte Dateitypen** hinzufügen.

![](images/cc163080.xpsg0609(de-de,technet.10).jpg)

**Abbildung 6.9: Dialogfeld „Eigenschaften von Designierte Dateitypen“**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0609_big(de-de,technet.10).jpg)  

Bei dem in diesem Handbuch definierten Entwurf eines Gruppenrichtlinienobjekts werden die Dateitypen.mdb und.lnk entfernt und der Dateityp.ocx hinzugefügt. In der folgenden Tabelle werden die designierten Dateitypen aufgeführt.

**Tabelle 6.2: Designierte Dateitypen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Dateierweiterung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

<th style="border:1px solid black;">

Dateierweiterung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


.ade

</td>

<td style="border:1px solid black;">


Microsoft Access-Projekterweiterung

</td>

<td style="border:1px solid black;">


.msc

</td>

<td style="border:1px solid black;">


Microsoft Common Console-Dokument

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.adp

</td>

<td style="border:1px solid black;">


Microsoft Access-Projekt

</td>

<td style="border:1px solid black;">


.msi

</td>

<td style="border:1px solid black;">


Windows Installer-Paket

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.bas

</td>

<td style="border:1px solid black;">


Visual Basic-Klassenmodul

</td>

<td style="border:1px solid black;">


.msp

</td>

<td style="border:1px solid black;">


Windows Installer-Patch

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.bat

</td>

<td style="border:1px solid black;">


Batchdatei

</td>

<td style="border:1px solid black;">


.mst

</td>

<td style="border:1px solid black;">


Visual Test-Quelldatei

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.chm

</td>

<td style="border:1px solid black;">


Kompilierte HTML-Hilfedatei

</td>

<td style="border:1px solid black;">


.ocx

</td>

<td style="border:1px solid black;">


ActiveX-Steuerelement

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.cmd

</td>

<td style="border:1px solid black;">


Windows NT-Befehlsskript

</td>

<td style="border:1px solid black;">


.pcd

</td>

<td style="border:1px solid black;">


Photo CD-Bild

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.com

</td>

<td style="border:1px solid black;">


MS-DOS-Anwendung

</td>

<td style="border:1px solid black;">


.pif

</td>

<td style="border:1px solid black;">


Verknüpfung mit MS-DOS-Programm

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.cpl

</td>

<td style="border:1px solid black;">


Systemsteuerungsoption

</td>

<td style="border:1px solid black;">


.reg

</td>

<td style="border:1px solid black;">


Registrierungseintrag

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.crt

</td>

<td style="border:1px solid black;">


Sicherheitszertifikat

</td>

<td style="border:1px solid black;">


.scr

</td>

<td style="border:1px solid black;">


Bildschirmschoner

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.exe

</td>

<td style="border:1px solid black;">


Anwendung

</td>

<td style="border:1px solid black;">


.sct

</td>

<td style="border:1px solid black;">


Windows-Skriptkomponente

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.hlp

</td>

<td style="border:1px solid black;">


Windows-Hilfedatei

</td>

<td style="border:1px solid black;">


.shs

</td>

<td style="border:1px solid black;">


Shell-Datenauszug

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.hta

</td>

<td style="border:1px solid black;">


HTML-Anwendung

</td>

<td style="border:1px solid black;">


.url

</td>

<td style="border:1px solid black;">


Internetverknüpfung (Uniform Resource Locator, URL)

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.inf

</td>

<td style="border:1px solid black;">


Setupinformationsdatei

</td>

<td style="border:1px solid black;">


.vb

</td>

<td style="border:1px solid black;">


Visual Basic-Datei

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.ins

</td>

<td style="border:1px solid black;">


Internetkommunikationseinstellung

</td>

<td style="border:1px solid black;">


.vbe

</td>

<td style="border:1px solid black;">


Codierte VBScript-Skriptdatei

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.isp

</td>

<td style="border:1px solid black;">


Internetkommunikationseinstellung

</td>

<td style="border:1px solid black;">


.vbs

</td>

<td style="border:1px solid black;">


VBScript-Skriptdatei

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.js

</td>

<td style="border:1px solid black;">


JScript-Datei

</td>

<td style="border:1px solid black;">


.wsc

</td>

<td style="border:1px solid black;">


Windows-Skriptkomponente

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.jse

</td>

<td style="border:1px solid black;">


Codierte JScript-Skriptdatei

</td>

<td style="border:1px solid black;">


.wsf

</td>

<td style="border:1px solid black;">


Windows-Skriptdatei

</td>

</tr>

<tr>

<td style="border:1px solid black;">


.mde

</td>

<td style="border:1px solid black;">


Microsoft Access-MDE-Datenbank

</td>

<td style="border:1px solid black;">


.wsh

</td>

<td style="border:1px solid black;">


Windows Scripting Host-Einstellungsdatei

</td>

</tr>

</table>


##### Vertrauenswürdige Herausgeber

Sie können das Dialogfeld **Eigenschaften von Vertrauenswürdigen Herausgebern** verwenden, um festzulegen, welche Benutzer vertrauenswürdige Herausgeber auswählen können. Sie können auch bestimmen, welche Zertifikatssperrungsprüfungen ggf. durchgeführt werden, bevor ein Herausgeber als vertrauenswürdig eingestuft wird. Bei aktivierten Zertifikatsregeln wird durch Richtlinien für Softwareeinschränkungen eine Zertifikatssperrliste geprüft, um die Gültigkeit des Zertifikats und der Signatur der Software sicherzustellen. Durch diesen Vorgang kann jedoch beim Starten von Programmen die Systemleistung verringert werden.

Mit den Optionen auf der in der folgenden Abbildung dargestellten Registerkarte **Allgemein** des Dialogfelds **Eigenschaften von Vertrauenswürdigen Herausgebern** können Sie Einstellungen für ActiveX-Steuerelemente und andere signierte Inhalte konfigurieren.

![](images/cc163080.xpsg0610(de-de,technet.10).jpg)

**Abbildung 6.10: Dialogfeld „Eigenschaften von Vertrauenswürdigen Herausgebern“**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163080.xpsg0610_big(de-de,technet.10).jpg)  

In der folgenden Tabelle werden die Optionen für vertrauenswürdige Herausgeber in Bezug auf ActiveX-Steuerelemente und andere signierte Inhalte aufgeführt.

**Tabelle 6.3: Aufgaben und Einstellungen für vertrauenswürdige Herausgeber**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellungsname

</th>

<th style="border:1px solid black;">

Aufgabe

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Unternehmensadministratoren

</td>

<td style="border:1px solid black;">


Verwenden Sie diese Einstellung, um nur Unternehmensadministratoren zu erlauben, Entscheidungen zu signierten aktiven Inhalten zu treffen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Administratoren des lokalen Computers

</td>

<td style="border:1px solid black;">


Verwenden Sie diese Einstellung, um Administratoren des lokalen Computers zu erlauben, alle Entscheidungen zu signierten aktiven Inhalten zu treffen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Endbenutzer

</td>

<td style="border:1px solid black;">


Verwenden Sie diese Einstellung, um Benutzern zu erlauben, Entscheidungen zu signierten aktiven Inhalten zu treffen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Herausgeber

</td>

<td style="border:1px solid black;">


Verwenden Sie diese Einstellung, um sicherzustellen, dass das Zertifikat des Softwareherausgebers nicht gesperrt wurde.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zeitstempel

</td>

<td style="border:1px solid black;">


Verwenden Sie diese Einstellung, um sicherzustellen, dass das von der Organisation für den Zeitstempel der aktiven Inhalte verwendete Zertifikat nicht gesperrt wurde.

</td>

</tr>

</table>

 
[Zum Seitenanfang](#mainsection)  


### Entwerfen und Bereitstellen von Richtlinien für Softwareeinschränkungen

In diesem Abschnitt wird beschrieben, wie Richtlinien für Softwareeinschränkungen mithilfe des Gruppenrichtlinien-Snap-Ins verwaltet werden, was bei der erstmaligen Bearbeitung einer Richtlinie zu berücksichtigen ist und wie eine Richtlinie für Softwareeinschränkungen auf eine Gruppe von Benutzern angewendet wird. Außerdem werden verschiedene Aspekte erörtert, die mit der Bereitstellung einer Richtlinie für Softwareeinschränkungen in Zusammenhang stehen.


#### Integration in Gruppenrichtlinien

Sie können eine Richtlinie für Softwareeinschränkungen mithilfe des Gruppenrichtlinien-Snap-Ins für eine Gruppe von Clientcomputern sowie für alle Benutzer verwalten, die sich bei den Computern anmelden. Die Richtlinie wird auf die die in diesem Handbuch definierten Organisationseinheiten „Desktop“ und „Laptop“ angewendet.

##### Domäne

Der Administrator sollte für die Richtlinie für Softwareeinschränkungen ein eigenes Gruppenrichtlinienobjekt erstellen. So lässt sich die Gruppenrichtlinie deaktivieren, ohne andere auf das Objekt angewendete Richtlinien zu beeinträchtigen, wenn unerwartete Probleme auftreten sollten.

##### Lokal

Für die eigenständigen Clientcomputer in der Umgebung sollte eine lokale Richtlinie konfiguriert werden. Dieser Vorgang wird in diesem Handbuch in Kapitel 5, „Schützen eigenständiger Windows XP-Clients“, beschrieben.


#### Entwerfen einer Richtlinie

In diesem Abschnitt werden die beim Entwerfen und Bereitstellen einer Richtlinie für Softwareeinschränkungen auszuführenden Schritte beschrieben. Beim Entwerfen von Richtlinien müssen mehrere Entscheidungen getroffen werden. Diese werden in der folgenden Tabelle beschrieben.

**Tabelle 6.4: Wichtige Überlegungen beim Entwerfen von Richtlinien**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Entscheidung

</th>

<th style="border:1px solid black;">

Zu berücksichtigende Faktoren

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Laptops oder Arbeitsstationen

</td>

<td style="border:1px solid black;">


Prüfen Sie die Bedürfnisse der mobilen Benutzer in der Umgebung, um zu bestimmen, ob für die Laptops eine andere Richtlinie erforderlich ist als für Desktops. Laptops verlangen häufig eine größere Flexibilität als Desktops.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Serverfreigaben, Anmeldeskripts und Basislaufwerke

</td>

<td style="border:1px solid black;">


Sie müssen Pfadregeln für alle Anwendungen definieren, die von einer Serverfreigabe oder einem Basisverzeichnis gestartet werden. Sie können der Pfadregel Anmeldeskriptdateien hinzufügen. Wenn ein Skript andere Skripts aufruft, fügen Sie der Pfadregel außerdem die Speicherorte dieser ausführbaren Dateien hinzu.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Gruppenrichtlinienobjekt oder lokale Sicherheitsrichtlinie

</td>

<td style="border:1px solid black;">


In diesem Handbuch wird für den Entwurf ein Gruppenrichtlinienobjekt verwendet. Sie sollten sich jedoch auch über die Auswirkungen einer lokalen Sicherheitsrichtlinie auf den Entwurf bewusst sein.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Benutzer- oder Computerrichtlinie

</td>

<td style="border:1px solid black;">


Dieser Entwurf wendet alle Einstellungen auf Computerebene an.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Standardsicherheitsstufe

</td>

<td style="border:1px solid black;">


Es wird empfohlen, **Nicht erlaubt** als Standardeinstellung zu festzulegen und anschließend den Rest der Richtlinie entsprechend zu konfigurieren. Die Standardeinstellung **Nicht eingeschränkt** ist ebenfalls verfügbar.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zusätzliche Regeln

</td>

<td style="border:1px solid black;">


Wenn Sie die Standardrichtlinie **Nicht erlaubt** verwenden, müssen Sie je nach Bedarf zusätzliche Pfadregeln für das Betriebssystem anwenden. Bei Verwendung von **Nicht erlaubt** werden die vier Regeln automatisch erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Richtlinienoptionen

</td>

<td style="border:1px solid black;">


Wenn Sie eine lokale Sicherheitsrichtlinie verwenden und die Richtlinie nicht auf Administratoren auf den Clientcomputern in der Umgebung angewendet werden soll, wählen Sie für die Richtlinie die Erzwingungsoption zum **Überspringen von Administratoren** aus.

Wenn Sie zusätzlich zu ausführbaren Dateien und Skripts auch DLLs überprüfen möchten, wählen Sie für die Richtlinie die Erzwingungsoption **DLL-Prüfung** aus.

Wenn Sie Regeln für Dateitypen festlegen möchten, die nicht in der Standardliste der designierten Dateitypen aufgeführt werden, verwenden Sie je nach Bedarf die Option für das Hinzufügen zum Dialogfeld **Eigenschaften von Designierte Dateitypen.**  

Wenn Sie ändern möchten, welche Personen Entscheidungen zum Herunterladen von ActiveX-Steuerelementen und anderen signierten Inhalten treffen können, aktivieren Sie auf der Registerkarte **Allgemein** des Dialogfelds **Eigenschaften von Vertrauenswürdigen Herausgebern** das Kontrollkästchen **Herausgeber.**  

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anwenden der Richtlinie auf einen Standort, eine Domäne oder Organisationseinheit

</td>

<td style="border:1px solid black;">


Die Richtlinie befindet sich unter der Organisationseinheit für Desktops und Laptops.

</td>

</tr>

</table>


**Hinweis**: Obwohl in diesem Handbuch empfohlen wird, Richtlinien für Softwareeinschränkungen auf Computerebene zu erzwingen, gibt es viele Fälle, in denen eine Erzwingung auf Benutzerebene sinnvoll ist. Eine Organisation mit freigegebenen Computern wie z. B. Terminalserver-Anwendungsservern oder Callcenter-Arbeitsstationen lassen möglicherweise zu, dass bestimmte Benutzer eine Anwendungsfamilie ausführen, wobei jedoch allen anderen Benutzern der Zugriff verweigert wird.

##### Empfohlene Vorgehensweisen

Microsoft empfiehlt, für die Richtlinie für Softwareeinschränkungen ein eigenes Gruppenrichtlinienobjekt zu erstellen. Dann hat es keine Auswirkungen auf die verbleibende Domänen- oder lokale Richtlinie, wenn Sie die Richtlinie notfalls deaktivieren müssen.

Wenn Sie außerdem während der Entwurfsphase der Organisationseinheit eine Arbeitsstation mithilfe der Richtlinie für Softwareeinschränkungen versehentlich sperren, starten Sie den Computer im **Abgesicherten Modus** neu, melden Sie sich als lokaler Administrator an, und ändern Sie dann die Richtlinie. Die Richtlinie für Softwareeinschränkungen wird nicht angewendet, wenn Windows im **Abgesicherten Modus** gestartet wird. Nachdem Sie den Computer im **Abgesicherten Modus** gestartet haben, führen Sie Gpupdate.exe aus, und starten Sie den Computer dann neu.

Die optimale Sicherheit erzielen Sie, wenn Sie zusammen mit der Richtlinie für Softwareeinschränkungen Zugriffskontrolllisten verwenden. Gewähren Sie Benutzern keine Administratorrechte. Benutzer versuchen möglicherweise, nicht erlaubte Dateien umzubenennen bzw. zu verschieben oder nicht eingeschränkte Dateien zu überschreiben, um die Richtlinien für Softwareeinschränkungen zu umgehen. Verwenden Sie Zugriffskontrolllisten, um zu verhindern, dass Benutzer diese Aktionen ausführen. Benutzer, die Mitglied der lokalen Gruppe **Administratoren** sind, können die von Ihnen implementierten Richtlinien für Softwareeinschränkungen umgehen. Deshalb empfiehlt Microsoft, Benutzern möglichst keine Administratorrechte zu gewähren.

Anmeldeskripts befinden sich meist auf dem Domänencontroller oder zentralen Server unter SYSVOL. Häufig wird bei jeder Anmeldung ein anderer Domänencontroller verwendet. Wenn die Standardregel auf **Nicht erlaubt** gesetzt ist, müssen Sie Regeln erstellen, die die Speicherorte der Anmeldeskripts angeben. Wenn die Anmeldeserver ähnliche Namen haben, können Sie Platzhalter für die Identifizierung verwenden oder für den Namen des Anmeldeskripts die Einstellung „Nicht eingeschränkt“ verwenden.

**Hinweis**: Testen Sie die neuen Einstellungen der Richtlinie für Softwareeinschränkungen ausgiebig in Testumgebungen, bevor Sie sie auf die Domäne anwenden. Neue Richtlinieneinstellungen zeigen möglicherweise ein anderes Verhalten als zunächst erwartet. Durch umfassende Tests wird die Möglichkeit verringert, dass Sie auf Probleme zu stoßen, wenn Sie die Einstellungen der Richtlinie für Softwareeinschränkungen im gesamten Netzwerk bereitstellen.


#### Die einzelnen Verfahrensschritte

Verwenden Sie die folgenden Informationen als Leitfaden für das Entwerfen einer Richtlinie für Softwareeinschränkungen und das Anwenden des Entwurfs in Form eines Gruppenrichtlinienobjekts auf die Laptops und Desktops in der Umgebung.

Schritt 1. Erstellen eines Gruppenrichtlinienobjekts für die Organisationseinheit

Suchen Sie die Organisationseinheit, die für die Desktops oder Laptops in der Umgebung erstellt wurde. Wenn Sie auf einem eigenständigen Client arbeiten, befinden sich die Einstellungen in der lokalen Computerrichtlinie. Klicken Sie in dieser Richtlinie auf **Eigenschaften**, und erstellen Sie dann ein neues Gruppenrichtlinienobjekt. Benennen Sie die Richtlinie gemäß der Benennungskonvention der Organisation. Berücksichtigen Sie, dass diese Richtlinie nur zum Erzwingen von Softwareeinschränkungen verwendet wird.

Schritt 2. Festlegen der Richtlinien für Softwareeinschränkungen

Markieren Sie das Gruppenrichtlinienobjekt, und klicken Sie auf **Bearbeiten.**   Durchlaufen Sie die Struktur bis zum Eintrag **Windows-Einstellungen\Sicherheitseinstellungen\Richtlinien für Softwareeinschränkung.**   Bei der ersten Bearbeitung der Richtlinie wird die folgende Meldung angezeigt:

Keine Richtlinien für Softwareeinschränkung definiert.

Durch diese Meldung werden Sie darauf hingewiesen, dass durch Erstellen einer Richtlinie Standardwerte definiert werden. Diese Standardwerte können Einstellungen anderer Richtlinien für Softwareeinschränkungen außer Kraft setzen. Da noch keine Einstellungen für Softwareeinschränkungen festgelegt wurden, gehen Sie von den Standardeinstellungen aus. Klicken Sie mit der rechten Maustaste auf das Menü **Aktion**, und wählen Sie **Neue Richtlinien für Softwareeinschränkungen erstellen** aus.

Schritt 3. Einrichten der Pfadregeln

Nachdem Sie bestimmt haben, welche Anwendungen und Skripts auf den Arbeitsstationen vorhanden sind, können Sie die Pfadregeln einrichten. Einige Programme starten zum Ausführen von Aufgaben andere Programme. Die Softwareanwendungen in der Umgebung sind u. U. von einem oder mehreren Hilfsprogrammen abhängig. Eine Inventar- und Installationsdokumentation der derzeit installierten Software ist beim Nachverfolgen von Pfadregeln hilfreich. Ein Entwurf für Arbeitstationen kann beispielsweise die folgenden Richtlinien umfassen:
* Anwendungen = *\Programme

* Freigegebene Gruppenanwendungen= g:\Gruppenanwendungen

* Anmeldeskript = Logon.bat

* Desktopverknüpfungen = *.lnk

* Genehmigte VBS-Skripts =*.vbs


##### Schritt 4. Festlegen der Richtlinienoptionen

Die folgenden Optionen beinhalten die empfohlenen Richtlinieneinstellungen für den in diesem Handbuch definierten Entwurf. Diese Optionen ändern den Gültigkeitsbereich des Erzwingungsverhalten der Authenticode-Vertrauenseinstellungen für digital signierte Dateien.
* **Erzwingen.**   Wenn der Computer Teil der Domäne ist, stellen Sie sicher, dass die Gruppe **Domänen-Admins** automatisch der Gruppe **Administratoren** hinzugefügt wird.

* **Übernehmen für Benutzer.**   Umfasst alle Benutzer außer den lokalen Administratoren. Die Verwendung dieser Option verzögert den Start aller Anwendungen. Um diese Verzögerung auszugleichen, wird die Richtlinie darauf konfiguriert, DLLs nicht zu prüfen.

* **Übernehmen für Dateien.**   Umfasst alle Softwaredateien mit Ausnahme von Bibliotheken (z. B. DLLs). Die Verwendung dieser Option verzögert den Start aller Anwendungen. Um diese Verzögerung auszugleichen, wird die Richtlinie darauf konfiguriert, DLLs nicht zu prüfen.

* **Designierte Dateitypen.**   Bei dem in diesem Handbuch definierten Entwurf eines Gruppenrichtlinienobjekts werden die Dateitypen.mdb und.lnk entfernt und der Dateityp.ocx hinzugefügt. Sie können je nach Bedarf benutzerdefinierte Erweiterungen von Anwendungsdateitypen hinzufügen, damit für diese die gleichen Regeln gelten.

* **Vertrauenswürdige Herausgeber.**   Bei dem in diesem Handbuch definierten Entwurf eines Gruppenrichtlinienobjekts wurde die Gruppe **Administratoren** aktiviert und die Option für **Eigenschaften von Vertrauenswürdigen Herausgebern: Administratoren des lokalen Computers** ausgewählt.


Bevor Sie einem Herausgeber vertrauen, wählen Sie beim Entwerfen eines Gruppenrichtlinienobjekts die Option **Überprüfen: Herausgeber**, um sicherzustellen, dass die Richtlinie Zertifikate überprüft.

##### Schritt 5. Anwenden der Standardeinstellungen

Es empfiehlt sich, die Richtlinie mit der Standardeinstellung **Nicht eingeschränkt** zu konfigurieren. Durch diese Methode wird sichergestellt, dass die Richtlinie korrekt initialisiert wird, bevor Softwareeinschränkungen angewendet werden. Setzen Sie die Standardeinstellung nach dem Überprüfen der Richtlinieneinstellungen auf **Nicht erlaubt** zurück.

Schritt 6. Testen der Richtlinie

Wenn der Computer sich in einer Domäne befindet, verschieben Sie den Computer in den Organisationseinheitscontainer, auf den die Richtlinie angewendet wird. Starten Sie den Testcomputer neu, und melden Sie sich an. Die Testpläne sollten Informationen dazu enthalten, wie die einzelnen Anwendungen nach dem Anwenden der Richtlinie funktionieren sollen. Führen Sie die Anwendungen aus, um sicherzustellen, dass sie ordnungsgemäß funktionieren und dass auf alle ihre Funktionen zugegriffen werden kann. Nachdem Sie das Funktionieren der Anwendungen überprüft haben, simulieren Sie einen Angriff auf die Anwendungen, um sicherzustellen, dass die Richtlinie keine Sicherheitslücken aufweist.

Wenn der Computer ein eigenständiger Client ist, melden Sie sich am Testcomputer an, und folgen Sie dem Testplan. Nachdem Sie die Anwendungen überprüft haben, starten Sie den simulierten Angriff erneut, um sicherzustellen, dass die Richtlinie keine Sicherheitslücken aufweist.


#### Bereitstellen der Richtlinie für Softwareeinschränkungen

Nach ausgiebigen Tests der Richtlinie wenden Sie sie auf die Desktop- oder Laptoporganisationseinheit in der Umgebung an. Wenn es sich um einen eigenständigen Client handelt, wenden Sie sie auf die lokalen Computereinstellungen auf dem Client an. Öffnen Sie das MMC-Snap-In „Computer und Benutzer“, und durchlaufen Sie das Verzeichnis bis zum Organisationseinheitscontainer für die Desktops oder Laptops. Erstellen Sie dann mithilfe des Gruppenrichtlinienobjekt-Editors das neue Gruppenrichtlinienobjekt. Bearbeiten Sie die Eigenschaften, und wenden Sie die entsprechenden Richtlinieneinstellungen gemäß den Informationen in den folgenden Tabellen unter **Windows-Einstellungen\Sicherheitseinstellungen** auf **Richtlinien für Softwareeinschränkung** an.

**Tabelle 6.5: Sicherheitsstufen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Standardregel in der Benutzeroberfläche

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Nicht erlaubt

</td>

<td style="border:1px solid black;">


Software wird unabhängig von den Zugriffsrechten des Benutzers nicht ausgeführt.

</td>

<td style="border:1px solid black;">


Verwenden Sie diese Standardregel

</td>

</tr>

</table>


**Tabelle 6.6: Zusätzliche Regeln**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Pfadregel

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


%HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\Current Version\SystemRoot%

</td>

<td style="border:1px solid black;">


Nicht eingeschränkt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


%HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\Current Version\SystemRoot%\*.exe

</td>

<td style="border:1px solid black;">


Nicht eingeschränkt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


%HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\Current Version\SystemRoot%\System32\*.exe

</td>

<td style="border:1px solid black;">


Nicht eingeschränkt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


%HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\Current Version\ProgramFilesDir%

</td>

<td style="border:1px solid black;">


Nicht eingeschränkt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


*.vbs

</td>

<td style="border:1px solid black;">


Nicht erlaubt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


G:\Gruppenanwendungen

</td>

<td style="border:1px solid black;">


Nicht eingeschränkt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Logon.bat oder Anmeldeskript

</td>

<td style="border:1px solid black;">


Nicht eingeschränkt

</td>

</tr>

<tr>

<td style="border:1px solid black;">


*\Programme

</td>

<td style="border:1px solid black;">


Nicht eingeschränkt

</td>

</tr>

</table>


**Tabelle 6.7: Erzwingen für Dateien und Benutzer**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Erzwingungsoptionen

</th>

<th style="border:1px solid black;">

Empfehlung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Wenden Sie Richtlinien für Softwareeinschränkungen auf Folgendes an:

</td>

<td style="border:1px solid black;">


Alle Softwaredateien außer Bibliotheken (z. B. DLLs).

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Wenden Sie Richtlinien für Softwareeinschränkungen auf folgende Benutzer an:

</td>

<td style="border:1px solid black;">


Alle Benutzer außer den lokalen Administratoren.

</td>

</tr>

</table>


**Tabelle 6.8: Designierte Dateitypen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Dateitypen

</th>

<th style="border:1px solid black;">

Empfehlung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Eigenschaften von Designierte Dateitypen

</td>

<td style="border:1px solid black;">


Entfernen Sie die Dateitypen.mdb und.lnk, und fügen Sie den Dateityp.ocx hinzu.

</td>

</tr>

</table>


**Tabelle 6.9: Vertrauenswürdige Herausgeber**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Vertrauenswürdige Herausgeber

</th>

<th style="border:1px solid black;">

Empfehlung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Erlauben Sie den folgenden Benutzergruppen die Auswahl vertrauenswürdiger Herausgeber:

</td>

<td style="border:1px solid black;">


**Administratoren des lokalen Computers**

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Bestimmen Sie, ob das Zertifikat gesperrt wurde.

</td>

<td style="border:1px solid black;">


Wählen Sie die Option **Herausgeber** aus.

</td>

</tr>

</table>

 
[Zum Seitenanfang](#mainsection)  



### Zusammenfassung

Die Richtlinie für Softwareeinschränkungen bietet Administratoren eine effektive Möglichkeit für die Identifizierung und Steuerung von Software auf Computern mit Windows XP Professional. Sie können Richtlinien erstellen, um schädliche Skripts zu blockieren, Computer in der Umgebung zu sperren oder die Ausführung von Anwendungen zu verhindern. In einem Unternehmen empfiehlt es sich, Richtlinien für Softwareeinschränkungen mit Gruppenrichtlinienobjekten zu verwalten und dann die einzelnen Richtlinien an die Anforderungen der verschiedenen Benutzergruppen und Computer anzupassen. Microsoft empfiehlt, in einer Umgebung mit eigenständigen Computern keine Benutzergruppen zu verwalten.

Richtlinien für Softwareeinschränkungen erhöhen bei richtiger Anwendung die Sicherheit von Computern, erleichtern ihre Verwaltung und senken letzten Endes die Gesamtkosten für Betriebssysteme auf diesen Computern.


#### Weitere Informationen

Die folgenden Links bieten weitere Informationen zu sicherheitsbezogenen Themen hinsichtlich Windows XP Professional.
* Weitere Informationen zur Verwendung von Richtlinien für Softwareeinschränkungen finden Sie im Artikel „[Schutz vor nicht autorisierter Software mit Richtlinien für Softwareeinschränkung](https://technet.microsoft.com/de-de/library/4b16da45-ae6b-452e-89c8-ddf606e14b8c(v=TechNet.10))“ (in englischer Sprache) unter http://www.microsoft.com/germany/technet/prodtechnol/winxppro/maintain/rstrplcy.mspx.

* Weitere Informationen zu Gruppenrichtlinien finden Sie in „[Windows 2000-Gruppenrichtlinien](http://www.microsoft.com/windows2000/techinfo/howitworks/management/grouppolwp.asp)“ (in englischer Sprache) unter www.microsoft.com/windows2000/techinfo/howitworks/management/grouppolwp.asp.

 

In diesem Beitrag
* [Überblick](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10))
* [Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP](https://technet.microsoft.com/de-de/library/4eddb4e4-fd7b-444c-8484-bb8ee220c0e1(v=TechNet.10))
* [Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory](https://technet.microsoft.com/de-de/library/620c0004-41a8-4d13-9a61-e6d879f9cc65(v=TechNet.10))
* [Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients](https://technet.microsoft.com/de-de/library/bca34b8d-a1ca-42e4-b743-aa3ca12fd8f9(v=TechNet.10))
* [Kapitel 4: Administrative Vorlagen für Windows XP](https://technet.microsoft.com/de-de/library/adb79ec2-691f-4a9f-b940-36d2d9807fd7(v=TechNet.10))
* [Kapitel 5: Schützen eigenständiger Windows XP-Clients](https://technet.microsoft.com/de-de/library/a134d1cb-2ad1-4549-99c8-2a5e0128f2dc(v=TechNet.10))
* Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients
* [Kapitel 7: Zusammenfassung](https://technet.microsoft.com/de-de/library/8001f9fb-f330-4ab4-a134-ff756091ea0d(v=TechNet.10))
* [Anhang A: Weitere Anleitungen für Windows XP Service Pack 2](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapa.mspx)
* [Anhang A: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/6b4fdfca-4c2c-47f6-8c92-de33a663ea03(v=TechNet.10))
* [Anhang B: Testen des Sicherheitshandbuchs für Windows XP](https://technet.microsoft.com/de-de/library/09c716f4-b167-49ec-8122-93e1b8c5f456(v=TechNet.10))
* [Danksagungen](https://technet.microsoft.com/de-de/library/7e874ad0-7c5a-4f64-9349-760666ab3e61(v=TechNet.10))
 

Download

![](images/cc163080.icon_exe(de-de,technet.10).gif)[Windows XP-Sicherheitshandbuch herunterladen (engl.)](http://go.microsoft.com/fwlink/?linkid=14840&amp;clcid=0x409"><img AltText="Download)  
 

 
[Zum Seitenanfang](#mainsection)