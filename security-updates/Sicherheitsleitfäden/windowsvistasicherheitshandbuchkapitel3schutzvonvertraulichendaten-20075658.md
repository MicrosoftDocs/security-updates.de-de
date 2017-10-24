---
Title: Windows Vista-Sicherheitshandbuch – Kapitel 3 (Schutz von vertraulichen Daten)
TOCTitle: Windows Vista-Sicherheitshandbuch – Kapitel 3 (Schutz von vertraulichen Daten)
ms:assetid: ea0af17d-7c97-4469-843e-27a15261f407
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443715(v=TechNet.10)
ms:contentKeyID: 20075658
---


# Windows Vista-Sicherheitshandbuch



### Kapitel 3: Schutz von vertraulichen Daten
Veröffentlicht: November 8, 2006
 

Alljährlich werden weltweit Hunderttausende von Computern, die nicht über angemessene Schutzmaßnahmen verfügen, verloren, gestohlen oder unsachgemäß außer Betrieb genommen. Laut der Umfrage des CSI/FBI über Computerkriminalität und Sicherheit (Computer Crime and Security Survey) im Jahr 2006 sind die Kosten, die sich aus Datenverlusten ergeben, im Vergleich zum Vorjahr um satte 65 % gestiegen.

Wirksame Technologiefunktionen und Dienste, mit denen es möglich ist, den Risiken von Datendiebstahl und Datengefährdung entgegenzuwirken, zählten zu den wichtigsten Kundenwünschen für Windows Vista™. Dies ist teilweise dadurch begründet, dass böswillige Benutzer häufig ein anderes Betriebssystem auf einem Clientcomputer ausführen, die Festplatte in einen anderen Computer einbauen oder mit anderen Offline-Angriffsmethoden die Daten auf verlorenen oder gestohlenen Computern abrufen können. In vielen Fällen ist die Absicherung der Daten durch neue Gesetze und Vorschriften zu einer gesetzlichen Pflicht geworden.

Aus diesen Sicherheitsgründen hat Microsoft sowohl neue als auch optimierte Funktionen und Dienste entwickelt, mit denen ein Unternehmen die Daten auf den Clientcomputern noch besser schützen kann. Die in diesem Kapitel erläuterten Funktionen und Dienste sind für den Schutz von Daten auf Clientcomputern ausgelegt, auf denen Windows Vista in der Unternehmensclient-Umgebung ausgeführt wird. Die Konfiguration dieser Funktionen ergibt sich dabei aus Ihren individuellen Anforderungen und Ihrer Arbeitsumgebung. In diesem Kapitel finden Sie einen Beispielprozess, aus dem hervorgeht, wie Sie die nachstehenden Funktionen und Dienste gemäß Ihren Datenschutzanforderungen optimal konfigurieren:
* BitLocker™-Laufwerkverschlüsselung

* Verschlüsselndes Dateisystem (EFS)

* Rechteverwaltungsdienste (RMS)

* Gerätesteuerung

 

Mit BitLocker, EFS und RMS sowie mit der Gerätesteuerung können Sie vertrauliche Daten im Unternehmen schützen. Jede Technologie und jede Methode übernimmt dabei bestimmte Funktionen zum Schutz von Daten. Alle diese Technologien und Methoden sind Elemente für den Datenschutz, die sich gegenseitig ergänzen. Microsoft empfiehlt daher dringend, diese Elemente in die Gesamtsicherheitsstrategie des Unternehmens einzubinden. Sie können die Elemente wahlweise einzeln oder in Kombination miteinander nutzen, je nach den Sicherheitsanforderungen Ihres Unternehmens. Die Beispiele in der nachstehenden Tabelle zeigen, wie diese Technologien und Methoden gemeinsam für den Schutz in verschiedenen Szenarien in einem Unternehmen sorgen.

**Tabelle 3.1 Vergleich der Datenschutztechnologien in Windows Vista**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Szenario

</th>

<th style="border:1px solid black;">

    BitLocker

</th>

<th style="border:1px solid black;">

        EFS

</th>

<th style="border:1px solid black;">

        RMS

</th>

<th style="border:1px solid black;">

Gerätesteuerung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Datenschutz für Laptops

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Datenschutz für Server in Zweigstellen

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schutz für lokale Dateien und Ordner, die nur von einem einzelnen Benutzer verwendet werden

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Datenschutz für Desktops

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schutz für Dateien und Ordner auf gemeinsam genutzten Computern

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schutz für Remotedateien und -ordner

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schutz vor nicht vertrauenswürdigen Netzwerkadministratoren

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Durchsetzung von Richtlinien für Remotedokumente

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schutz von Inhalten beim Transport

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schutz von Inhalten bei der Zusammenarbeit

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schutz vor Datendiebstahl

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


          

</td>

</tr>

</table>


Auf dieser Seite

