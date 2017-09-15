---
TOCTitle: 'RMS – Häufig gestellte Fragen: Bereitstellung'
Title: 'RMS – Häufig gestellte Fragen: Bereitstellung'
ms:assetid: '5559ae65-77ae-4e0b-bfd8-3512409ed29b'
ms:contentKeyID: 18118846
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720274(v=WS.10)'
---

RMS – Häufig gestellte Fragen: Bereitstellung
=============================================

RMS-Bereitstellung – Häufig gestellte Fragen
--------------------------------------------

-   [Wenn die in RMS verwendeten Sicherheitsprinzipale Mitglieder der globalen Adressliste (Global Address List, GAL) sind, besteht dann eine Abhängigkeit von der Exchange-Version?](#bkmk_20)
-   [Welche Rolle hat SQL Server in RMS?](#bkmk_21)
-   [Muss sich der Computer eines Benutzers für die Verwendung von RMS in derselben Domäne befinden wie der RMS-Stammcluster?](#bkmk_22)
-   [Welche Ports müssen in der internetseitigen Firewall und welche in der intranetseitigen Firewall für die Kommunikation mit RMS geöffnet sein, wenn ein Benutzer einen RMS-Server in einem Umkreisnetzwerk platzieren möchte?](#bkmk_23)
-   [Wie werden untergeordnete Server in einem rein lizenzierenden Cluster registriert, und muss etwas unternommen werden, um die Clients auf dieses Cluster hinzuweisen?](#bkmk_24)
-   [Welchen Vorteil hat die Verwendung eines rein lizenzierenden Clusters?](#bkmk_25)
-   [Welche Schritte müssen ausgeführt werden, um eine RMS-Installation vollständig zurückzusetzen (Rollback)?](#bkmk_26)
-   [Muss ich nach der Deinstallation des RMS-Clients mithilfe der Funktion „Software“ in der Systemsteuerung noch weitere Dateien entfernen?](#bkmk_27)
-   [Funktioniert RMS mit dem FAT-Dateisystem?](#bkmk_28)
-   [Welche Hardwarekonfiguration wird normalerweise für den von RMS verwendeten Datenbankserver empfohlen?](#bkmk_29)
-   [Wie wirkt sich die Verwendung des globalen Katalogs zur Gruppenerweiterung durch RMS auf die Arbeitsgeschwindigkeit des globalen Katalogservers aus?](#bkmk_30)
-   [Sind für RMS Schemaänderungen in Active Directory erforderlich?](#bkmk_31)
-   [Wird der Dienstverbindungspunkt (Service Connection Point, SCP) zwischen den verschiedenen Domänencontrollern in der Domäne, in der der RMS-Cluster installiert ist, automatisch repliziert?](#bkmk_32)
-   [Wie kann der RMS-Client installiert und konfiguriert werden, wenn die Benutzer auf ihren Computern nicht über Administratorberechtigungen verfügen?](#bkmk_33)
-   [Inwieweit ist RMS skalierbar?](#bkmk_35)
-   [Unterstützt RMS Hardwaresicherheitsmodule (Hardware Security Modules, HSMs), um die RMS-Schlüssel in der Hardware zu sichern?](#bkmk_36)

<span id="BKMK_20"></span>
#### Wenn die in RMS verwendeten Sicherheitsprinzipale Mitglieder der globalen Adressliste (Global Address List, GAL) sind, besteht dann eine Abhängigkeit von der Exchange-Version?

RMS hängt von Active Directory ab, Exchange tut dies nicht. Exchange 5.5 verwendet jedoch ein eigenes Verzeichnis und greift nicht auf Active Directory zurück. Stellen Sie sicher, dass jedes Benutzer- und Gruppenobjekt in Active Directory ein gültiges E-Mail-Attribut hat, das den vollständig qualifizierten Domänennamen enthält. Diese Prüfung wird bei Verwendung von Exchange 2000 oder höher automatisch ausgeführt.

<span id="BKMK_21"></span>
#### Welche Rolle hat SQL Server in RMS?

In RMS werden alle Dienstkonfigurationsdaten, Informationen zu Prinzipalen im System, sämtliche Protokollierungsdaten sowie Suchen während der Erweiterung von Active Directory und der Verteilerliste in einer Datenbank gespeichert bzw. zwischengespeichert. Die vollständige Funktionsfähigkeit von RMS wurde für SQL Server 2000 und SQL Server 2005 geprüft.

<span id="BKMK_22"></span>
#### Muss sich der Computer eines Benutzers für die Verwendung von RMS in derselben Domäne befinden wie der RMS-Server?

Der Computer des Benutzers muss nicht Mitglied derselben Domäne wie der RMS-Cluster sein, er muss jedoch das RMS-Cluster finden können. Die einfachste Möglichkeit für Clientcomputer, den RMS-Cluster zu finden, ist eine Active Directory-Suche über den Dienstverbindungspunkt (Service Connection Point, SCP). In den Registrierungseinstellungen des Clients kann aber auch festgelegt werden, dass der RMS-Cluster ohne eine Active Directory-Suche gefunden werden kann. Die genauen Registrierungseinstellungen hängen von der RMS-fähigen Anwendung ab.

<span id="BKMK_23"></span>
#### Welche Ports müssen in der internetseitigen Firewall und welche in der intranetseitigen Firewall für die Kommunikation mit RMS geöffnet sein, wenn ein Benutzer den RMS-Server in einem Umkreisnetzwerk platzieren möchte?

Die internen Benutzer benötigen Zugriff auf die RMS-Server, die Rechtekontozertifikate (Rights Account Certificates, RACs) und Nutzungslizenzen ausstellen. Der RMS-Server verwendet zum Abhören standardmäßig HTTP (TCP-Port 80) bzw. HTTPS (TCP-Port 443), je nachdem, ob der Server für die Verwendung von SSL konfiguriert ist. Deshalb müssen diese Ports in der internetseitigen Firewall geöffnet sein. Darüber hinaus müssen Sie weitere Ports öffnen, die von Mitgliedern einer Domäne in der intranetseitigen Firewall verwendet werden.

<span id="BKMK_24"></span>
#### Wie werden untergeordnete Server in einem rein lizenzierenden Cluster registriert, und muss etwas unternommen werden, um die Clients auf dieses Cluster hinzuweisen?

Wenn der erste RMS-Server im Stammcluster in einem Unternehmen installiert wird, erhält er vom Microsoft-Registrierungsdienst ein Server-Lizenzgeberzertifikat. Bei der Installation und Bereitstellung eines weiteren RMS-Servers können Sie diesen dem Stammcluster beitreten lassen oder ihn als Server in einem untergeordneten rein lizenzierenden Cluster registrieren. Wenn Sie sich für die Registrierung als Server in einem untergeordneten rein lizenzierenden Cluster entscheiden, sendet der RMS-Server eine Registrierungsanforderung an den RMS-Stammcluster. RMS-fähige Anwendungen geben an, wo eine Clientanwendung nach dem rein lizenzierenden Server suchen soll. Ein Beispiel für eine RMS-fähige Anwendung, die standardmäßig nach dem Stammcluster sucht, ist Office 2003. Dieses Verhalten kann mithilfe von Registrierungseinstellungen so geändert werden, dass die Anwendung nach dem neuen untergeordneten rein lizenzierenden Server sucht.

<span id="BKMK_25"></span>
#### Welchen Vorteil hat die Verwendung eines untergeordneten rein lizenzierenden Clusters?

Ein Vorteil besteht darin, dass auf diese Weise Abteilungen innerhalb einer Organisation voneinander getrennt werden können. Wenn keine vertrauenswürdige Veröffentlichungsdomäne zwischen RMS-Clustern aufgebaut wurde, können Inhalte nur von Benutzern abgerufen werden, die Zugriff auf einen bestimmten Lizenzierungsserver haben. So kann beispielsweise die Rechtsabteilung verhindern, dass Benutzer außerhalb der Abteilung ihre RMS-verschlüsselten E-Mails lesen können. Darüber hinaus können auf dem rein lizenzierenden Server verschiedene Optionen festgelegt werden, wie z. B. Vorlagen für Benutzerrechterichtlinien, Protokollierung, Mitgliedschaft in der Administratorengruppe und Ausschlussrichtlinien.

<span id="BKMK_26"></span>
#### Welche Schritte müssen ausgeführt werden, um eine RMS-Installation vollständig zurückzusetzen (Rollback)?

Mit den folgenden Schritten können Sie eine RMS-Installation vollständig rückgängig machen.

**So setzen Sie eine RMS-Installation zurück**
1.  Entfernen Sie mithilfe der RMS-Verwaltungswebsite den Dienstverbindungspunkt (Service Connection Point, SCP) für Ihren RMS-Cluster.

2.  Klicken Sie auf der Seite **Globale Verwaltung** auf **RMS von dieser Website entfernen**, um die Bereitstellung von RMS auf dem Server aufzuheben. Heben Sie zuerst die Bereitstellung unterregistrierter Server in rein lizenzierenden Clustern auf, bevor Sie mit der Aufhebung der Bereitstellung der Stammclusterserver beginnen.

3.  Klicken Sie in der **Systemsteuerung** auf **Software**, und entfernen Sie das Programm **Rights Management Services**.

4.  Entfernen Sie auf Ihrem Datenbankserver alle eventuell verbliebenen RMS-Datenbanken.

5.  Entfernen Sie das RMS-Dienstkonto aus der Liste der berechtigten Anmeldungen beim Datenbankserver, und entfernen Sie anschließend das Konto selbst aus Active Directory.

6.  Wenn die RMS-Clients unter Windows XP und Windows 2000 ausgeführt werden, entfernen Sie den RMS-Client von den Clientcomputern.

| ![](images/Cc720274.Important(WS.10).gif)Wichtig                                                                                                                                                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Danach können Sie keine durch Rechte geschützte Inhalte mehr öffnen. Für den Fall, dass RMS zum Schützen wertvoller Daten verwendet wurde, setzen Sie zuerst RMS außer Betrieb, bevor Sie die RMS-Installation zurücksetzen. |

<span id="BKMK_27"></span>
#### Muss ich nach der Deinstallation des RMS-Clients mithilfe der Funktion „Software“ in der Systemsteuerung noch weitere Dateien entfernen?

Obwohl es nicht unbedingt notwendig ist, können Sie die Lockbox aus dem Verzeichnis „%systemroot%\\system32“ löschen.

<span id="BKMK_28"></span>
#### Funktioniert RMS mit dem FAT-Dateisystem?

Ja, RMS funktioniert auch auf einem Computer mit dem Dateisystem FAT, obwohl die Verwendung des Dateisystems NTFS empfohlen wird.

<span id="BKMK_29"></span>
#### Welche Hardwarekonfiguration wird normalerweise für den von RMS verwendeten Datenbankserver empfohlen?

Die Protokollierungsdatenbank wächst schnell an, besonders in Umgebungen, in denen RMS häufig verwendet wird. Wenn Sie die Verwendung von SQL Server für Ihren Datenbankserver erwägen, sollten Sie SQL Server 2000 Enterprise Edition oder SQL Server 2005 Enterprise Edition unter Windows 2000 Advanced Server oder Windows Server 2003 Enterprise Edition in einem Cluster mit aktiver Standby-Konfiguration verwenden. In diesem Fall wird eine Konfiguration mit RAID-1-Festplatten für die Protokollierung und RAID-5-Festplatten für Daten sowie mindestens 512 MB Arbeitsspeicher (RAM) empfohlen. Bei dieser Konfiguration sollte mindestens ein Pentium III-Prozessor mit 1,4 GHz verwendet werden. Bei reinen Datenbankservern kann auf den Einsatz von Systemen mit mehreren Prozessoren verzichtet werden.

<span id="BKMK_30"></span>
#### Wie wirkt sich die Verwendung des globalen Katalogs zur Gruppenerweiterung durch RMS auf die Arbeitsgeschwindigkeit des globalen Katalogservers aus?

Der RMS-Server führt eine Zwischenspeicherung von Gruppenerweiterungslisten durch, sodass keine große Belastung für den globalen Katalogserver entsteht. Häufige Aktualisierungen der Gruppenmitgliedschaft erhöhen die Abhängigkeit vom globalen Katalogserver, obwohl die Ausfallzeit während des Abrufs neuer Gruppenlisten über die Registrierung konfiguriert werden kann. Die häufige Erweiterung großer Gruppen wirkt sich nachteilig auf die Arbeitsgeschwindigkeit aus. Weitere Informationen dazu finden Sie im Abschnitt zum Ändern der Active Directory-Cacheeinstellungen in „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.

<span id="BKMK_31"></span>
#### Sind für RMS Schemaänderungen in Active Directory erforderlich?

Damit RMS die in der Veröffentlichungslizenz angegebene Gruppenmitgliedschaft erfolgreich über die Grenzen der Gesamtstruktur hinaus erweitern kann, muss in der lokalen Active Directory-Gesamtstruktur ein Kontaktobjekt vorhanden sein, das die Gruppe in der Remotegesamtstruktur darstellt. RMS kann die Attribute des Kontaktobjekts abfragen und herausfinden, dass dieses Objekt eine Gruppe in einer anderen Gesamtstruktur darstellt.

Damit RMS diese Abfrage ausführen kann, ist in Active Directory das Schemaattribut „msExchOriginatingForest“ für Exchange Server 2003 oder später erforderlich. Dieses Attribut wird standardmäßig im Active Directory-Schema installiert, wenn auf einem Server in der Gesamtstruktur Exchange Server 2003 ausgeführt wird. Das Attribut muss in der Gesamtstruktur jedes Active Directory-Schemas vorhanden sein, das an RMS teilnimmt. Wenn Sie Exchange Server 2003 nicht verwenden, können Sie das Schema mit dem RMS Administration Toolkit separat in der Active Directory-Struktur installieren.

<span id="BKMK_32"></span>
#### Wird der Dienstverbindungspunkt (Service Connection Point, SCP) zwischen den verschiedenen Domänencontrollern in der Domäne, in der der RMS-Server installiert ist, automatisch repliziert?

Nachdem der erste RMS-Server in einer Gesamtstruktur bereitgestellt wurde, muss er mithilfe eines Domänenkontos, das ausreichende Berechtigungen zum Erstellen eines Containerobjekts unter dem Container „Dienste“ im Konfigurationscontainer von Active Directory hat, in Active Directory registriert werden. Die vordefinierte Sicherheitsgruppe „Organisations-Admins“ ist ein Beispiel für ein Konto mit den erforderlichen Berechtigungen. Dadurch wird ein Dienstverbindungspunkt erstellt. Da dieser sich im Container „Dienste“ befindet, repliziert Active Directory diese Informationen auf alle Domänencontroller in der Gesamtstruktur.

<span id="BKMK_33"></span>
#### Wie kann der RMS-Client installiert und konfiguriert werden, wenn die Benutzer auf ihren Computern nicht über Administratorberechtigungen verfügen?

Der RMS-Client ist eine Windows-Installationsprogrammdatei und kann mithilfe einer Softwareverteilungsinfrastruktur, z. B. mit Systems Management Server (SMS) 2003, verteilt werden. Der RMS-Client kann außerdem mit einem Gruppenrichtlinienobjekt verteilt werden, das ein Dienstkonto mit Administratorberechtigungen verwendet. Wenn der RMS-Client unter Windows Vista ausgeführt wird, ist keine separate RMS-Clientinstallation mehr erforderlich, da diese in das Betriebssystem integriert ist.

<span id="BKMK_35"></span>
#### Inwieweit ist RMS skalierbar?

RMS ist ein zustandsloser Webdienst. Er kann wie andere Websites oder Webdienste in Clustern gruppiert werden, und seine Auslastung lässt sich durch Lastenausgleich regulieren. Die RMS-Leistung hängt hauptsächlich von der Prozessorverfügbarkeit ab und kann daher durch die Verwendung zusätzlicher Prozessoren verbessert werden.

<span id="BKMK_36"></span>
#### Unterstützt RMS Hardwaresicherheitsmodule (Hardware Security Modules, HSMs), um die RMS-Schlüssel in der Hardware zu sichern?

Ja, RMS kann mit CAPI-HSMs, wie z. B. dem nCipher-HSM, eingesetzt werden.