[BitLocker-Laufwerkverschlüsselung](#eeaa)  
[Verschlüsselndes Dateisystem](#edaa)  
[Rechteverwaltungsdienste](#ecaa)  
[Gerätesteuerung](#ebaa)  
[Weitere Informationen](#eaaa)  



### BitLocker-Laufwerkverschlüsselung

Die BitLocker-Laufwerkverschlüsselung schützt die Daten auf Clientcomputern. Das gesamte Windows-Volume wird verschlüsselt, so dass nicht autorisierte Benutzer nicht in der Lage sind, die Windows-Maßnahmen für den Datei- und Systemschutz auszuhebeln oder Daten auf dem abgesicherten Laufwerk offline abzurufen. Zu einem frühen Zeitpunkt im Startvorgang prüft BitLocker die System- und Hardwareintegrität des Clientcomputers. Falls BitLocker feststellt, dass versucht wurde, die Systemdateien oder andere Daten zu manipulieren, wird der Clientcomputer nicht gestartet.

BitLocker hilft zu verhindern, dass Datendiebe, die ein anderes Betriebssystem starten oder ein Softwareangriffstool ausführen, die Datei- und Systemschutzmaßnahmen von Windows Vista für die auf dem geschützten Laufwerk gespeicherten Dateien umgehen oder diese Dateien offline anzeigen können.

Mit der BitLocker-Laufwerkverschlüsselung wird die normale Bootsequenz so lange gesperrt, bis der Benutzer eine PIN-Nummer eingibt oder ein USB-Flash-Laufwerk mit den entsprechenden Schlüsseln für die Entschlüsselung einlegt. Der größtmögliche Schutz wird erzielt, wenn der Computer über ein TPM 1.2 (Trusted Platform Module) verfügt. Dieses Modul schützt die Benutzerdaten und sorgt außerdem dafür, dass ein Clientcomputer, auf dem Windows Vista ausgeführt wird, auch im Offlinezustand nicht manipuliert werden kann. Weitere Informationen zur TPM-Technologie finden Sie in den Spezifikationen und Dokumenten auf der Website der [Trusted Computing Group](http://www.trustedcomputinggroup.org/) (engl.). Falls kein TPM vorhanden ist, kann BitLocker dennoch zum Schutz der Daten beitragen; die Systemintegrität lässt sich allerdings nicht überprüfen.

BitLocker steht in der Enterprise Edition und der Ultimate Edition von Windows Vista für Clientcomputer zur Verfügung.

**Hinweis:**   BitLocker bietet Schutz für die Windows-Partition und ist kein Ersatz für EFS. Mit BitLocker werden keine Daten verschlüsselt, die sich außerhalb der Windows-Partition befinden. Die Anwendung sorgt jedoch für eine zusätzliche Sicherheitsschicht für EFS, indem die EFS-Schlüssel innerhalb der Windows-Partition verschlüsselt werden.


#### Risikobewertung

Mobile Computer werden im Allgemeinen in unsicheren Arbeitsumgebungen eingesetzt, in denen ein höheres Risiko besteht, dass die Computer verloren gehen oder gestohlen werden. Falls ein böswilliger Benutzer physischen Zugriff auf ein System erlangt, kann dieser Benutzer zahlreiche Sicherheitsmaßnahmen umgehen, die für den Schutz des Systems und der Daten gedacht waren. Auch Desktopcomputer in freigegebenen oder öffentlichen Umgebungen sind oft einem beträchtlichen Risiko ausgesetzt. Das wichtigste Risiko, dem BitLocker entgegenwirken soll, ist der Diebstahl der Daten, die sich auf gestohlenen oder verloren gegangenen mobilen Computern befinden.

Wenn ein Angreifer physischen Zugriff auf einen Computer erhält, ist mit den folgenden Konsequenzen zu rechnen:
* Der Angreifer kann sich bei Windows Vista anmelden und Dateien kopieren.

* Der Angreifer kann den Clientcomputer zu folgenden Zwecken mit einem anderen Betriebssystem starten:
* Anzeigen von Dateinamen
 

* Kopieren von Dateien
 

* Lesen des Inhalts der Ruhezustandsdatei oder der Auslagerungsdatei, um so ggf. Kopien von derzeit bearbeiteten Dokumenten in Klartext aufzufinden
 

* Lesen des Inhalts der Ruhezustandsdatei, um so eventuell Klartextkopien von privaten Softwareschlüsseln aufzufinden
 

 

 

Selbst wenn die Dateien mit EFS verschlüsselt werden, könnte ein unvorsichtiger Benutzer eine Datei aus einem verschlüsselten in ein unverschlüsseltes Verzeichnis kopieren oder verschieben, so dass der Inhalt der Datei als Klartext vorliegt. Außerdem können uninformierte IT-Mitarbeiter die Verschlüsselung von verborgenen Ordnern, in denen Sicherungskopien der derzeit bearbeiteten Dateien durch die Anwendungen abgelegt werden, schlichtweg übersehen. Darüber hinaus bestehen einige Risiken im Hinblick auf die Bedienung (z. B. Manipulation und Bearbeitung von System- und Bootdateien durch nicht autorisierte Benutzer), die einen normalen Systembetrieb unmöglich machen können.


#### Risikominderung

Um diese Risiken zu mindern, sollte die Bootsequenz im Computer so geschützt werden, dass das System nur dann startet, wenn der betreffende Benutzer eine entsprechende Autorisierung beibringt. Außerdem sollten Betriebssystem- und Datendateien geschützt werden.


#### Überlegungen zur Risikominderung

Mit BitLocker lassen sich die Risiken aus dem vorangegangenen Abschnitt „Risikobewertung“ mindern. Bevor Sie jedoch BitLocker erstmalig einsetzen, beachten Sie die nachstehenden Anforderungen und Best Practice-Verfahren für diese Datenschutzfunktion:
* Damit BitLocker mit der optimalen Konfiguration genutzt werden kann, muss die Hauptplatine des Clientcomputers mit einem TPM 1.2-Chip ausgestattet sein, der eine mit der Trusted Computing Group konforme BIOS-Implementierung enthält. Darüber hinaus ist (optional) ein Systemstartschlüssel erforderlich, um einen zusätzlichen Authentifizierungsfaktor zu bieten. Der Systemstartschlüssel besteht entweder aus einem zusätzlichen physischen Schlüssel (ein USB-Flash-Laufwerk, auf dem sich ein maschinenlesbarer Schlüssel befindet) oder aus einem PIN-Eintrag, der vom Benutzer festgelegt wird. Zudem sind sichere Benutzeranmeldungs- und Kennwortprotokolle erforderlich.

* BitLocker ist nur dann funktionsfähig, wenn die Festplatte des Computers ordnungsgemäß partitioniert ist. Für BitLocker sind zwei NTFS-Laufwerkvolumes erforderlich: ein Systemvolume und ein Betriebssystemvolume. Die Partition für das Systemvolume sollte mindestens 1,5 GB umfassen.

* BitLocker-Konfigurationen, die nicht auf die Authentifizierung mit externem Schlüssel setzen, sind anfälliger für hardwarebasierte Angriffe.

* Wenn Sie BitLocker mit einem USB-Schlüssel oder einer PIN-Nummer nutzen, müssen Verfahren für den Fall aufgestellt werden, dass die Benutzer die Schlüssel verlieren oder die PIN-Nummer vergessen.

* BitLocker wirkt sich geringfügig auf die Systemleistung aus, was aber in der Regel nicht wahrnehmbar ist. Sollte die Systemleistung einen entscheidenden Stellenwert einnehmen (z. B. bei Servern), testen Sie die Konfiguration gründlich, um so sicherzustellen, dass die Leistung durch BitLocker nicht maßgeblich beeinträchtigt wird.

* Je nach Computerhersteller müssen Sie bei den TPM-Verwaltungstools den TPM-Gerätestatus und das BIOS-Administratorkennwort während Buildprozesses ggf. manuell festlegen. Die vollständig automatisierte oder skriptgesteuerte Bereitstellung und Aktualisierung ist dadurch dann eventuell nicht möglich.

* Ein TPM-Gerät ist nur dann funktionsfähig, wenn ein Endorsement Key (EK) für die Anmeldeinformationen vorliegt. Diesen EK erhalten Sie über den Hersteller des Computers oder einen VAR (Value Added Reseller) oder, nach erfolgter Bereitstellung des Systems, auch von IT-Supportmitarbeitern. Der EK muss sicher aufbewahrt und, während der Computer in Gebrauch ist, verfolgt werden.

* Falls der Computer nicht über TPM verfügt, sollte der Computer die Verwendung von USB-Geräten bei seinem Start unterstützen, so dass das Volume während der Bootsequenz mithilfe eines Systemstartschlüssels entsperrt werden kann.

* Wenn Software- oder Systemaktualisierungen im Remoteverfahren und außerhalb der normalen Geschäftszeiten verteilt werden und Sie die Benutzercomputer in Abwesenheit der Benutzer neu starten, kann sich BitLocker auf die Verfahren zur Softwareverteilung auswirken. Beispiel:
* Ein Computer ist mit TPM und einer PIN-Nummer oder mit TPM und einem Systemstartschlüssel geschützt. Um 2:00 Uhr in der Nacht stellen Sie eine Softwareaktualisierung für den Computer bereit, bei der ein Neustart erforderlich ist. Der Computer kann jedoch ohne die PIN-Nummer oder den Systemstartschlüssel nicht gestartet werden.
 

* Auch Computer, die Sie derzeit für Wartungsarbeiten bei Bedarf über die Funktion „Wake-on-LAN“ oder über eine BIOS-Funktion zum automatischen Einschalten starten, sind durch den Schutz mit TPM und PIN-Nummer oder Systemstartschlüssel betroffen.
 

 

* Updates für BIOS/TPM-Firmware, die von OEMs vertrieben werden, können sich auf für BitLocker aktivierte Computer auswirken. Ermitteln Sie anhand der Installationsanweisungen des OEM, ob Wiederherstellungsinformationen (Wiederherstellungskennwörter und Schlüssel) auch nach der Aktualisierung noch vorhanden sind und ob zusätzliche Schutzvorkehrungen (PINs oder Systemstartschlüssel) beibehalten werden.

* Anwendungsaktualisierungen können sich auf für BitLocker aktivierte Computer auswirken. Wenn der Boot-Manager oder von BitLocker überwachte Dateien im Rahmen der Installation oder Aktualisierung geändert werden, schlägt das Starten des Systems fehl, und der Computer wird in den Wiederherstellungsmodus versetzt. Vor dem Installieren oder Aktualisieren von Anwendungen, die sich auf die Bootumgebung von Windows Vista auswirken, sollten Sie diese Anwendungen daher auf für BitLocker aktivierten Computern testen.

* Auf allen Domänencontroller in der Domäne muss Microsoft® Windows Server® 2003 mit Service Pack 1 (SP1) oder höher ausgeführt werden.

**Hinweis**:   Bei Windows Server 2003 muss das Schema so erweitert werden, dass die Speicherung der BitLocker-Wiederherstellungsinformationen im Active Directory®-Verzeichnisdienst unterstützt wird.

 


#### Verfahren zur Risikominderung

Ermitteln Sie die bestmögliche Konfiguration von BitLocker zum Schutz vertraulicher Daten auf den verwalteten Clientcomputern mithilfe des nachstehenden Verfahrens zur Risikominderung.

**So verwenden Sie dieses Verfahren zur Risikominderung**
* Informieren Sie sich über die Technologien und Funktionen von BitLocker.

**Hinweis:** Weitere Informationen zu BitLocker finden Sie auf der Webseite [BitLocker-Laufwerkverschlüsselung – Überblick](https://technet.microsoft.com/de-de/library/c32fc2a2-5b2f-4360-99ea-8258b04e5f45(v=TechNet.10)).

* Beurteilen Sie die Notwendigkeit von BitLocker in Ihrer Arbeitsumgebung.

* Stellen Sie fest, ob die Hardware, Firmware und Software in Ihrem Unternehmen den Anforderungen von BitLocker entspricht.

* Bestimmen Sie die Systeme im Unternehmen, die durch BitLocker geschützt werden sollen.

* Ermitteln Sie den Umfang des Schutzes, der für diese Systeme erforderlich ist. Unter Umständen kann das Betriebssystem nur mit einer PIN-Nummer oder einem USB-Schlüssel, der wiederum Verschlüsselungsschlüssel enthält, gestartet werden. Ohne diese Schlüssel ist das Starten das Betriebssystem nicht möglich.

* Installieren Sie die notwendigen Treiber auf einem Testsystem.

* Konfigurieren Sie BitLocker mithilfe von Gruppenrichtlinienobjekten (GPOs) auf Testsystemen.

* Nachdem die Tests erfolgreich abgeschlossen wurden, installieren Sie die Treiber, und konfigurieren Sie BitLocker auf Produktionssystemen.

 

Risikominderung bei BitLocker mithilfe von Gruppenrichtlinien

Für die Konfiguration von BitLocker empfiehlt Microsoft zwei bestimmte Gruppenrichtlinienvorlagen. Mit diesen Vorlagen sind Sie in der Lage, die TPM-Konfiguration völlig getrennt von den übrigen Bestandteilen von BitLocker zu verwalten. In der nachstehenden Tabelle werden die Gruppenrichtlinieneinstellungen aufgeführt, die für BitLocker in der Vorlage „VolumeEncryption.admx“ zur Verfügung stehen. Diese Einstellungen können im Gruppenrichtlinienobjekt-Editor im folgenden Verzeichnis konfiguriert werden:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\BitLocker-Laufwerkverschlüsselung**

**Tabelle 3.2 Einstellungen für die BitLocker-Laufwerkverschlüsselung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinieneinstellung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

<th style="border:1px solid black;">

Standardeinstellung in Windows Vista

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Turn on BitLocker backup to Active Directory Domain Services (BitLocker-Sicherung in Active Directory-Domänendiensten aktivieren)

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht die Sicherung der BitLocker-Wiederherstellungsinformationen in Active Directory. Diese Wiederherstellungsinformationen umfassen das Wiederherstellungskennwort und einige eindeutige Kennungen.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Control Panel Setup: Configure recovery folder (Systemsteuerungs-Setup: Wiederherstellungsordner konfigurieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung legen Sie fest, ob der Benutzer im Setup-Assistenten für BitLocker gefragt werden soll, ob der Wiederherstellungsschlüssel in einem Ordner gespeichert werden soll. Diese Einstellung bestimmt den Standardpfad, der angezeigt wird, wenn der Benutzer durch den Setup-Assistent für BitLocker aufgefordert wird, den Pfad für den Ordner einzugeben, in dem der Wiederherstellungsschlüssel gespeichert werden soll.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Control Panel Setup: Configure recovery options (Systemsteuerungs-Setup: Wiederherstellungsoptionen konfigurieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung legen Sie fest, ob der Benutzer im Setup-Assistenten für BitLocker gefragt werden soll, ob ein Wiederherstellungskennwort angelegt werden soll. Das Wiederherstellungskennwort besteht aus einer auf Zufallsbasis erzeugten 48-stelligen Zeichenfolge.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Control Panel Setup: Enable advanced startup options (Systemsteuerungs-Setup: Erweiterte Startoptionen aktivieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung legen Sie fest, ob der Benutzer im Setup-Assistenten für BitLocker gefragt werden soll, ob eine PIN-Nummer auf dem Computer erstellt werden soll. Die PIN-Nummer besteht aus einer 4- bis 20-stelligen Ziffernfolge, die der Benutzer bei jedem Starten des Computers eingeben muss. Die Anzahl der Stellen lässt sich nicht über eine Richtlinie festlegen.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Configure encryption method (Verschlüsselungsmethode konfigurieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung konfigurieren Sie den Verschlüsselungsalgorithmus und die Schlüsselgröße für BitLocker. Diese Richtlinieneinstellung gilt für vollständig entschlüsselte Datenträger. Falls der Datenträger bereits verschlüsselt ist oder gerade verschlüsselt wird, ist eine Änderung der Verschlüsselungsmethode wirkungslos.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Configure TPM platform validation profile (Profil für Überprüfung der TPM-Platform konfigurieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung legen Sie fest, wie der Verschlüsselungsschlüssel des Volumes durch TPM gesichert werden soll. Diese Richtlinieneinstellung tritt nicht in Kraft, wenn der Computer kein kompatibles TPM besitzt. Vorhandene Kopien des Verschlüsselungsschlüssels bleiben außerdem von Änderungen dieser Richtlinie unberührt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


In der obigen Tabelle werden die einzelnen Einstellungen kurz beschrieben. Weitere Informationen zu einer bestimmten Einstellung finden Sie im Gruppenrichtlinienobjekt-Editor auf der Registerkarte **Erklärung** dieser Einstellung.

In der nachstehenden Tabelle werden die Gruppenrichtlinieneinstellungen aufgeführt, die für TPM in der Vorlage „TPM.admx“ zur Verfügung stehen. Diese Einstellungen können im Gruppenrichtlinienobjekt-Editor im folgenden Verzeichnis konfiguriert werden:

**Computerkonfiguration\Administrative Vorlagen\System\Trusted Platform Module Services**

**Tabelle 3.3 Einstellungen für das Trusted Platform Module (TPM)**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinieneinstellung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

<th style="border:1px solid black;">

Standardeinstellung in Windows Vista

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Turn on TPM backup to Active Directory Domain Services (TPM-Sicherung in Active Directory-Domänendiensten aktivieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung verwalten Sie die Sicherung der TPM-Wiederherstellungsinformationen in Active Directory. Diese Wiederherstellungsinformationen umfassen eine kryptografische Ableitung des Kennworts des TPM-Besitzers.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Configure the list of blocked TPM commands (Liste der blockierten TPM-Befehle konfigurieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung verwalten Sie die Gruppenrichtlinienliste der TPM-Befehle, die von Windows blockiert werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Ignore the default list of blocked TPM commands (Standardliste der blockierten TPM-Befehle ignorieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung verwalten Sie die Durchsetzung der Standardliste blockierter TPM-Befehle, die auf dem Computer vorliegt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Ignore the local list of blocked TPM commands (Lokale Liste der blockierten TPM-Befehle ignorieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung verwalten Sie die Durchsetzung der lokalen Liste blockierter TPM-Befehle, die auf dem Computer vorliegt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


In dieser Tabelle werden die einzelnen Einstellungen kurz beschrieben. Weitere Informationen zu einer bestimmten Einstellung finden Sie im Gruppenrichtlinienobjekt-Editor auf der Registerkarte **Erklärung** dieser Einstellung.

Ihre Sicherheitsrichtlinien müssen die Kennwort- und Schlüsselverwaltung durch BitLocker effektiv unterstützen. Diese Richtlinien sollten so umfassend gestaltet sein, dass die Daten angemessen gesichert sind, ohne dabei so starke Einschränkungen aufzustellen, dass BitLocker nur noch unter Schwierigkeiten unterstützt werden kann. In der folgenden Liste finden Sie einige Beispiele für Richtlinien:
* Verlangen Sie stets die Sicherung der Wiederherstellungskennwörter in Active Directory.

* Verlangen Sie stets die Sicherung der TPM-Besitzerinformationen in Active Directory.

* Nutzen Sie Wiederherstellungsschlüssel zusammen mit Wiederherstellungskennwörtern als Sicherungsmethode oder als alternatives Wiederherstellungsverfahren.

* Wenn Sie TPM und eine PIN-Nummer oder USB-Systemstartschlüssel verwenden, ändern Sie diese Angaben in regelmäßigen Abständen.

* Unterbinden Sie den Zugriff auf TPM-fähige Computer mithilfe eines BIOS-Administratorkennworts.

* Sorgen Sie dafür, dass die Benutzer keine Schlüssel (z. B. USB-Systemstartschlüssel) auf dem Computer speichern.

* Speichern Sie die Wiederherstellungsschlüssel an zentraler Stelle, so dass der Support und die Wiederherstellung nach einem Systemausfall unkomplizierter ablaufen.

* Sichern Sie die Wiederherstellungsinformationen auf sicheren Offlinespeichermedien.

 
[Zum Seitenanfanq](#mainsection)  



### Verschlüsselndes Dateisystem

Mit dem verschlüsselnden Dateisystem (Encrypting File System, EFS) können Sie Dateien und Ordner verschlüsseln, um so zum Schutz der Daten vor unbefugtem Zugriff beizutragen. Das EFS ist in das NTFS-Dateisystem integriert, und sein Betrieb ist für Anwendungen vollständig transparent. Wenn ein Benutzer oder ein Programm versucht, auf eine verschlüsselte Datei zuzugreifen, versucht das Betriebssystem automatisch, einen Entschlüsselungsschlüssel für den Inhalt dieser Datei abzurufen und führt anschließend im Hintergrund die Ver- und Entschlüsselung im Namen des Benutzers durch. Benutzer mit autorisierten Schlüsseln können wie gewohnt auf verschlüsselte Dateien zugreifen und mit diesen Dateien arbeiten, während anderen Benutzern der Zugriff verwehrt wird. Windows Vista umfasst zahlreiche neue Features für die Sicherheit, die Leistung und die Verwaltung des EFS:
* Sie können die Benutzerschlüssel auf Smartcards speichern.

* Sie können die Wiederherstellungsschlüssel auf Smartcards speichern, so dass eine sichere Datenwiederherstellung ohne dedizierte Arbeitsstation für die Wiederherstellung möglich wird, und das selbst über Remotedesktopsitzungen.

* Sie können die Windows-Auslagerungsdatei über EFS mit einem Schlüssel verschlüsseln, der beim Starten des Systems erzeugt und beim Herunterfahren automatisch vernichtet wird.

* Sie können den Offlinedateicache mit EFS verschlüsseln. In Windows Vista greift diese Verschlüsselungsfunktion nicht auf den Systemschlüssel zurück, sondern auf den Schlüssel des Benutzers. Auf diese Weise lassen sich die einzelnen Dateien im Offlinedateicache nur durch den Benutzer öffnen, für den die betreffende Datei zwischengespeichert wurde.

* Die Gruppenrichtlinie bietet zahlreiche neue Konfigurationsoptionen zur Durchsetzung von Unternehmensrichtlinien.

* EFS unterstützt eine größere Palette von Benutzerzertifikaten und Schlüsseln.

 

Windows Vista wurde um eine Reihe neuer Gruppenrichtlinienoptionen ergänzt, mit denen Administratoren Unternehmensrichtlinien für EFS definieren und umsetzen können. Hierzu gehört beispielsweise die Möglichkeit, Smartcards für EFS anzufordern, die Verschlüsselung der Auslagerungsdatei zu erzwingen, eine Mindestlänge für Schlüssel im EFS vorzuschreiben und die Verschlüsselung des Ordners mit den eigenen Dateien eines Benutzers durchzusetzen.

**Hinweis**   Microsoft empfiehlt den gemeinsamen Einsatz von BitLocker und EFS, um so den größtmöglichen Schutz für Daten zu erzielen.


#### Risikobewertung

Der nicht autorisierte Zugriff auf Daten kann die Unternehmensprozesse und die Rentabilität eines Unternehmens ernsthaft gefährden. Daten sind stets in Gefahr, insbesondere wenn mehrere Benutzer Zugriff auf dasselbe System besitzen oder wenn mobile Computersysteme eingesetzt werden. Der Bereich, in dem EFS zur Risikominderung beitragen soll, umfasst den Datendiebstahl oder die Gefährdung von Daten, die sich aus dem Verlust oder dem Diebstahl mobiler Computer (oder auch durch Offenlegung eines Insiders) ergibt. Freigegebene Computer sind u. U. ebenfalls dieser Gefahr ausgesetzt.

Wenn ein Angreifer physischen Zugriff auf einen Computer erhält, der unverschlüsselte Daten enthält, ist mit den folgenden Konsequenzen zu rechnen:
* Der Angreifer könnte den Computer neu starten, seine Benutzerberechtigungen auf die Rechte eines lokalen Administrators erweitern und so auf die Daten des Benutzers zugreifen. Der Angreifer könnte außerdem Tools herunterladen, die einen Brute-Force-Angriff starten, um das Kennwort des Benutzers zu ermitteln. Auf diese Weise könnte der Angreifer sich als dieser Benutzer anmelden und auf dessen Daten zugreifen.

* Der Angreifer könnte versuchen, sich bei Windows Vista anzumelden und alle Daten, die dem Benutzer zur Verfügung stehen, auf ein Wechselmedium zu kopieren, per E-Mail zu versenden, über das Netzwerk zu kopieren oder per FTP auf einen Remoteserver zu übertragen.

* Der Angreifer könnte den Computer mit einem anderen Betriebssystem starten und Dateien direkt von der Festplatte kopieren.

* Der Angreifer könnte den Computer mit einem anderen Netzwerk verbinden, den gestohlenen Computer starten und sich dann im Remoteverfahren bei diesem Computer anmelden.

* Wenn ein Benutzer die Netzwerkdateien in den Offlinedateien zwischenspeichert, kann ein Angreifer die Berechtigungen auf „Administrator/LocalSystem“ erhöhen und den Inhalt des Offlinedateicache untersuchen.

* Ein neugieriger Mitarbeiter könnte vertrauliche Dateien öffnen, die anderen Benutzern eines freigegebenen Computers gehören.

* Ein Angreifer könnte den Computer mit einem anderen Betriebssystem neu starten, den Inhalt der Auslagerungsdatei lesen und Kopien von derzeit bearbeiteten Dokumenten in Klartext auffinden.

 


#### Risikominderung

Um diesen Risken einer Datengefährdung zu begegnen, können Sie die Daten verschlüsseln, sobald sie auf der Festplatte gespeichert werden. Die neuesten Verbesserungen der EFS-Technologie in Windows Vista tragen zur Risikominderung in den folgenden Situationen bei:
* Das EFS sorgt dafür, dass ein Angreifer keine verschlüsselten Dateien über ein anderes Betriebssystem lesen kann: Der Angreifer muss einen passenden Schlüssel beibringen, mit dem sich der Inhalt entschlüsseln lässt. Sie können einen solchen Schlüssel auf einer Smartcard speichern, was die Sicherheit noch weiter erhöht.

* Die Stärke der Verschlüsselung durch EFS kann über eine Gruppenrichtlinie erzwungen werden.

* Sie können ein Angriff vereiteln, bei dem versucht wird, mit einem Brute-Force-Kennwortangriff auf die Daten eines Benutzers zuzugreifen, indem Sie die EFS-Schlüssel des Benutzers auf einer Smartcard ablegen oder auch BitLocker in Kombination mit EFS einsetzen, so dass dem Angreifer der Zugriff auf die Kennwort-Hashwerte und die zwischengespeicherten Anmeldeinformationen des Benutzers verweigert wird.

* Wenn Sie die Verschlüsselung des Ordners mit den eigenen Dateien eines Benutzers per Gruppenrichtlinie erzwingen, kann ein Angreifer nicht mehr auf die vertraulichen Daten dieses Benutzers zugreifen. Sie können auch die Verschlüsselung für andere Pfade oder für die gesamte Datenpartition des Benutzers mit einem Anmeldeskript erzwingen.

* Mit EFS ist die Verschlüsselung mehrerer Laufwerke und Netzwerkfreigaben möglich.

* EFS schützt den Inhalt der Systemauslagerungsdatei und des Offlinedateicache.

 


#### Überlegungen zur Risikominderung

Mit EFS in Windows Vista lassen sich die Risiken aus dem vorangegangenen Abschnitt „Risikobewertung“ mindern. Vor der Bereitstellung des EFS ist allerdings Folgendes zu beachten:
* Sie müssen bewährte Verfahren umsetzen, die alle Anforderungen hinsichtlich der Schlüsselverwaltung und der Datenwiederherstellung erfüllen. Wenn keine zuverlässigen, eindeutig definierten Verfahren bestehen, sind wichtige Daten unter Umständen nicht mehr abrufbar, wenn die zugehörigen Schlüssel verloren gehen.

* Im normalen Betrieb ist die Mehrbelastung durch EFS nicht wahrnehmbar. Falls die Systemleistung einen hohen Stellenwert einnimmt, führen Sie ausführliche Tests durch, um so sicherzustellen, dass die Leistung durch EFS nicht beeinträchtigt wird.

* Wenn Sie EFS auf einem Volume aktivieren, können Sie die Dateien auf diesem Volume nicht gleichzeitig komprimieren.

* Falls notwendig, stellen Sie weitere Skripts bereit, mit denen Ordner mit vertraulichen Daten verschlüsselt werden, und testen Sie diese Skripts.

* Benutzer und IT-Mitarbeiter müssen richtig geschult werden, um die folgenden Probleme zu vermeiden:
* Kopieren oder Verschieben von Dateien von einem verschlüsselten an einen unverschlüsselten Speicherort, wobei die Gefahr besteht, dass die Dateien als Dateien mit Klartext formatiert werden.
 

* Kein Verschlüsseln von verborgenen Ordnern, in denen Sicherungskopien der derzeit bearbeiteten Dateien durch die Anwendungen abgelegt werden.
 

 

* Testen Sie die EFS-Konfiguration gründlich, und stellen Sie so sicher, dass die Verschlüsselung für alle Ordner mit vertraulichen Dateien aktiviert ist (z. B. Ordner mit den eigenen Dateien, Desktop, temporäre Ordner).

 

**Hinweis:** EFS kann nur mit Windows Vista Business Edition, Enterprise Edition und Ultimate Edition bereitgestellt werden.


#### Verfahren zur Risikominderung

Ermitteln Sie die bestmögliche Konfiguration von EFS zum Schutz vertraulicher Daten auf den verwalteten Clientcomputern mithilfe des nachstehenden Verfahrens zur Risikominderung.

**So verwenden Sie dieses Verfahren zur Risikominderung**
* Informieren Sie sich über die Technologien und Funktionen von EFS.

**Hinweis**: Weitere Informationen finden Sie im Artikel [Vorgehensweisen bei Verwendung des Verschlüsselnden Dateisystems](http://support.microsoft.com/kb/223316).

* Beurteilen Sie die Notwendigkeit von EFS in Ihrer Arbeitsumgebung.

* Ziehen Sie die Konfiguration von EFS mithilfe von Gruppenrichtlinien in Erwägung.

* Ermitteln Sie, welche Computersysteme und Benutzer EFS benötigen.

* Ermitteln Sie den Umfang des erforderlichen Schutzes. Beispiel: Ist der Einsatz von Smartcards mit EFS in Ihrer Organisation vorgeschrieben?

* Konfigurieren Sie EFS gemäß Ihrer Arbeitsumgebung mithilfe von Gruppenrichtlinien.

 

Spezielle Schritte zur Risikominderung bei EFS

Die Einstellungen im folgenden Abschnitt ermöglichen die Verwaltung von EFS mit Gruppenrichtlinien:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Richtlinien öffentlicher Schlüssel\Verschlüsselndes Dateisystem**

Um einen Datenwiederherstellungs-Agenten (Data Recovery Agent, DRA) hinzuzufügen oder zu erstellen, klicken Sie mit der rechten Maustaste auf **Verschlüsselndes Dateisystem**, und klicken Sie dann im Dialogfeld **Eigenschaften von Verschlüsselndes Dateisystem** auf **Eigenschaften.**  


**Abbildung 3.1 Das Dialogfeld „Eigenschaften von Verschlüsselndes Dateisystem“**
 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/dd443715.vsgf0301_big(de-de,technet.10).gif)
Auch die vier Gruppenrichtlinienvorlagen in der nachstehenden Tabelle enthalten verschiedene EFS-Einstellungen.

**Tabelle 3.4: EFS-Gruppenrichtlinieneinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Vorlage und Einstellung

</th>

<th style="border:1px solid black;">

Pfad und Beschreibung

</th>

<th style="border:1px solid black;">

Standardeinstellung in Windows Vista

</th>

</tr>

<tr>

<td style="border:1px solid black;">


**GroupPolicy.admx**  
Richtlinienverarbeitung der EFS-Wiederherstellung

</td>

<td style="border:1px solid black;">


**Computerkonfiguration\**  
**Administrative Vorlagen\**  
**System\Gruppenrichtlinie**  
Mit dieser Einstellung bestimmen Sie den Zeitpunkt, zu dem die Verschlüsselungsrichtlinien aktualisiert werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**EncryptFilesonMove.admx**  
Dateien, die in verschlüsselte Ordner verschoben werden, nicht automatisch verschlüsseln

</td>

<td style="border:1px solid black;">


**Computerkonfiguration\**  
**Administrative Vorlagen\**  
**System\**  
Mit dieser Einstellung werden Dateien, die in einen verschlüsselten Ordner verschoben werden, nicht durch Windows Explorer verschlüsselt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**OfflineFiles.admx**  
Offlinedateicache verschlüsseln

</td>

<td style="border:1px solid black;">


**Computerkonfiguration\**  
**Administrative Vorlagen\**  
**Netzwerk\Offlinedateien\**  
Mit dieser Einstellung legen Sie fest, ob Offlinedateien verschlüsselt werden sollen.

**Hinweis**   Bei Windows XP werden diese Dateien mit dem Systemschlüssel verschlüsselt, bei Windows Vista hingegen mit dem Schlüssel des Benutzers.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**Search.admx**  
Indizierung verschlüsselter Dateien zulassen

</td>

<td style="border:1px solid black;">


**Computerkonfiguration\**  
**Administrative Vorlagen\**  
**Windows-Komponenten\**  
**Suche\**  
Diese Einstellung ermöglicht die Indizierung verschlüsselter Objekte durch die Windows-Suche.

**Hinweis**   Die Indizierung verschlüsselter Dateien kann zu Problemen im Hinblick auf die Datensicherheit führen. Der Index ist zudem nicht angemessen durch EFS oder andere Maßnahmen geschützt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


In dieser Tabelle werden die einzelnen Einstellungen kurz beschrieben. Weitere Informationen zu einer bestimmten Einstellung finden Sie im Gruppenrichtlinienobjekt-Editor auf der Registerkarte **Erklärung** dieser Einstellung.
 
[Zum Seitenanfanq](#mainsection)  



### Rechteverwaltungsdienste

Die Rechteverwaltungsdienste (Rights Management Services, RMS) sorgen für die Durchsetzung von Sicherheits- und Nutzungsrichtlinien für vertrauliche E-Mails, Dokumente, Webinhalte und andere Informationen. Bei RMS werden die Daten fortlaufend verschlüsselt, so dass beim Transport einer Datei oder einer E-Mail-Meldung im Unternehmen oder über das Internet nur die Benutzer den Zugriff darauf erhalten, die über eine entsprechende Authentifizierung und ausdrückliche Autorisierung verfügen. RMS besteht aus drei Komponenten:
* **RMS-Server.**   Windows Vista erfordert Windows Rights Management Services für Windows Server 2003 (oder höher).

* **RMS-Client.**   Dieser Client ist Bestandteil von Windows Vista.

* **RMS-Plattform oder -Anwendung.**   Diese Plattform oder Anwendung verschlüsselt und steuert die Nutzung der verwalteten Daten.

 


#### Risikobewertung

RMS mindert das Risiko in Unternehmen, dass Unbefugte vertrauliche Daten einsehen können, die entweder aus Versehen oder in böswilliger Absicht an nicht autorisierte Benutzer verteilt oder für diese zugänglich gemacht wurden. Beispiele für diese Art von Risiken:
* Nicht autorisierte Benutzer schnüffeln im Netzwerk herum, greifen auf USB-Flash-Laufwerke und mobile Festplatten zu oder erhalten Zugang zu unzureichend geschützten Serverfreigaben und Speicherbereichen.

* Autorisierte Benutzer senden vertrauliche Daten an nicht autorisierte Empfänger innerhalb oder außerhalb des Unternehmens.

* Autorisierte Benutzer kopieren oder verschieben vertrauliche Daten an nicht autorisierte Speicherorte oder Anwendungen oder von einem autorisierten Gerät auf ein nicht autorisiertes Gerät, z. B. auf ein Wechselspeichergerät.

* Autorisierte Benutzer eröffnen nicht autorisierten Benutzern über Peer-to-Peer-Technologien (P2P) oder über Instant Messaging versehentlich den Zugang zu vertraulichen Daten.

* Autorisierte Benutzer drucken vertrauliche Dateien, und die gedruckten Dokumente werden von nicht autorisierten Benutzern gefunden und verteilt, kopiert oder per Fax oder E-Mail verschickt.

 


#### Risikominderung

Damit die Daten, die die Benutzer gemeinsam nutzen und zur Zusammenarbeit heranziehen, unabhängig von den jeweiligen Schutzmaßnahmen effektiv abgesichert sind, empfiehlt Microsoft, die Daten direkt mit RMS zu schützen, so dass ein nahtloser Schutz der Daten bei der Übertragung zwischen Hosts, Geräten und Freigaben gewährleistet ist.


#### Überlegungen zur Risikominderung

Mit RMS lassen sich die Risiken aus dem vorangegangenen Abschnitt „Risikobewertung“ mindern. Vor der Bereitstellung von RMS ist allerdings Folgendes zu beachten:
* RMS erfordert Windows Rights Management Services für Windows Server 2003 (oder höher) als RMS-Server. Auf dem Clientcomputer müssen zudem RMS-fähige Anwendungen installiert sein.

* Um die SharePoint-RMS-Integration nutzen zu können, bei der die Dokumente und Daten auf SharePoint-Sites durch RMS geschützt werden, benötigen Sie Microsoft SharePoint® Server.

* Soll die optionale Smartcard-Integration der RMS-Lösung genutzt werden, stellen Sie sicher, dass alle Clientcomputer, über die Sie auf die Inhalte zugreifen, mit den Smartcards kompatibel ist.

* Für den gemeinsamen Einsatz webgestützter Anwendungen wie Outlook Web Access (OWA) mit RMS ist das Rechteverwaltungs-Add-On für Internet Explorer erforderlich.

* IT-Mitarbeiter müssen entsprechend geschult werden, damit sie RMS problemlos bereitstellen, für den Support sorgen und die Fehlerbehebung vornehmen können.

 


#### Verfahren zur Risikominderung

Ermitteln Sie die bestmögliche Konfiguration von RMS zum Schutz vertraulicher Daten auf den verwalteten Clientcomputern mithilfe des nachstehenden Verfahrens zur Risikominderung.

**So verwenden Sie dieses Verfahren zur Risikominderung**
* Informieren Sie sich über die Technologien und Funktionen von RMS.

**Hinweis**   Weitere Informationen zu RMS finden Sie im Windows Server 2003 Technology Center zu [Windows Rights Management Services](http://www.microsoft.com/windowsserver2003/technologies/rightsmgmt/default.mspx) (engl.).

* Beurteilen Sie die Notwendigkeit von RMS in Ihrer Arbeitsumgebung.

* Ermitteln Sie den Grad der Unterstützung von RMS durch die Anwendungen und Dienste.

* Erwägen Sie potenzielle Architekturen für die RMS-Bereitstellung, beispielsweise:
* Einzelner Server (oder einzelner Cluster)
 

* Einzelne Zertifizierung, einzelne Lizenz
 

* Einzelne Zertifizierung, mehrere Lizenzen
 

* Mehrere Zertifizierungen, einzelne Lizenz
 

* Mehrere Zertifizierungen, mehrere Lizenzen
 

 

* Ermitteln Sie die Daten, die mit RMS geschützt werden sollen.

* Ermitteln Sie die Benutzer und Gruppen, die Zugriff auf bestimmte Daten benötigen.

* Konfigurieren Sie RMS so, dass nur der wirklich benötigte Zugriff auf Daten möglich ist.

 


#### Verwalten von RMS mithilfe von Gruppenrichtlinien

Die Gruppenrichtlinieneinstellungen für die Konfiguration von RMS werden nicht im Rahmen der Installation von Windows Vista festgelegt. RMS ist in erster Linie eine servergestützte Lösung; die Konfiguration für das Verhalten der Dienste sollte daher direkt auf dem RMS-Server erfolgen.

RMS-fähige Anwendungen besitzen zudem ggf. eigene Einstellungen, mit denen die Verarbeitung RMS-geschützter Inhalte geregelt ist. RMS-bezogene Einstellungen sind beispielsweise in Microsoft Office 2003 (und höher) sowie in Anwendungen wie Microsoft Outlook® und Microsoft Word zu finden. Weitere Informationen zu diesen Einstellungen finden Sie im Artikel [Office 2003 Policy Template Files and Deployment Planning Tools](http://office.microsoft.com/en-us/ork2003/ha011513711033.aspx) (engl.).
 
[Zum Seitenanfanq](#mainsection)  



### Gerätesteuerung

Die Fähigkeit von Benutzern, ihren Clientcomputern neue Plug &amp; Play-Hardware (PnP) wie USB-Schlüssellaufwerke oder andere Wechselspeichergeräte hinzuzufügen, bereitet IT-Administratoren beträchtliche Probleme mit der Sicherheit. Diese Geräte erschweren nicht nur die Verwaltung der Clientcomputer, wenn die Benutzer darauf nicht unterstützte Hardware installieren, sondern sie können eine echte Bedrohung für die Datensicherheit darstellen.

Ein böswilliger Benutzer könnte möglicherweise mithilfe eines Wechselspeichergeräts geistiges Eigentum eines Unternehmens entwenden. Wenn ein Angreifer schädliche Software auf einem Wechselspeichergerät mit einem Skript zur automatischen Ausführung konfiguriert, könnte er damit diese Software auf einem unbeaufsichtigten Clientcomputer installieren.

Bei Windows Vista sind IT-Administratoren mithilfe von Gruppenrichtlinien in der Lage, die Installation von nicht unterstützten oder nicht zulässigen Geräten zu überwachen und zu steuern. Sie können beispielsweise Benutzern die Installation ganzer Geräteklassen (z. B. Drucker) gestatten, hingegen jegliche Arten von Wechselspeichergeräten untersagen. Ein Administrator kann die Genehmigung erhalten, diese Richtlinien außer Kraft zu setzen und so auch nicht genehmigte Hardware zu installieren.

Dabei ist jedoch zu beachten, dass ein Gerät nicht für bestimmte Benutzer installiert wird, sondern für einen Computer. Sobald ein Benutzer ein Gerät installiert, steht dieses Gerät in der Regel allen Benutzern dieses Computers zur Verfügung. Windows Vista unterstützt nunmehr die Zugriffssteuerung auf Benutzerebene für den Lese- und Schreibzugriff auf installierte Geräte. So können Sie beispielsweise den uneingeschränkten Schreib- und Lesezugriff auf installierte Geräte (z. B. ein USB-Flash-Laufwerk) für ein bestimmtes Benutzerkonto gestatten und einem anderen Benutzerkonto auf demselben Computer nur den Lesezugriff gewähren.

Weitere Informationen zur Gerätesteuerung und zu deren Konfiguration finden Sie in der [*Schritt-für-Schritt-Anleitung zur Steuerung der Geräteinstallation über Gruppenrichtlinien*](https://technet.microsoft.com/de-de/library/1495196d-06d0-4ddc-85f3-953ddbb41e7e(v=TechNet.10)).


#### Risikobewertung

Das unbefugte Hinzufügen oder Entfernen von Geräten stellt ein großes Sicherheitsrisiko dar, da ein Angreifer hierdurch in die Lage versetzt werden kann, schädliche Software auszuführen, Daten zu entfernen und unerwünschte Daten hinzuzufügen. Einige Beispiele hierfür:
* Ein autorisierter Benutzer könnte vertrauliche Dateien (versehentlich oder in voller Absicht) von einem autorisierten Gerät auf ein nicht autorisiertes Wechselspeichergerät kopieren. Dies umfasst auch das Kopieren von Dateien aus einem verschlüsselten Speicherort an einen nicht verschlüsselten Speicherort auf einem Wechselspeichergerät.

* Ein Angreifer könnte sich bei Windows Vista anmelden und Daten auf ein Wechselspeichergerät kopieren.

* Wenn ein Angreifer bösartige Software auf einem Wechselspeichergerät mit einem Skript für die automatische Ausführung konfiguriert, könnte er damit diese Software auf einem unbeaufsichtigten Clientcomputer installieren.

* Ein Angreifer könnte ein nicht autorisiertes Gerät zur Aufzeichnung von Tastatureingaben installieren, mit dem er die Angaben zu den Benutzerkonten aufzeichnen und so später einen weiteren Angriff starten könnte.

 


#### Risikominderung

Um diese Risiken zu mindern, empfiehlt Microsoft, die verwalteten Computersysteme vor der Installation und der Nutzung nicht autorisierter Geräte zu schützen. Mithilfe von Gruppenrichtlinieneinstellungen können Sie beispielsweise die Nutzung von PnP-Geräten (z. B. USB-Flash-Laufwerke) und anderen Wechselspeichergeräten steuern.


#### Überlegungen zur Risikominderung

Mit Gruppenrichtlinien in Windows Vista lassen sich die Risiken aus dem vorangegangenen Abschnitt „Risikobewertung“ mithilfe der Einstellungen für die Geräteinstallation mindern. Bevor Sie jedoch die Gerätesteuerung für die Clientcomputer in Ihrer Arbeitsumgebung bereitstellen, beachten Sie die folgenden Überlegungen zur Risikominderung:
* Wenn Sie Einschränkungen für die Geräte festlegen, kann sich dies störend auf die normale (legitime) gemeinsame Nutzung von Dateien auswirken, oder mobile Benutzer können nicht mehr so effektiv wie gewohnt arbeiten.

* Durch die Einschränkungen für die Geräte ist es unter Umständen nicht mehr möglich, einen USB-Schlüssel im Rahmen der BitLocker-Laufwerkverschlüsselung einzusetzen. Ist beispielsweise die Richtlinieneinstellung „Wechselmedien: Schreibzugriff verweigern“ für einen Benutzer in Kraft, so kann das BitLocker-Setupprogramm selbst dann nicht den Systemstartschlüssel auf ein USB-Flash-Laufwerk schreiben, wenn dieser Benutzer als Administrator angemeldet ist.

* Einige Geräte besitzen eine ID sowohl als Wechselspeichergerät als auch als lokaler Speicher, beispielsweise einige bootfähige USB-Flash-Laufwerke. Testen Sie daher die Gruppenrichtlinienobjekte gründlich, damit gewährleistet ist, dass die richtigen Geräte mit den richtigen Einschränkungen und Zulassungen versehen sind.

 


#### Verfahren zur Risikominderung

Ermitteln Sie die bestmögliche Konfiguration der Gerätesteuerung zum Schutz vertraulicher Daten auf den verwalteten Clientcomputern mithilfe des nachstehenden Verfahrens zur Risikominderung.

**So verwenden Sie dieses Verfahren zur Risikominderung**
* Informieren Sie sich über die Gerätesteuerungsfunktionen von Windows Vista.

**Hinweis**: Weitere Informationen finden Sie in der [*Schritt-für-Schritt-Anleitung zur Steuerung der Geräteinstallation über Gruppenrichtlinien*](https://technet.microsoft.com/de-de/library/1495196d-06d0-4ddc-85f3-953ddbb41e7e(v=TechNet.10)) (engl.).

* Beurteilen Sie die Notwendigkeit der Gerätesteuerung in Ihrer Arbeitsumgebung.

* Untersuchen Sie die Gruppenrichtlinieneinstellungen für die Gerätesteuerung.

* Ermitteln Sie die notwendigen Wechselspeichergeräte in der Arbeitsumgebung, und halten Sie die erforderliche Hardware- oder Kompatibilitäts-IDs dieser Geräte fest.

* Ermitteln Sie, welche Computersysteme und Benutzer die Wechselspeichergeräte benötigen.

* Konfigurieren Sie die Gruppenrichtlinien so, dass die Installation explizit erforderlicher Geräteklassen zugelassen wird.

* Konfigurieren Sie die Gruppenrichtlinien so, dass die Installation von Geräten auf Computersystemen zugelassen wird, die diese Geräte explizit benötigen.

 

Steuern der Geräteinstallation mithilfe von Gruppenrichtlinien

Zur Steuerung der Geräteinstallation empfiehlt Microsoft, die Gruppenrichtlinienvorlage „DeviceInstallation.admx“ zu verwenden. Tabelle 3.5 enthält die Gruppenrichtlinieneinstellungen, die in dieser Vorlage zur Verfügung stehen. Diese Einstellungen können im Gruppenrichtlinienobjekt-Editor im folgenden Verzeichnis konfiguriert werden:

**Computerkonfiguration\Administrative Vorlagen\System\Device Installation\Device Installation Restrictions**

**Tabelle 3.5 Einstellungen für die USB-Gerätesteuerung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinieneinstellung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

<th style="border:1px solid black;">

Standardeinstellung in Windows Vista

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Allow administrators to override Device Installation policies (Außerkraftsetzen der Geräteinstallationsrichtlinien durch Administratoren zulassen)

</td>

<td style="border:1px solid black;">


Mitglieder der Administratorengruppe können die Treiber für jegliche Geräte installieren und aktualisieren, unabhängig von anderen Richtlinieneinstellungen. Ansonsten unterliegen auch Administratoren sämtlichen Richtlinien, die die Geräteinstallation einschränken.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Allow installation of devices using drivers that match these device setup classes (Installation von Geräten mit Treibern in diesen Gerätesetupklassen zulassen)

</td>

<td style="border:1px solid black;">


Diese Einstellung enthält eine Liste der GUIDs von Gerätesetupklassen, die die Benutzer installieren können, sofern diese Installation nicht durch die folgenden Richtlinieneinstellungen explizit untersagt ist:  
**Prevent installation of devices that match these device IDs**  
**Prevent installation of devices for these device classes**  
**Prevent installation of removable devices**  
Verwenden Sie diese Einstellung nur dann, wenn die Einstellung **Prevent installation of devices not described by other policy settings** aktiviert ist.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prevent installation of devices using drivers that match these device setup classes (Installation von Geräten mit Treibern in diesen Gerätesetupklassen verhindern)

</td>

<td style="border:1px solid black;">


Diese Einstellung enthält eine benutzerdefinierte Meldung, die dem Benutzer im Titel des Benachrichtigungshinweises angezeigt werden soll, sobald die Richtlinie die Installation eines Geräts verhindert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Display a custom message when installation is prevented by policy (balloon title) (Benutzerdefinierte Meldung (Titel im Benachrichtigungshinweis) anzeigen, wenn die Installation durch die Richtlinie verhindert wird)

</td>

<td style="border:1px solid black;">


Diese Einstellung enthält eine benutzerdefinierte Meldung, die im Titel des Benachrichtigungshinweises angezeigt werden soll, sobald eine Einstellung in einer Richtlinie die Installation eines Geräts verhindert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Display a custom message when installation is prevented by policy (balloon text) (Benutzerdefinierte Meldung (Text im Benachrichtigungshinweis) anzeigen, wenn die Installation durch die Richtlinie verhindert wird)

</td>

<td style="border:1px solid black;">


Diese Einstellung enthält eine benutzerdefinierte Meldung, die als Text des Benachrichtigungshinweises angezeigt werden soll, sobald die Richtlinie die Installation eines Geräts verhindert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Allow installation of devices that match any of these device IDs (Installation von Geräten mit einer dieser Geräte-IDs zulassen)

</td>

<td style="border:1px solid black;">


Diese Einstellung enthält eine Liste der Plug &amp; Play-Hardware-IDs und kompatiblen IDs für Geräte, die die Benutzer installieren können, sofern diese Installation nicht durch die folgenden Einstellungen ausdrücklich untersagt ist:  
**Prevent installation of devices that match these device IDs**  
**Prevent installation of devices for these device classes**  
**Prevent installation of removable devices**  
Verwenden Sie diese Einstellung nur dann, wenn die Einstellung **Prevent installation of devices not described by other policy settings** aktiviert ist.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prevent installation of devices that match any of these device IDs (Installation von Geräten mit einer dieser Geräte-IDs verhindern)

</td>

<td style="border:1px solid black;">


Diese Einstellung enthält eine Liste der Plug &amp; Play-Hardware-IDs und kompatiblen IDs für Geräte, die die Benutzer nicht installieren können.  
**Hinweis**:   Diese Richtlinieneinstellung hat Vorrang vor allen Richtlinieneinstellungen, mit denen die Installation eines Geräts zugelassen wird.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prevent installation of removable devices (Installation von Wechselgeräten verhindern)

</td>

<td style="border:1px solid black;">


Wenn Sie diese Einstellung aktivieren, können die Benutzer keine Wechselspeichergeräte installieren, und es nicht möglich, die Treiber der vorhandenen Wechselspeichergeräte zu aktualisieren.  
**Hinweis**:   Diese Richtlinieneinstellung hat Vorrang vor allen Richtlinieneinstellungen, mit denen die Installation eines Geräts zugelassen wird.  
Diese Richtlinie wird nur dann angewendet, wenn aus den Treibern des Geräts eindeutig und richtig hervorgeht, dass das betreffende Gerät tatsächlich ein Wechselspeichergerät ist. Weitere Informationen finden Sie in der [*Schritt-für-Schritt-Anleitung zur Steuerung der Geräteinstallation über Gruppenrichtlinien*](https://technet.microsoft.com/de-de/library/1495196d-06d0-4ddc-85f3-953ddbb41e7e(v=TechNet.10)) (engl.).

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prevent installation of devices not described by other policy settings (Installation von Geräten verhindern, die nicht in anderen Richtlinieneinstellungen beschrieben sind)

</td>

<td style="border:1px solid black;">


Wenn Sie diese Einstellung aktivieren, können Sie die Treiber jeglicher Geräte nicht aktualisieren, die nicht in den folgenden Einstellungen beschrieben sind:  
**Allow installation of devices that match these device IDs**  
**Allow installation of devices for these device classes**

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


In dieser Tabelle werden die einzelnen Einstellungen kurz beschrieben. Weitere Informationen zu einer bestimmten Einstellung finden Sie im Gruppenrichtlinienobjekt-Editor auf der Registerkarte **Erklärung** dieser Einstellung.

Steuern der Gerätenutzung mithilfe von Gruppenrichtlinien

Mit Windows Vista können Sie nicht nur die Installation von Geräten steuern, sondern auch die Zugriffsebene auf bestimmte Geräteklassen, die die Benutzer nach deren Installation erhalten sollen. Die nachstehenden Tabellen zeigen zwei weitere Vorlagen mit Einstellungen, die sich auf das Verhalten der Geräte auswirken können. Die Vorlage „RemovableStorage.admx“ enthält die folgende Einstellung für Wechselspeichergeräte und befindet sich im Gruppenrichtlinienobjekt-Editor im folgenden Verzeichnis:

**Computerkonfiguration\Administrative Vorlagen\System\Removable Storage Access**

**Tabelle 3.6 Geräteeinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinieneinstellung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

<th style="border:1px solid black;">

Standardeinstellung in Windows Vista

</th>

</tr>

<tr>

<td style="border:1px solid black;">


All Removable Storage classes: Deny all access (Alle Wechselspeichergeräteklassen: Jeglichen Zugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung konfigurieren Sie den Zugriff auf alle Klassen von Wechselspeichergeräten.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


All Removable Storage: Allow direct access in remote sessions (Alle Wechselspeichergeräteklassen: Direkten Zugriff in Remotesitzungen zulassen)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung erhalten standardmäßige Benutzerkonten den Zugriff auf Wechselspeichergeräte in Remotesitzungen. In der Standardkonfiguration ist dieser Zugriff für Remotesitzungen nicht zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CD and DVD: Deny read access (CD und DVD: Lesezugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Lesezugriff auf die CD- und DVD-Laufwerke dieser Wechselspeichergeräteklasse untersagt. In der Standardeinstellung ist der Lesezugriff zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CD and DVD: Deny write access (CD und DVD: Schreibzugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Schreibzugriff auf die Wechselspeichergeräteklasse der CD- und DVD-Laufwerke unterbunden. In der Standardeinstellung ist der Schreibzugriff auf diese Geräteklasse zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Custom Classes: Deny read access (Benutzerdefinierte Klassen: Lesezugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Lesezugriff auf benutzerdefinierte Geräteklassen untersagt. In der Standardeinstellung ist der Lesezugriff zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Custom Classes: Deny write access (Benutzerdefinierte Klassen: Schreibzugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Schreibzugriff auf benutzerdefinierte Geräteklassen untersagt. In der Standardeinstellung ist der Schreibzugriff auf diese Geräteklasse zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Floppy Drives: Deny read access (Diskettenlaufwerke: Lesezugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Lesezugriff auf Diskettenlaufwerke untersagt. In der Standardeinstellung ist der Lesezugriff zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Floppy Drives: Deny write access (Diskettenlaufwerke: Schreibzugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Schreibzugriff auf Diskettenlaufwerke untersagt. In der Standardeinstellung ist der Schreibzugriff auf diese Geräteklasse zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Removable Disks: Deny read access (Wechselmedien: Lesezugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Lesezugriff auf Wechselfestplatten untersagt. In der Standardeinstellung ist der Lesezugriff zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Removable Disk: Deny write access (Wechselmedien: Schreibzugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Schreibzugriff auf Wechselfestplatten untersagt. In der Standardeinstellung ist der Schreibzugriff auf diese Geräteklasse zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Tape Drives: Deny read access (Bandlaufwerke: Lesezugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Lesezugriff auf Bandlaufwerke untersagt. In der Standardeinstellung ist der Lesezugriff zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Tape Drives: Deny write access (Bandlaufwerke: Schreibzugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Schreibzugriff auf Bandlaufwerke untersagt. In der Standardeinstellung ist der Schreibzugriff auf diese Geräteklasse zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


WPD Devices: Deny read access (WPD-Geräte: Lesezugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Lesezugriff auf tragbare Windows-Geräte verweigert, z. B. auf Medienwiedergabegeräte und Mobiltelefone. In der Standardeinstellung ist der Lesezugriff zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


WPD Devices: Deny write access (WPD-Geräte: Schreibzugriff verweigern)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung wird der Schreibzugriff auf tragbare Windows-Geräte verweigert, z. B. auf Medienwiedergabegeräte und Mobiltelefone. In der Standardeinstellung ist der Schreibzugriff auf diese Geräteklasse zulässig.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


In dieser Tabelle werden die einzelnen Einstellungen kurz beschrieben. Weitere Informationen zu einer bestimmten Einstellung finden Sie im Gruppenrichtlinienobjekt-Editor auf der Registerkarte **Erklärung** dieser Einstellung.

Steuern der Funktionen für automatische Wiedergabe und AutoAusführen mithilfe von Gruppenrichtlinien

Die nachstehenden Einstellungen in der Vorlage „Autoplay.admx“ wirken sich auf das Verhalten der automatischen Wiedergabe und der AutoAusführen-Funktion von Wechselspeichergeräten und Wechselmedien in Windows Vista aus. Die Einstellungen für diese Vorlage finden Sie im Gruppenrichtlinienobjekt-Editor im folgenden Verzeichnis:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\AutoPlay Policies**

**Tabelle 3.7 Richtlinieneinstellungen für die automatische Wiedergabe**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinieneinstellung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

<th style="border:1px solid black;">

Standardeinstellung in Windows Vista

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Turn off Autoplay (Automatische Wiedergabe deaktivieren)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Sie die automatische Wiedergabe für CD-, DVD-ROM- und Wechsellaufwerke oder für alle Laufwerke gleichzeitig deaktivieren.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Default behavior for AutoRun (Standardverhalten für AutoAusführen)

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung konfigurieren Sie das Standardverhalten für AutoAusführen-Befehle. Standardmäßig wird der Benutzer in Windows Vista aufgefordert, die Ausführung eines AutoAusführen-Befehls zu bestätigen.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


In dieser Tabelle werden die einzelnen Einstellungen kurz beschrieben. Weitere Informationen zu einer bestimmten Einstellung finden Sie im Gruppenrichtlinienobjekt-Editor auf der Registerkarte **Erklärung** dieser Einstellung.

Diese Einstellungen befinden sich auch in der Benutzerkonfiguration im Gruppenrichtlinienobjekt-Editor im folgenden Verzeichnis:

**Benutzerkonfiguration\Administrative Vorlagen\Windows-Komponenten\AutoPlay Policies**

Bei einem Konflikt mit den Einstellungen für die Gerätesteuerung erhält die Einstellung in der Computerkonfiguration den Vorrang vor der Einstellung in der Benutzerkonfiguration.

**Hinweis**: In einigen Richtlinieneinstellungen werden GUIDs für Gerätesetupklassen verwendet, in anderen dagegen GUIDs für Plug &amp; Play-Gerätesetupklassen. Weitere Informationen finden Sie im Abschnitt über das [Auswählen von Treibern beim Setup](http://msdn2.microsoft.com/en-us/library/ms791096.aspx) (engl.).
 
[Zum Seitenanfanq](#mainsection)  



### Weitere Informationen

Weitere Informationen zu den neuen und überarbeiteten Sicherheitsfunktionen und Technologien zum Schutz vertraulicher Daten in Windows Vista finden Sie hier:
* [Vorgehensweisen bei Verwendung des Verschlüsselnden Dateisystems](http://support.microsoft.com/kb/223316)

* [BitLocker Drive Encryption](http://www.microsoft.com/technet/windowsvista/security/bitlockr.mspx) (engl.)

* [*Schritt-für-Schritt-Anleitung zur Steuerung der Geräteinstallation über Gruppenrichtlinien*](https://technet.microsoft.com/de-de/library/1495196d-06d0-4ddc-85f3-953ddbb41e7e(v=TechNet.10))


* [First Look: New Security Features in Windows Vista](https://www.microsoft.com/technet/technetmag/issues/2006/05/firstlook/default.aspx) (engl.)

* [Windows Vista - Verbesserungen aus den Bereichen Sicherheit und Datenschutz](https://technet.microsoft.com/de-de/library/0024115e-c180-4573-9802-7eca9fc16a70(v=TechNet.10))


* [Encrypting File System](http://www.microsoft.com/technet/security/guidance/cryptographyetc/efs.mspx) (engl.)

* [Trusted Computing Group](http://www.trustedcomputinggroup.org/) (engl.)

* [Office 2003 Policy Template Files and Deployment Planning Tools](http://office.microsoft.com/en-us/ork2003/ha011513711033.aspx) (engl.)

* [Windows Server 2003 Technology Center – Windows Rights Management Services](http://www.microsoft.com/windowsserver2003/technologies/rightsmgmt/default.mspx) (engl.)

 
[Zum Seitenanfanq](#mainsection)
 


### In diesem Beitrag
* [Übersicht](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/default.mspx)
* [Kapitel 1: Implementieren der Sicherheitsbasis](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx)
* [Kapitel 2: Schutz vor Malware](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx)
* Kapitel 3: Schutz von vertraulichen Daten
* [Kapitel 4: Anwendungskompatibilität](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/application_compatibility.mspx)
* [Kapitel 5: Hochsicherheit (SSLF)](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/specialized_security.mspx)
* [Anhang A: Sicherheitsrelevante Gruppenrichtlinieneinstellungen](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/security_group_policy_settings.mspx)
 

**Download**  


[Windows Vista-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=74028) (engl.)

**Update Notifications**  


[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden.](http://go.microsoft.com/fwlink/?linkid=54982) (engl.)

**Feedback**  


[Senden Sie uns Ihre Kommentare und Anregungen.](mailto:secwish@microsoft.com?subject=windows vista security guide) (engl.)
 

<table style="border:1px solid black;">

<tr>

<td style="border:1px solid black;">

[Zum Seitenanfanq](#mainsection)

</td>

<td style="border:1px solid black;">

[![](https://technet.microsoft.com/de-de/Dd443715.pageLeft(de-de,TechNet.10).gif "Dd443715.pageLeft(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx)
5 von 7[![](https://technet.microsoft.com/de-de/Dd443715.pageRight(de-de,TechNet.10).gif "Dd443715.pageRight(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/application_compatibility.mspx)

</td>

</tr>

</table>





