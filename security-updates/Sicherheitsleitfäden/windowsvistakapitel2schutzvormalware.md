---
Title: Windows Vista – Kapitel 2 (Schutz vor Malware)
TOCTitle: Windows Vista – Kapitel 2 (Schutz vor Malware)
ms:assetid: c1356f48-abed-446b-8a54-9e9387eff56c
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443673(v=TechNet.10)
ms:contentKeyID: 20075616
---


# Windows Vista-Sicherheitshandbuch



### Kapitel 2: Schutz vor Malware
Veröffentlicht: 08. Nov 2006
 

Bei bösartiger Software, auch *Malware* genannt, handelt es sich um Programme oder Dateien, die schädlich für Computerbenutzer sind. Beispiele für Malware umfassen Computerviren, Würmer, Trojanerprogramme sowie Spyware, die ohne Erlaubnis Informationen über einen Computerbenutzer sammelt.

Windows Vista™ enthält mehrere neue Technologien, mit denen Sie den Schutz vor Malware bei Computern verbessern können, auf denen in Ihrer Umgebung Windows Vista ausgeführt wird. Sie können diese Funktionen und Dienste zusätzlich zu den Einstellungen in den Gruppenrichtlinienobjekten (GPOs) verwenden, die im vorherigen Kapitel beschrieben wurden und die teilweise ebenfalls vor Malware schützen.

In Windows Vista umfasst auch Microsoft® Internet Explorer® 7 einige Verbesserungen, die zum Schutz vor Malware beitragen. Technologien, die dazu beitragen, die Installation unerwünschter Software verhindern, sowie Technologien, die vor der nicht autorisierten Weitergabe persönlicher Daten schützen, sorgen für stark erhöhte Browsersicherheit und verbesserten Schutz vertraulicher Informationen.

Dieses Kapitel enthält einen Überblick über diese Technologien sowie Empfehlungen, wie sie bei Bedarf konfiguriert werden können. Sie können diese Empfehlungen in den entsprechenden Gruppenrichtlinienobjekten implementieren, die in Kapitel 1, „Implementieren der Sicherheitsbasis“, beschrieben werden. Sie müssen in diesem Zusammenhang jedoch berücksichtigen, dass bei vielen Einstellungen für diese Technologien spezifische Informationen über Ihre Umgebung erforderlich sind. Aus diesem Grund sind die meisten empfohlenen Werte für diese zusätzlichen Einstellungen nicht in den Gruppenrichtlinienobjekten enthalten, die im vorherigen Kapitel beschrieben wurden.

All diese Technologien sind standardmäßig so konfiguriert, dass sie erhöhten Schutz für Computer bieten, auf denen Windows Vista in der Unternehmensclient-Umgebung (EC-Umgebung) ausgeführt wird. Es gibt jedoch einige neue Einstellungen für Gruppenrichtlinien, die Sie verwenden können, um Verhalten und Funktionalität dieser Technologien anzupassen. Auf diese Weise können Sie einen noch besseren Schutz vor Malware in Ihrer Umgebung erreichen.

Dieses Kapitel ist in die folgenden neuen und verbesserten Sicherheitstechnologien in Windows Vista und Internet Explorer 7 unterteilt:
* Schutztechnologien in Windows Vista

* Schutztechnologien in Internet Explorer 7


**Hinweis**:   Für jedes dieser Gebiete im Kapitel werden spezifische Gruppenrichtlinieneinstellungen beschrieben, um die Standardkonfiguration bei einer Neuinstallation von Windows Vista zu dokumentieren. Spezifische Änderungen von Einstellungen oder Empfehlungen sind mit dem Symbol ‡ gekennzeichnet. Weitere Details zu diesen Einstellungswerten finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

Auf dieser Seite

[Schutztechnologien in Windows Vista](#ecaa)  
[Schutztechnologien in Internet Explorer 7](#ebaa)  
[Weitere Informationen](#eaaa)  



### Schutztechnologien in Windows Vista

Windows Vista enthält mehrere neue und verbesserte Technologien, die einen verbesserten Schutz vor Malware ermöglichen. Diese Technologien umfassen:
* Benutzerkontensteuerung (UAC)

* Windows Defender

* Windows-Firewall

* Windows-Sicherheitscenter

* Tool zum Entfernen bösartiger Software

* Richtlinien für Softwareeinschränkungen


Zusätzlich zu diesen Schutztechnologien muss berücksichtigt werden, dass die Anmeldung unter einem Standardbenutzerkonto weiterhin als äußerst empfehlenswerte Sicherheitsmaßnahme gilt. Selbst wenn die genannten Schutztechnologien aktiviert sind, müssen Sie besondere Schutzmaßnahmen für Benutzer mit Administratorzugriff vorsehen, da diese Benutzer anderenfalls Risiken ausgesetzt sind.


#### Benutzerkontensteuerung

Windows Vista beinhaltet Benutzerkontensteuerung (User Account Control, UAC), um eine Methode zum Trennen der Rechte und Aufgaben von Standardbenutzern und Administratoren bereitzustellen. Durch Benutzerkontensteuerung wird die Sicherheit erhöht, da die Benutzer bei Verwendung eines Standardbenutzerkontos besser als früher mit dem Computer interagieren können. Benutzer können jetzt mehr Aufgaben ausführen und eine höhere Anwendungskompatibilität nutzen, ohne sich mit Administratorrechten anmelden zu müssen. Dies trägt dazu bei, die Auswirkungen von Malware zu verringern sowie vor der Installation unautorisierter Software und vor nicht genehmigten Systemänderungen zu schützen.

**Hinweis**:   In früheren Versionen von Windows diente die Gruppe „Hauptbenutzer“ dazu, den Mitgliedern dieser Gruppe das Ausführen von Systemaufgaben, z. B. das Installieren von Anwendungen, zu ermöglichen, ohne dass dazu vollständige Administratorrechte erforderlich waren. In der Benutzerkontensteuerung die Gruppe „Hauptbenutzer“ nicht verwendet. Unter Windows Vista wurden die dieser Gruppe gewährten Rechte entfernt. Allerdings steht die Gruppe „Hauptbenutzer“ aus Gründen der Abwärtskompatibilität mit anderen Versionen des Betriebssystems weiterhin zur Verfügung. Um die Gruppe „Hauptbenutzer“ in Windows Vista nutzen zu können, müssen Sie eine neue Sicherheitsvorlage anwenden, um die Standardberechtigungen für Systemordner und die Registrierung zu ändern. Auf diese Weise können Sie den Mitgliedern der Gruppe „Hauptbenutzer“ Berechtigungen gewähren, die den Berechtigungen dieser Gruppe in Windows XP entsprechen.

In Windows Vista können Standardbenutzer jetzt viele Aufgaben ausführen, für die zuvor Administratorzugriff erforderlich war, die jedoch die Sicherheit nicht beeinträchtigten. So können Standardbenutzer jetzt beispielsweise Zeitzoneneinstellungen ändern, eine Verbindung mit einem sicheren drahtlosen Netzwerk herstellen sowie genehmigte Geräte und Microsoft ActiveX®-Steuerelemente installieren.

Außerdem trägt die Funktion „Administratorbestätigungsmodus“ in der UAC-Technologie ebenfalls dazu bei, Computer mit dem Betriebssystem Windows Vista vor bestimmten Arten von Malware zu schützen. Standardmäßig können Administratoren die meisten Programme und Aufgaben mit Standardbenutzerrechten ausführen. Wenn Benutzer Verwaltungsaufgaben wie das Installieren neuer Software oder Ändern bestimmter Systemeinstellungen vornehmen müssen, werden sie zuerst zur Bestätigung aufgefordert, bevor sie diese Aufgaben ausführen können. Allerdings stellt dieser Modus nicht dasselbe Maß an Schutz wie ein Standardbenutzerkonto bereit. Er kann auch nicht gewährleisten, dass bereits auf dem Clientcomputer vorhandene schädliche Software nicht die Software manipuliert, die erhöhte Rechte aufweist. Weiterhin ist nicht gewährleistet, dass die Software mit erhöhten Rechten nach der Zuweisung der erhöhten Rechte nicht selbst schädliche Aktionen ausführt.

Um von dieser Technologie zu profitieren, haben Sie jetzt die Möglichkeit, neue Gruppenrichtlinieneinstellungen in Windows Vista zu konfigurieren, mit denen das Verhalten der Benutzerkontensteuerung gesteuert wird. Die im vorherigen Kapitel beschriebenen Gruppenrichtlinieneinstellungen sind so konfiguriert, dass das vorgeschriebene Verhalten für die Benutzerkontensteuerung erzwungen wird. Allerdings empfiehlt Microsoft die Prüfung der Vorgaben für diese Einstellungen, die in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“, beschrieben werden. Dadurch soll sichergestellt werden, dass sie für die Anforderungen Ihrer Umgebung optimal konfiguriert sind.

Risikobewertung

Wenn sich Benutzer, die über Administratorrechte verfügen, anmelden, sind ihre Verwaltungsfunktionen aktiviert. Dies könnte zur Folge haben, dass Administratoraufgaben versehentlich oder mit böswilliger Absicht ausgeführt werden, ohne dass der jeweilige Benutzer dies bemerkt. Beispiel:
* Ein Benutzer lädt unbemerkt Malware von einer schädlichen oder infizierten Website herunter und installiert diese.

* Ein Benutzer wird dazu gebracht, eine E-Mail-Anlage zu öffnen, die Malware enthält. Diese Malware wird ausgeführt und installiert sich möglicherweise selbstständig auf dem Computer.

* Ein Wechseldatenträger wird in den Computer eingelegt, und die Autorun-Funktion versucht dann, die schädliche Software automatisch auszuführen.

* Ein Benutzer installiert nicht unterstützte Anwendungen, die die Leistungsfähigkeit oder Zuverlässigkeit des Computers beeinträchtigen können.


#### Risikominderung

Als Ansatz zur Risikominderung wird empfohlen, dass sich alle Benutzer zum Ausführen alltäglicher Aufgaben mit einem Standardbenutzerkonto anmelden. Benutzer sollten ihre Benutzerrechte nur dann auf die Ebene eines Administratorkontos anheben, wenn diese Zugriffsebene für bestimmte Aufgaben erforderlich ist. Stellen Sie außerdem sicher, dass UAC aktiviert ist, damit der Benutzer zur Bestätigung aufgefordert wird, wenn Aufgaben ausgeführt werden sollen, für die Administratorrechte erforderlich sind.

#### Erwägungen bei der Risikominderung

UAC kann dazu beitragen, die im vorherigen Abschnitt „Risikobewertung“ beschriebenen Risiken zu mindern. Sie müssen jedoch Folgendes berücksichtigen:
* Wenn Sie über betriebsinterne Anwendungsentwickler verfügen, empfiehlt Microsoft, dass diese den Artikel [Windows Vista Application Development Requirements for User Account Control Compatibility](http://www.microsoft.com/downloads/details.aspx?familyid=ba73b169-a648-49af-bc5e-a2eebb74c16b&amp;displaylang=en) (engl.) herunterladen und lesen. Dieses Dokument beschreibt, wie UAC-kompatible Anwendungen für Windows Vista entworfen und entwickelt werden.

* UAC kann Probleme für Anwendungen verursachen, die mit dieser Technologie nicht kompatibel sind. Aus diesem Grund ist es wichtig, Anwendungen vor deren Bereitstellung mit der Benutzerkontensteuerung zu testen. Weitere Informationen zum Testen der Anwendungskompatibilität finden Sie im [Desktop Deployment Center](http://www.microsoft.com/germany/technet/desktopdeployment/default.mspx) von TechNet.

* Da UAC in vielen Fällen eine Aufforderung zur Eingabe von Verwaltungsberechtigungen und zur Erhöhung von Benutzerrechten anzeigt, steigt die Anzahl der Schritte beim Ausführen vieler häufiger Verwaltungsaufgaben. Sie sollten die Auswirkungen dieser zusätzlichen Schritte gemeinsam mit den Mitarbeitern beurteilen, die administrative Aufgaben ausführen. Wenn die zusätzlichen UAC-Aufforderungen diese Benutzer stark beeinträchtigen, können Sie die UAC-Richtlinieneinstellung „Verhalten der Benutzeraufforderung mit erhöhten Rechten für Administratoren im Administratorbestätigungsmodus“ in „Erhöhte Rechte ohne Eingabeanforderung“ ändern. Wenn Sie diese Richtlinie ändern, steigen jedoch möglicherweise die Sicherheitsrisiken in Ihrer Umgebung, was wiederum vom Windows-Sicherheitscenter gemeldet wird.

* Ein Benutzer, der über Administratorrechte verfügt, kann den Administratorbestätigungsmodus deaktivieren und UAC so konfigurieren, dass beim Installieren von Anwendungen keine Anmeldeinformationen angefragt werden. Zudem kann dieser Benutzer das Verhalten der Benutzeraufforderung zur Erhöhung von Rechten ändern. Aus diesem Grund muss die Anzahl der Benutzer in Ihrem Unternehmen kontrolliert werden, die über Administratorzugriff auf die Computer verfügen.

* Microsoft empfiehlt, zwei Konten für Mitarbeiter zuzuweisen, die Administrationsaufgaben ausführen. Für alltägliche Aufgaben sollten die Mitarbeiter ein Konto auf Standardbenutzerebene verwenden. Wenn spezielle Verwaltungsaufgaben erforderlich sind, sollten sich die Mitarbeiter mit dem Konto auf Administratorebene anmelden, die Aufgaben ausführen und sich dann abmelden und wieder mit dem Standardbenutzerkonto arbeiten.

* Mit den Gruppenrichtlinieneinstellungen für dieses Handbuch wird die Fähigkeit eines Standardbenutzers deaktiviert, seine Berechtigungen zu erhöhen. Dies ist der empfohlene Ansatz, da auf diese Weise sichergestellt wird, dass Verwaltungsaufgaben nur von den Konten ausgeführt werden können, die hierfür auf Administratorebene speziell eingerichtet wurden.

* Wenn eine Anwendung fälschlicherweise als Administrator- oder Benutzeranwendung identifiziert wird (beispielsweise mit einem „Administrator“- oder „Standard“-Token), könnte die Anwendung von Windows Vista im falschen Sicherheitskontext gestartet werden.


#### Verfahren zur Risikominderung

Starten Sie das Verfahren zur Risikominderung, indem Sie die vollständigen Möglichkeiten von UAC untersuchen. Weitere Informationen finden Sie unter [*Windows Vista - User Account Control Schritt für Schritt*](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/library/0d75f774-8514-4c9e-ac08-4c21f5c6c2d9.mspx) und im Dokument [Getting Started with User Account Control on Windows Vista](http://technet.microsoft.com/en-us/windowsvista/aa906022.aspx) (engl.).

**So verwenden Sie dieses Verfahren zur Risikominderung**
1. Ermitteln Sie die Anzahl der Benutzer, die in der Lage sind, Verwaltungsaufgaben auszuführen.

2. Ermitteln Sie, wie oft Verwaltungsaufgaben erforderlich sind.

3. Bestimmen Sie, ob Administratoren in der Lage sein sollten, Verwaltungsaufgaben durch einfache Zustimmung an der UAC-Bestätigungsaufforderung auszuführen, oder ob sie spezielle Anmeldeinformationen zum Ausführen von Verwaltungsaufgaben eingeben müssen.

4. Bestimmen Sie, ob Standardbenutzer die Fähigkeit zum Erhöhen von Rechten besitzen sollten, um Verwaltungsaufgaben ausführen zu können. Die Richtlinieneinstellungen, die als Bestandteil dieses Handbuchs angewendet werden, blockieren speziell die Fähigkeit von Standardbenutzern, ihre Rechte zu erhöhen.

5. Ermitteln Sie, wie bei der Installation von Anwendungen verfahren werden soll.

6. Passen Sie die UAC-Gruppenrichtlinieneinstellungen an Ihre Anforderungen an.

Verwenden von Gruppenrichtlinien zum Verringern des Risikos für UAC

Die UAC-Einstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Lokale Richtlinien\Sicherheitsoptionen**

Die folgende Tabelle enthält spezifische Informationen zu den Sicherheitseinstellungen für diese Technologie in Windows Vista.

**Tabelle 2.1 UAC-Kontrolleinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Administratorbestätigungsmodus für das integrierte Administratorkonto

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung bestimmt das Verhalten des Administratorbestätigungsmodus für das vordefinierte Administratorkonto.

</td>

<td style="border:1px solid black;">


Deaktiviert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Verhalten der Benutzeraufforderung mit erhöhten Rechten für Administratoren im Administratorbestätigungsmodus

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung bestimmt das Verhalten der Benutzeraufforderung zur Erhöhung von Rechten für Administratoren.

</td>

<td style="border:1px solid black;">


Aufforderung zur Eingabe der Zustimmung ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Verhalten der Anhebungsaufforderung für Standardbenutzer

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung bestimmt das Verhalten der Anhebungsanforderung für Standardbenutzer.

</td>

<td style="border:1px solid black;">


Aufforderung zur Eingabe der Anmeldeinformationen ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anwendungsinstallationen erkennen und erhöhte Rechte anfordern

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung bestimmt das Verhalten der Erkennung von Anwendungsinstallationen für das gesamte System.

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Nur ausführbare Dateien heraufstufen, die signiert und validiert sind

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung erzwingt PKI-Signaturüberprüfungen für jede interaktive Anwendung, welche die Erhöhung der Rechte anfordert. Unternehmensadministratoren können die Liste mit Anwendungen, die durch den Administrator genehmigt werden müssen, mit Zertifikaten im Speicher mit vertrauenswürdigen Herausgebern des lokalen Computers kontrollieren.

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Nur erhöhte Rechte für UIAccess-Anwendungen, die an sicheren Orten installiert sind

</td>

<td style="border:1px solid black;">


Mit dieser Sicherheitseinstellung wird festgelegt, dass sich Anwendungen an einem sicheren Speicherort im Dateisystem befinden müssen, wenn sie die Ausführung mit einer UIAccess-Integritätsebene anfordern.

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Alle Administratoren im Administratorbestätigungsmodus ausführen

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung bestimmt das Verhalten aller UAC-Richtlinien für das gesamte System.

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Bei Benutzeraufforderung nach erhöhten Rechten zum sicheren Desktop wechseln

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung bestimmt, ob die Erhöhungsanforderung eine Benutzeraufforderung auf dem interaktiven Benutzerdesktop oder dem sicheren Desktop anzeigt.

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Datei- und Registrierungsschreibfehler an Einzelbenutzerstandorte virtualisieren

</td>

<td style="border:1px solid black;">


Diese Sicherheitseinstellung ermöglicht die Umleitung von Schreibfehlern älterer Anwendungen an definierte Orte in der Registrierung und dem Dateisystem.

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

Die Benutzeroberfläche für die UAC-Anmeldeinformationen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\Benutzerschnittstellen für Anmeldeinformationen**

Die folgende Tabelle enthält spezifische Informationen zu den Sicherheitseinstellungen für diese Technologie in Windows Vista.

**Tabelle 2.2 Einstellungen für die Benutzeroberfläche für die UAC-Anmeldeinformationen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Enumerate administrator accounts on elevation (Administratorkonten bei Heraufstufung auflisten)

</td>

<td style="border:1px solid black;">


Standardmäßig werden alle Administratorkonten angezeigt, wenn ein Benutzer versucht, die Rechte einer laufenden Anwendung zu erhöhen. Wenn Sie diese Einstellung aktivieren, müssen die Benutzer immer einen Benutzernamen und ein Kennwort eingeben, um ihre Rechte zu erhöhen.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Require trusted path for credential entry (Vertrauenswürdigen Pfad für die Eingabe von Anmeldeinformationen erfordern)

</td>

<td style="border:1px solid black;">


Wenn Sie diese Einstellung aktivieren, fordert Windows Vista den Benutzer auf, Anmeldeinformationen mithilfe eines vertrauenswürdigen Pfades einzugeben. Auf diese Weise wird verhindert, dass ein trojanisches Pferd oder andere Arten von schädlichem Code die Windows-Anmeldeinformationen des Benutzers stehlen. Diese Richtlinie betrifft nur Authentifizierungsaufgaben ohne Anmeldung. Als Best Practice für die Sicherheit sollte diese Richtlinie aktiviert werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

Die Einstellungen für den ActiveX-Installationsdienst können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\ActiveX-Installationsdienst**

Die folgende Tabelle stellt spezifische Informationen zu den Sicherheitseinstellungen für den ActiveX-Installationsdienst in Windows Vista zur Verfügung.

**Tabelle 2.3 ActiveX-Installationsdienst**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Approved Installation Sites for ActiveX Controls (Zulässige Installationssites für ActiveX-Steuerelemente)

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht es einem Administrator, einem Standardbenutzerkonto das Recht zum Installieren von ActiveX-Steuerelementen aus einer Liste mit genehmigten ActiveX-Installationssites zu gewähren.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für diese Einstellung. Weitere Informationen zu dieser Einstellung finden Sie auf der Registerkarte **Erklärung** der Einstellung im Gruppenrichtlinienobjekt-Editor.


#### Windows Defender

Bei Windows Defender handelt es sich um ein Programm, das in Windows Vista enthalten ist und zudem als Download für Windows XP zur Verfügung steht. Das Programm trägt dazu bei, Computer vor Popupfenstern, Leistungseinbußen und Sicherheitsbedrohungen durch Spyware und andere unerwünschte Software zu schützen. Windows Defender überwacht in Echtzeit wichtige Prüfpunkte des Betriebssystems Windows Vista. Dabei handelt es sich um Bereiche, die bevorzugte Ziele unerwünschter Software sind, beispielsweise der Startordner oder die Autorun-Einträge in der Registrierung.

Windows Defender trägt auch dazu bei, unerwünschte Anwendungen wie Adware, Keylogger und Spyware zu erkennen und zu entfernen. Wenn ein Programm versucht, einen geschützten Bereich in Windows Vista zu ändern, wird der Benutzer von Windows Defender aufgefordert, die Änderung entweder zu genehmigen oder sie abzulehnen, um die Installation von Spyware zu verhindern. Durch diese Überwachung wird die Zuverlässigkeit von Computern erhöht, auf denen Windows Vista ausgeführt wird. Gleichzeitig wird dadurch der Datenschutz für die Benutzer verbessert. Windows Defender ist in Windows Vista standardmäßig aktiviert. Obwohl Ihnen diese Technologie bereits einen erhöhten Schutz vor Spyware zur Verfügung stellt, können Sie das Programm auch in Verbindung mit Schutzprodukten von Drittanbietern verwenden. Um den bestmöglichen Schutz vor schädlicher Software zu gewährleisten, empfiehlt Microsoft dringend, dass die Kunden auch eine vollständige Antivirenlösung in Verbindung mit Windows Defender bereitstellen.

Sie können neue Gruppenrichtlinieneinstellungen in Windows Vista konfigurieren, um das Verhalten von Windows Defender zu steuern. Die im vorherigen Kapitel beschriebenen Gruppenrichtlinieneinstellungen enthalten keine Einstellungen, mit denen das Standardverhalten von Windows Defender geändert wird, da die Werte für diese Einstellungen vermutlich jeweils von den Anforderungen Ihrer Umgebung abhängen.

Microsoft SpyNet-Community

Bei Microsoft SpyNet handelt es sich um eine Onlinecommunity, die Computerbenutzer beim richtigen Reagieren auf potenzielle Bedrohungen durch Spyware unterstützen soll. Die Community trägt auch dazu bei, die Ausbreitung von Infektionen durch Spyware einzudämmen.

Wenn Windows Defender Software oder durch Software vorgenommene Änderungen entdeckt, für die noch keine Risikoeinstufung vorgenommen wurde, können Sie sehen, wie andere Mitglieder auf die Warnung reagieren. Umgekehrt unterstützen die von Ihnen ergriffenen Maßnahmen andere Mitglieder der Community dabei, sich für eine angemessene Reaktion auf Bedrohungen zu entscheiden. Darüber hinaus helfen Ihre Maßnahmen Microsoft bei der Entscheidung, welche Software auf potenzielle Bedrohungen untersucht werden soll. Sie können entweder grundlegende oder zusätzliche Informationen über festgestellte Software senden. Zusätzliche Informationen tragen dazu bei, die Funktionsweise von Windows Defender zu verbessern. Beispielsweise kann die hierzu verwendete Technologie den Speicherort von erkannten Elementen auf Ihrem Computer erfassen, wenn gefährliche Software entfernt wurde. In diesen Fällen sammelt und sendet Windows Defender diese Informationen automatisch an die Community.

Risikobewertung

Spyware verursacht eine Reihe ernsthafter Risiken für Unternehmen, die gemindert werden müssen, um sicherzustellen, dass Daten und Computer nicht gefährdet werden. Die am häufigsten festzustellenden Risiken, die Spyware für ein Unternehmen darstellt, umfassen unter anderem:
* Vertrauliche Unternehmensdaten, die von nicht autorisierten Benutzern angezeigt werden könnten

* Persönlichen Informationen, die von nicht autorisierten Benutzern angezeigt werden könnten

* Computer, deren Sicherheit durch einen nicht autorisierten Angreifer verletzt wird

* Produktivitätsausfälle, da Spyware die Leistung und Stabilität von Computern beeinträchtigt

* Steigende Supportkosten aufgrund von Spywareinfektionen

* Ein gewisses Erpressungspotenzial für Ihr Unternehmen, wenn eine Infektion vertrauliche Daten offen legt


Risikominderung

Windows Defender ist zur Reduzierung der durch Spyware verursachten Risiken konzipiert. Regelmäßige Updates für die Technologie werden automatisch über Windows Update bereitgestellt. Sie haben auch die Möglichkeit, stattdessen die Microsoft Windows Server Update Services (WSUS) zu verwenden.

Zusätzlich zum Spywareschutz durch Windows Defender empfiehlt Microsoft dringend, eine Antivirenlösung zu installieren, die den Spywareschutz auf die Erkennung von Viren, trojanischen Pferden und Würmern erweitert. Beispielsweise stellen Produkte wie Microsoft Forefront Client Security konsolidierten Malwareschutz für Desktops, Laptops und Serverbetriebssysteme in Unternehmen zur Verfügung.

Erwägungen bei der Risikominderung

Windows Defender ist in Windows Vista standardmäßig aktiviert. Bei der Entwicklung dieser Technologie wurde großer Wert darauf gelegt, dass die Benutzer unter normalen Betriebsbedingungen davon möglichst wenig bemerken. Allerdings sollten die folgenden Empfehlungen beim Bereitstellen von Windows Vista berücksichtigt werden:
* Testen Sie die Interoperabilität von Echtzeitscannern für Spyware oder Viren von Drittanbietern, die Sie möglicherweise in Ihrem Unternehmen verwenden möchten.

* Entwerfen Sie ein System zur Verwaltung der Updates für die Signaturdefinitionen, wenn in Ihrem Unternehmen eine große Zahl von Computern verwaltet wird.

* Informieren Sie Benutzer über die häufigsten Tricks, mit denen Spywareprogramme Benutzer zum Ausführen eines schädlichen Programms zu bewegen versuchen.

* Passen Sie den geplanten Zeitpunkt für die Prüfung an die Anforderungen Ihres Unternehmens an. Als Standardeinstellung ist eine tägliche Prüfung um 2:00 Uhr nachts vorgesehen. Wenn der Computer nicht in der Lage ist, die Prüfung zu diesem Zeitpunkt auszuführen, wird der Benutzer zu einem späteren Zeitpunkt benachrichtigt und aufgefordert, eine Prüfung durchzuführen. Wenn die Prüfung nicht innerhalb der nächsten zwei Tage erfolgt, wird sie ungefähr 10 Minuten nach dem nächsten Start des Computers ausgeführt. Diese Prüfung erfolgt als Prozess mit niedriger Priorität, so dass die Auswirkungen auf den Client so gering wie möglich bleiben. Durch die Leistungsverbesserungen bei der E/A-Verarbeitung in Windows Vista hat diese Prüfung mit niedriger Priorität wesentlich geringere Auswirkungen auf den Benutzer als unter Windows XP.

* Windows Defender ist nicht als Antispywarelösung für die Verwendung auf Unternehmensebene gedacht. Das Programm stellt weder zentrale Mechanismen zur Berichterstellung noch zur Überwachung oder Steuerung zur Verfügung, wie sie bei Geschäftsanwendungen üblich sind. Wenn zusätzliche Berichterstellung oder Steuerung erforderlich sind, müssen Sie den Einsatz zusätzlicher Produkte wie Microsoft Forefront Client Security in Betracht ziehen.

* Legen Sie fest, wie in Ihrem Unternehmen Berichte über mögliche Spyware an die Onlinecommunity Microsoft SpyNet weitergeleitet werden.


Verfahren zur Risikominderung

Da Windows Defender standardmäßig Bestandteil des Betriebssystems ist, sind keine zusätzlichen Schritte zum Aktivieren von Windows Defender erforderlich. Allerdings empfiehlt Microsoft einige zusätzliche Schritte, damit der dauerhafte Schutz Ihres Unternehmens sichergestellt wird.

**So verwenden Sie dieses Verfahren zur Risikominderung**
1. Machen Sie sich mit der Funktionalität zum Schutz vor Spyware von Windows Vista und Windows Defender vertraut.

2. Beschäftigen Sie sich mit den Gruppenrichtlinieneinstellungen für Windows Defender.

3. Erwägen Sie zusätzlichen Virenschutz für Ihr Unternehmen.

4. Planen Sie das optimale Updateverfahren für die Computer im Unternehmen. Es ist möglich, dass mobile Computer eine andere Updatekonfiguration als Desktopcomputer benötigen.

5. Schulen Sie die Benutzer, damit diese verdächtige Computeraktivitäten identifizieren können.

6. Schulen Sie Supportmitarbeiter in der Verwendung der Tools von Windows Defender, damit diese erfolgreich auf Supportanfragen reagieren können.

Verwenden einer Gruppenrichtlinie zur Risikominderung für Windows Defender

Sie können die verfügbaren Einstellungen für Windows Defender in folgendem Verzeichnis im Gruppenrichtlinienobjekt-Editor überprüfen und konfigurieren:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\Windows Defender**

**Tabelle 2.4 Windows Defender-Kontrolleinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Turn on definition updates through both WSUS und Windows Update (Definitionsupdates über WSUS und Windows Update aktivieren)

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht es Ihnen, Windows Defender zum Überprüfen und Installieren von Definitionsupdates von Windows Update zu konfigurieren, wenn ein lokal verwalteter Server für Windows Server Update Services (WSUS) nicht verfügbar ist.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Check for New Signatures Before Scheduled Scans (Vor geplanten Prüfungen auf neue Signaturen überprüfen)

</td>

<td style="border:1px solid black;">


Wenn Sie diese Einstellung aktivieren, wird bei der geplanten Prüfung auf neue Signaturen geprüft, bevor die eigentliche Prüfung beginnt. Wenn diese Einstellung auf **Deaktiviert** oder **Nicht konfiguriert** eingestellt ist, beginnen die geplanten Prüfungen, ohne dass zuvor neue Signaturen heruntergeladen werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Turn off Windows Defender (Windows Defender deaktivieren)

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Einstellung den Standardwert beibehalten, wird der Echtzeitschutz von Windows Defender aktiviert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Turn off Real-Time Protection Prompts for Unknown Detection (Aufforderungen zum Echtzeitschutz bei Erkennung unbekannter Aktivitäten deaktivieren)

</td>

<td style="border:1px solid black;">


Diese Einstellung bestimmt, ob Benutzer von Windows Defender gefragt werden, ob unbekannte Aktivitäten zugelassen oder blockiert werden sollen.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Enable Logging Known Good Detection (Protokollierung bei Erkennung nicht schädlicher Aktivitäten aktivieren)

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht das Protokollieren von Erkennungsdaten während des Echtzeitschutzes, wenn Windows Defender Dateien erkennt, die als nicht schädlich bekannt sind. Das Protokollieren erkannter Aktivitäten stellt Ihnen detaillierte Informationen zu den Programmen zur Verfügung, die auf den von Ihnen überwachten Computern ausgeführt werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Enable Logging Unknown Detection (Protokollierung bei Erkennung unbekannter Aktivitäten aktivieren)

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht das Protokollieren von erkannten Aktivitäten während des Echtzeitschutzes, wenn Windows Defender unbekannte Dateien erkennt. Das Protokollieren erkannter Aktivitäten stellt Ihnen detaillierte Informationen zu den Programmen zur Verfügung, die auf den von Ihnen überwachten Computern ausgeführt werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Download Entire Signature Set (Vollständigen Signatursatz herunterladen)

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht das Herunterladen des vollständigen Signatursatzes, anstatt nur die Signaturen herunterzuladen, die seit dem letzten Signaturdownload aktualisiert wurden. Wenn der vollständige Signatursatz heruntergeladen wird, können Probleme mit Signaturinstallationen leichter behoben werden. Da diese Datei groß ist, kann das Herunterladen jedoch länger dauern.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Configure Microsoft SpyNet Reporting (Berichterstellung für Microsoft SpyNet konfigurieren)

</td>

<td style="border:1px solid black;">


Diese Einstellung legt die Einstellungen für die Mitgliedschaft in der Onlinecommunity Microsoft SpyNet fest.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.


#### Windows-Firewall

Eine persönliche Firewall ist eine wesentlicher Bestandteil des Schutzes vor vielen Arten von Malware. Wie die Firewallfunktionalität in Windows XP Service Pack 2 (SP2) ist auch die Firewall in Windows Vista standardmäßig aktiviert, um den Computer des Benutzers zu schützen, sobald das Betriebssystem gestartet wurde.

Die Windows-Firewall in Windows Vista umfasst sowohl die Filterung eingehender als auch ausgehender Daten, um Benutzer durch das Beschränken von Betriebssystemressourcen zu schützen, die sich unerwartet verhalten. Die Firewall ist zudem in die Funktionen zur Netzwerkerkennung von Windows Vista integriert, so dass je nach Standort des Clientcomputers spezifische Regeln angewendet werden können. Wenn sich ein Laptopcomputer beispielsweise in einem Unternehmensnetzwerk befindet, können vom Administrator der Domänennetzwerkumgebung Firewallregeln definiert werden, die den Sicherheitsanforderungen dieses Netzwerks entsprechen. Wenn jedoch ein Benutzer versucht, mit demselben Laptop eine Internetverbindung über ein öffentliches Netzwerk herzustellen (beispielsweise über einen öffentlichen Hotspot), kann automatisch ein anderer Satz von Firewallregeln angewendet werden, um sicherzustellen, dass der Computer vor Angriffen geschützt ist.

Außerdem enthält Windows Vista als erstes Windows-Betriebssystem eine Firewallverwaltung mit IPsec (Internet Protocol Security). In Windows Vista sind in einer einzigen Konsole mit der Bezeichnung „Windows-Firewall mit erweiterter Sicherheit“ sowohl IPsec als auch die Firewallverwaltung integriert. In der Konsole werden die Filterung ein- und ausgehenden Datenverkehrs sowie Einstellungen für die IPsec-Server- und Domänenisolation in der Benutzeroberfläche zentralisiert, um so die Konfiguration zu vereinfachen und Richtlinienkonflikte zu verringern.

Risikobewertung

Eine Netzwerkverbindung ist in der modernen Geschäftswelt unverzichtbar. Allerdings ist diese Verbindung auch zu einem Hauptziel für Angreifer geworden. Die Bedrohungen, die auf Konnektivität zurückzuführen sind, müssen reduziert werden, um Sicherheitsverletzungen bei Daten oder Computern zu verhindern. Zu den häufigsten Bedrohungen für Unternehmen durch netzwerkbasierte Angriffe zählen u. a.:
* Ein Computer, dessen Sicherheit durch einen nicht autorisierten Angreifer verletzt wird, der dann Administratorzugriff auf diesen Computer erlangen könnte.

* Netzwerkscannerprogramme, mit denen ein Angreifer von einem Remotestandort aus offene Netzwerkports ermitteln kann, um einen Angriff zu starten.

* Vertrauliche Unternehmensdaten, die nicht autorisierten Benutzern zugänglich gemacht werden könnten, wenn es einem Trojanerprogramm gelingt, eine nicht autorisierte Netzwerkverbindung von einem Clientcomputer zu einem Angreifer zu öffnen.

* Mobile Computer, die Netzwerkangriffen ausgesetzt werden könnten, während sie sich außerhalb der Netzwerkfirewall des Unternehmens befinden.

* Computer in einem internen Netzwerk, die einem Netzwerkangriff durch einen manipulierten Computer ausgesetzt werden könnten, der direkt mit dem internen Netzwerk verbunden ist.

* Ein potenzielles Erpressungsrisiko für Ihr Unternehmen, wenn ein Angreifer erfolgreich die Sicherheit interner Computer verletzt.


Risikominderung

Die Firewall in Windows Vista schützt den Clientcomputer von Anfang an. Die Firewall blockiert den meisten unerwünschten eingehenden Datenverkehr, bis entweder durch einen Administrator oder eine Gruppenrichtlinie eine Änderung vorgenommen wird.

Die Windows-Firewall umfasst auch die Filterung ausgehenden Netzwerkverkehrs, wobei die Voreinstellung vorsieht, dass der gesamte ausgehende Netzwerkverkehr zulässig ist. Sie können Gruppenrichtlinieneinstellungen verwenden, um diese Regeln in der Firewall von Windows Vista zu konfigurieren. Dadurch wird sichergestellt, dass die Sicherheitseinstellungen auf dem Client konstant bleiben.

Erwägungen bei der Risikominderung

Es gibt einige Punkte, die Sie berücksichtigen sollten, wenn Sie die Firewall in Windows Vista verwenden möchten:
* Testen Sie die Interoperabilität von Anwendungen, die auf den Computern Ihres Unternehmens erforderlich sind. Für jede Anwendung sollten die Anforderungen an die Netzwerkports erfasst sein, um zu gewährleisten, dass nur die erforderlichen Ports durch die Windows-Firewall geöffnet werden.

* Die Firewall von Windows XP unterstützt ein Domänen- und ein Standardprofil. Das Domänenprofil ist aktiv, wenn der Client mit einem Netzwerk verbunden ist, das die Domänencontroller für die Domäne enthält, in der sich das zugehörige Computerkonto befindet. Auf diese Weise können Sie Regeln erstellen, die für die Anforderungen des internen Netzwerks des Unternehmens spezifisch sind. Die Windows Vista-Firewall enthält ein privates und ein öffentliches Profil, um die Schutzeinstellungen für Clientcomputer feiner abzustufen, wenn sich ein Benutzer außerhalb des Unternehmensnetzwerks und der zugehörigen Schutzmaßnahmen aufhält.

* Untersuchen Sie die Protokollierungsfunktionen der Windows-Firewall, um zu bestimmen, ob sie in Ihre vorhandenen Unternehmenslösungen für Berichterstellung oder Überwachung integriert werden kann.

* Standardmäßig blockiert die Windows-Firewall die Remotesteuerung oder Remoteverwaltung von Windows Vista-basierten Computern. Microsoft hat eine Reihe von Regeln speziell für solche Remoteaufgaben in der Windows-Firewall erstellt. Wenn Sie möchten, dass Ihre Unternehmenscomputer diese Remoteaufgaben unterstützen, müssen Sie die erforderlichen Regeln für jedes Profil aktivieren, für das die Aufgabe erforderlich ist. Sie können beispielsweise die Remotedesktop-Regel für das Domänenprofil aktivieren, damit Ihr Helpdesk Benutzer im Unternehmensnetzwerk unterstützt, jedoch diese Regel für die öffentlichen und privaten Profile deaktiviert lassen. Dadurch wird die Angriffsfläche Ihrer Computer verkleinert, wenn sie sich außerhalb Ihres Netzwerks befinden.


Risikominderung mithilfe der Windows-Firewall mit erweiterter Sicherheit

Windows Vista enthält neue Gruppenrichtlinieneinstellungen und eine Verwaltungsoberfläche, die Sie beim Konfigurieren der neuen Funktionalität in der Firewall von Windows Vista unterstützen. Die erweiterten Sicherheitseinstellungen für Windows Vista können nicht auf einen Clientcomputer angewendet werden, auf dem Windows XP ausgeführt wird.

Microsoft empfiehlt, dass Sie diese neuen Möglichkeiten eingehend untersuchen, um zu bestimmen, inwiefern sie Ihnen beim besseren Schützen Ihrer Umgebung nützlich sein können. Wenn Sie beabsichtigen, das Standardverhalten der Windows Vista-Firewall zu ändern, empfiehlt Microsoft die Verwendung der Gruppenrichtlinieneinstellungen für „Windows-Firewall mit erweiterter Sicherheit“, um Clientcomputer unter Windows Vista zu verwalten.

Sie können die neuen Gruppenrichtlinieneinstellungen und das Snap-In zur Verwaltung für die Windows-Firewall in folgendem Verzeichnis im Gruppenrichtlinienobjekt-Editor überprüfen und konfigurieren:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Windows-Firewall mit erweiterter Sicherheit**

Die Windows-Firewall mit erweiterter Sicherheit unterstützt die folgenden Umgebungsprofile:
* **Domänenprofil.**   Dieses Profil wird angewendet, wenn ein Computer mit einem Netzwerk verbunden ist und die Authentifizierung mit einem Domänencontroller in der Domäne vornimmt, der der Computer angehört.

* **Öffentliches Profil.**   Dieses Profil ist der Standardtyp für die Netzwerkadresse, wenn der Computer nicht mit einer Domäne verbunden ist. Die öffentlichen Profileinstellungen sollten am restriktivsten sein, da der Computer mit einem öffentlichen Netzwerk verbunden ist, in dem die Sicherheit nicht so streng kontrolliert werden kann wie innerhalb einer IT-Umgebung.

* **Privates Profil.**   Dieses Profil gilt nur, wenn ein Benutzer mit lokalen Administratorrechten das Profil einem Netzwerk zuweist, das zuvor als öffentliches Netzwerk konfiguriert war. Microsoft empfiehlt, dies nur für ein vertrauenswürdiges Netzwerk vorzunehmen.


Es muss berücksichtigt werden, dass jeweils nur ein Profil aktiv ist. Wenn der Computer mehrere Schnittstellen aufweist und diese mit mehreren Netzwerkadressen verbunden sind, müssen folgende Punkte bei der Auswahl des anzuwendenden Profils herangezogen werden:
1. Wenn alle Netzwerkschnittstellen mit einer Netzwerkadresse in einer Domäne verbunden sind, wählen Sie das Domänenprofil aus.

2. Wenn alle Netzwerkschnittstellen mit einer privaten Netzwerkadresse verbunden sind, wählen Sie das private Profil aus.

3. Wenn eine Netzwerkschnittstelle mit einer öffentlichen Netzwerkadresse verbunden ist, wählen Sie das öffentliche Profil aus.


Microsoft empfiehlt, die Windows-Firewall mit erweiterter Sicherheit für alle drei Profile zu aktivieren. Zusätzlich zu den erweiterten Firewallregeln unterstützt die Windows-Firewall auch Regeln für die Verbindungssicherheit. Die Verbindungssicherheit umfasst das Authentifizieren von zwei Computern, bevor diese mit der Kommunikation beginnen, sowie das Absichern der Informationen, die zwischen den beiden Computern ausgetauscht werden. Die Windows-Firewall mit erweiterter Sicherheit enthält IPsec-Technologie, um Schlüsselaustausch, Authentifizierung, Datenintegrität und optional die Datenverschlüsselung zu unterstützen.

Weitere Informationen finden Sie auf der TechNet Webseite zu [IPsec](http://www.microsoft.com/technet/network/ipsec/default.mspx) (engl.).

In Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“, werden alle empfohlenen Einstellungen für die Windows-Firewall mit erweiterter Sicherheit beschrieben, und es wird angegeben, für welche Einstellungen umgebungsspezifische Informationen erforderlich sind.


#### Windows-Sicherheitscenter

Das Windows-Sicherheitscenter (WSC) wird als Hintergrundprozess auf Computern ausgeführt, die das Betriebssystem Windows Vista oder Windows XP SP2 verwenden. In Windows Vista wird von dieser Funktion ständig der Status von vier wichtigen Sicherheitskategorien überprüft und angezeigt:
* Firewall

* Automatische Updates

* Schutz vor schädlicher Software

* Weitere Sicherheitseinstellungen


Der WSC-Prozess dient auch als Ausgangspunkt für den Zugriff auf andere sicherheitsbezogene Bereiche des Computers. Zudem können Sie über das Windows-Sicherheitscenter Support und Ressourcen zu Sicherheitsthemen erhalten. Beispielsweise stellt das WSC einen Link zur Verfügung, um Benutzern ohne Antivirensoftware Hilfestellung zu bieten. Bei Klicken auf den Link werden Antivirenlösungen angezeigt, die mit dem Windows-Sicherheitscenter kompatibel sind.

Microsoft hat das WSC in Windows Vista verbessert und hierzu eine neue Kategorie mit der Bezeichnung „Weitere Sicherheitseinstellungen“ eingeführt. Diese Kategorie zeigt den Status der Sicherheitseinstellungen in Internet Explorer und der Benutzerkontensteuerung an. Eine weitere neue Kategorie in Windows Vista ist „Schutz vor schädlicher Software“, in der Überwachungsfunktionen für Antiviren- und Antispywareprogramme bereitgestellt werden. Zusätzlich zu dem von Windows Vista bereitgestellten Standardschutz kann das WSC Sicherheitslösungen verschiedener Anbieter für die Windows-Firewall sowie Antiviren- und Antispywaresoftware überwachen, die auf demselben Clientcomputer ausgeführt werden. Darüber hinaus gibt das Windows-Sicherheitscenter an, welche Lösungen aktiviert und auf dem neuesten Stand sind.

Für Clientcomputer unter Windows Vista stellt das WSC direkte Links zu Anbietern zur Verfügung, die Sie zur Behebung eventuell auf dem Computer auftretender Probleme einsetzen können. Wenn beispielsweise eine Antiviren- oder Antispywarelösung eines Drittanbieters deaktiviert oder veraltet ist, stellt Ihnen das WSC eine Schaltfläche zur Verfügung, mit der Sie eine Lösung des jeweiligen Anbieters auf dem Computer starten und dadurch das Problem beheben können. Außerdem bietet das WSC Links zur Website des Anbieters, damit der Benutzer ein Abonnement aktivieren oder verlängern bzw. Updates beziehen kann. Für den optimalen Schutz vor schädlichen Programmen ist es wichtig, die Sicherheitssoftware zu aktivieren und auf dem neuesten Stand zu halten. Wenn diese Anforderungen nicht erfüllt sind, kann Ihr Computer schnell durch Malware gefährdet werden.

Das Windows-Sicherheitscenter wird auf Computern mit Windows Vista standardmäßig ausgeführt. Die im vorherigen Kapitel beschriebenen Gruppenrichtlinieneinstellungen enthalten keine Einstellungen, die das Standardverhalten des WSC ändern. Administratoren haben jedoch die Möglichkeit, mithilfe einer Gruppenrichtlinie sicherzustellen, dass die Clientbenutzeroberfläche des WSC auf den Computern in der Domäne entweder deaktiviert oder aktiviert bleibt. Sie können die für das WSC verfügbare Gruppenrichtlinieneinstellung in folgendem Verzeichnis des Gruppenrichtlinienobjekt-Editors überprüfen und konfigurieren:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\Sicherheitscenter**

Die Vorlagendatei „Securitycenter.admx“ enthält die XML-Einstellungsinformationen für diese Richtlinieneinstellung. Die folgende Tabelle beschreibt diese Einstellung.

**Tabelle 2.5 Einstellung für Windows-Sicherheitscenter**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Sicherheitscenter aktivieren (nur Domänencomputer)

</td>

<td style="border:1px solid black;">


Diese Einstellung gibt an, ob das Sicherheitscenter auf den Computern der Benutzer aktiviert oder deaktiviert ist. Die Einstellung gilt für die Computer, die zu einer Domäne gehören, in der Active Directory verwendet wird. Wenn für diese Einstellung der Standardwert „Nicht konfiguriert“ beibehalten wird, wird das Sicherheitscenter für Computer, die Mitglied der Domäne sind, deaktiviert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für diese Einstellung. Weitere Informationen zu dieser Einstellung finden Sie auf der Registerkarte **Erklärung** der Einstellung im Gruppenrichtlinienobjekt-Editor.


#### Tool zum Entfernen bösartiger Software

Das Tool zum Entfernen bösartiger Software in Microsoft Windows wurde entwickelt, um Malware von infizierten Computern zu entfernen. Jeden Monat veröffentlicht Microsoft eine neue Version des Tools über Microsoft Update, Windows Update, WSUS und das Microsoft Download Center. Da das Tool zum Entfernen bösartiger Software kein Antivirenprodukt mit vollständigem Funktionsumfang darstellt, empfiehlt Microsoft dringend, dass die Benutzer zudem Antivirensoftware ausführen, die fortlaufend Viren erkennt und löscht. Wenn das Tool ausgeführt wird, überprüft es Ihren Computer im Hintergrund und erstellt einen Bericht, wenn Infektionen erkannt wurden. Dieses Tool wird nicht als Bestandteil des Betriebssystems installiert, das es scannt. Für dieses Tool sind keine Gruppenrichtlinieneinstellungen in Windows Vista verfügbar.

Risikobewertung

Microsoft empfiehlt, dass zusätzlich zu den Schutzdiensten in Windows Vista noch ein Echtzeit-Virenscanner ausgeführt wird. Allerdings bestehen selbst bei Verwendung dieser Schutzmaßnahmen weiterhin zwei Risiken für Unternehmen:
* Der installierte Echtzeit-Virenscanner erkennt ein bestimmtes Vorkommen von Malware nicht.

* Der Malware gelingt es, den installierten Echtzeit-Virenscanner zu deaktivieren.


Für diese Situationen stellt das Tool zum Entfernen bösartiger Software eine zusätzliche Sicherheitsebene bereit, die zum Erkennen und Entfernen gängiger schädlicher Software beiträgt.

Risikominderung

Um diese Risiken zu mindern, empfiehlt Microsoft, dass Sie auf Ihren Clientcomputern die automatischen Updates aktivieren. Auf diese Weise wird das Tool zum Entfernen bösartiger Software heruntergeladen und ausgeführt, sobald eine neue Version veröffentlicht wird.

Wenn Sie die Verwendung dieses Tools in Ihrer Umgebung in Betracht ziehen, sollten Sie die Punkte in der folgenden Liste berücksichtigen, um die erfolgreiche Bereitstellung zu unterstützen:
* Das Tool zum Entfernen bösartiger Software weist eine Größe von rund 4 MB auf. Dies kann die Internetverbindung eines Unternehmens beeinträchtigen, wenn viele Clientcomputer gleichzeitig versuchen, das Tool herunterzuladen.

* Das Tool ist in erster Linie für Benutzer außerhalb von Unternehmen gedacht, auf deren Computern keine aktuelle Antivirenlösung installiert ist. Sie können das Tool jedoch auch in einer Unternehmensumgebung bereitstellen, um den vorhandenen Schutz zu verbessern und eine weitere Komponente zu Ihrer Strategie für tief greifenden Schutz hinzuzufügen. Sie können das Tool in einer Unternehmensumgebung mit einer oder mehreren der folgenden Methoden bereitstellen:
    - Windows Server Update Services

    - SMS-Softwarepaket

    - Auf Gruppenrichtlinien basierendes Computerstartskript

    - Auf Gruppenrichtlinien basierendes Benutzeranmeldeskript


Für Unternehmensumgebungen empfiehlt Microsoft den Microsoft Knowledge Base-Artikel 891716 [Bereitstellung des Microsoft Windows-Tools zum Entfernen bösartiger Software in einer Unternehmensumgebung](http://support.microsoft.com/kb/891716).

* Typischerweise erstellt das Windows-Tool zum Entfernen bösartiger Software ein temporäres Verzeichnis mit zufälligem Namen auf dem Stammlaufwerk Ihres Computers. Dieses Verzeichnis enthält mehrere Dateien sowie die Datei „Mrtstub.exe“. In den meisten Fällen wird dieser Ordner automatisch gelöscht, nachdem das Tool ausgeführt wurde oder der Computer den nächsten Neustart ausgeführt hat. Manchmal wird dieser Ordner jedoch nicht automatisch gelöscht. In diesen Fällen können Sie den Ordner manuell löschen, ohne dass dies negative Auswirkungen auf den Computer hätte.

* Ein Benutzer kann sich an einem Computer auch dann anmelden, wenn das Tool zum Entfernen bösartiger Software im Hintergrund ausgeführt wird. (Das Tool kann als Bestandteil einer Bereitstellung unter Verwendung der Windows Server Update Services ausgeführt werden.) In diesem Fall informiert Windows möglicherweise den Benutzer, dass das aktuelle Benutzerprofil beschädigt ist und ein neues Profil erstellt wird. Um dieses Problem zu lösen, kann das neue Profil gelöscht werden. Der Benutzer kann sich zu einem Zeitpunkt erneut am System anmelden, zu dem das Tool nicht ausgeführt wird. Dieses Problem tritt mit größter Wahrscheinlichkeit auf einem Computer mit dem Betriebssystem Windows 2000 auf.


#### Verfahren zur Risikominderung

Um das Tool zum Entfernen bösartiger Software wirksam zu verwenden, ziehen Sie den folgenden Prozess heran.

**So verwenden Sie dieses Verfahren zur Risikominderung**
1. Machen Sie sich mit den Fähigkeiten des Tools zum Entfernen bösartiger Software vertraut.

    Weitere Informationen finden Sie auf der Website für das [Tool zum Entfernen bösartiger Software](http://www.microsoft.com/germany/technet/sicherheit/tools/msrt.mspx).

2. Beurteilen Sie, ob das Tool in Ihrer Umgebung erforderlich ist.

3. Bestimmen Sie die am besten geeignete Methode zum Bereitstellen des Tools in Ihrem Unternehmen.

4. Identifizieren Sie die Systeme in Ihrem Unternehmen, die durch das Tool besser geschützt werden könnten.

5. Stellen Sie das Tool über die ausgewählte Bereitstellungsmethode bereit.



#### Richtlinien für Softwareeinschränkungen

Richtlinien für Softwareeinschränkungen bieten Administratoren die Möglichkeit, Anwendungssoftware zu identifizieren und ihre Ausführung auf lokalen Computern zu kontrollieren. Diese Funktion kann dazu beitragen, Computer mit den Betriebssystemen Windows Vista und Windows XP Professional vor bekannten Konflikten sowie vor schädlicher Software wie Viren und trojanischen Pferden zu schützen. Richtlinien für Softwareeinschränkungen können vollständig in Active Directory und die Gruppenrichtlinien integriert werden. Diese Funktion kann auch auf eigenständigen Computern verwendet werden. Richtlinien für Softwareeinschränkungen können für folgende Zwecke verwendet werden:
* Kontrollieren, welche Software auf den Clientcomputern in der Umgebung ausgeführt werden kann

* Einschränken des Zugriffs auf bestimmte Dateien auf Computern mit mehreren Benutzern

* Festlegen der Personen, die vertrauenswürdige Herausgeber zu Clientcomputern hinzufügen dürfen

* Definieren, ob die Richtlinien alle Benutzer betreffen oder nur einen Teil der Benutzer auf den Clientcomputern

* Verhindern der Ausführung von Programmdateien auf lokalen Computern mithilfe von Richtlinien, die auf folgenden Ebenen festgelegt werden: Computer, Organisationseinheit (OU), Website und Domäne.


**Wichtig**:   Es ist wichtig, alle in diesem Handbuch besprochenen Richtlinieneinstellungen gründlich zu testen, bevor sie in einer Produktionsumgebung bereitgestellt werden. Dies gilt insbesondere für den Fall, dass Richtlinien für Softwareeinschränkungen festgelegt werden. Fehler im Entwurf oder der Implementierung dieser Funktion können für die Benutzer beträchtliche Probleme verursachen.

Die Richtlinien für Softwareeinschränkungen haben sich in Windows Vista nicht spürbar geändert. Daher werden sie in diesem Handbuch nicht behandelt. Weitere Informationen zum Entwerfen und Implementieren dieser Richtlinien finden Sie im Artikel [Using Software Restriction Policies to Protect Against Unauthorized Software](http://technet.microsoft.com/en-us/windowsvista/aa940985.aspx) (engl.).

[Zum Seitenanfang](#mainsection)  



### Schutztechnologien in Internet Explorer 7

Es ist möglich, dass schädliche Websites die Sicherheit von Ihnen verwalteten Clientcomputer beeinträchtigen. Internet Explorer 7 enthält Technologien, die dazu beitragen, die Installation unerwünschter Software verhindern, sowie Technologien, die vor der nicht autorisierten Weitergabe persönlicher Daten schützen und so für eine stark erhöhte Browsersicherheit und verbesserten Schutz vertraulicher Informationen sorgen. Zu den neuen Sicherheitstechnologien in Internet Explorer 7 zählen unter anderem:
* Geschützter Modus von Internet Explorer

* ActiveX-Auswahlmöglichkeit

* Schutz vor domänenübergreifenden Skriptangriffen

* Sicherheitsstatusleiste

* Phishingfilter

* Zusätzliche Sicherheitsfunktionen


Internet Explorer 7 ist sowohl für Windows Vista als auch Windows XP verfügbar. Unter Windows Vista können zusätzliche Funktionen von Internet Explorer genutzt werden. Beispielsweise stehen bestimmte Funktionen in Internet Explorer 7 wie der geschützte Modus und der Jugendschutz nicht zur Verfügung, wenn der Browser auf Clientcomputern unter Windows XP verwendet wird. Auch die Aero-Benutzeroberfläche ist in Internet Explorer 7 auf Computern mit Windows XP nicht verfügbar.


#### Geschützter Modus von Internet Explorer

Der geschützte Modus von Internet Explorer in Windows Vista bietet zusätzliche Sicherheitsmaßnahmen, die das Browsen im Internet für die Benutzer sicherer gestalten. Außerdem trägt der geschützte Modus dazu bei, dass böswillige Benutzer davon abgehalten werden, die Kontrolle über den Browser eines Benutzers zu übernehmen und Code über erhöhte Berechtigungen auszuführen.

Der geschützte Modus vermindert zuvor vorhandene Sicherheitsanfälligkeiten in den Erweiterungen des Browsers, indem verhindert wird, dass diese Erweiterungen für die automatische Installation von schädlichem Code ausgenutzt werden können. Der geschützte Modus verwendet in Windows Vista Mechanismen mit höheren Integritätsebenen, die den Zugriff auf Prozesse, Dateien und Registrierungsschlüssel beschränken. Die Anwendungsprogrammierschnittstelle (API) für den geschützten Modus ermöglicht es Softwareanbietern, Erweiterungen und Add-Ons für Internet Explorer zu entwickeln, die mit dem Dateisystem und der Registrierung interagieren, während sich der Browser im geschützten Modus befindet.

Im geschützten Modus wird Internet Explorer 7 mit verringerten Berechtigungen ausgeführt, um zu verhindern, dass Benutzerdateien, Systemdateien oder Einstellungen ohne die ausdrückliche Zustimmung des Benutzers geändert werden. Mit der neuen Browserarchitektur wird zudem ein „Maklerprozess“ eingeführt, der die Sicherheit vorhandener Anwendungen verbessert, wenn diese aus dem geschützten Modus mit höheren Berechtigungen versehen werden. Dadurch wird verhindert, dass Daten an andere Speicherorte als die Verzeichnisse mit geringen Rechten im Browser heruntergeladen werden, z. B. dem Ordner für temporäre Internetdateien.

Der geschützte Modus ist in Internet Explorer 7 standardmäßig für alle Sicherheitszonen mit Ausnahme der Zone der vertrauenswürdigen Sites aktiviert. Allerdings können die Benutzer den Modus deaktivieren, was die Gesamtsicherheit verringert. Aus diesem Grund aktivieren die im vorherigen Kapitel beschriebenen Gruppenrichtlinieneinstellungen für den Browser den geschützten Modus in allen Zonen mit Webinhalten außer in der Zone der vertrauenswürdigen Sites. Zudem wird verhindert, dass Benutzer diese Einstellung deaktivieren können.

Sie können die für den geschützten Modus von Internet Explorer 7 verfügbare Gruppenrichtlinieneinstellung in folgendem Verzeichnis des Gruppenrichtlinienobjekt-Editors überprüfen und konfigurieren:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\Internet Explorer\Internetsystemsteuerung\Sicherheitsseite\\&lt;Zone&gt;**

Die folgende Tabelle beschreibt diese Einstellung.

**Tabelle 2.6 Einstellung für den geschützten Modus**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Geschützten Modus aktivieren *

</td>

<td style="border:1px solid black;">


Wenn diese Einstellung aktiviert ist, wird der geschützter Modus eingeschaltet. Die Benutzer haben nicht die Möglichkeit, den geschützten Modus zu deaktivieren.  
Wenn diese Einstellung deaktiviert ist, wird der geschützter Modus ausgeschaltet. Die Benutzer haben nicht die Möglichkeit, den geschützten Modus zu aktivieren.  
Wenn für diese Einstellung „**Nicht konfiguriert“** gewählt wurde, können die Benutzer die Einstellung nach Wunsch aktivieren oder deaktivieren.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>

\* Diese Einstellung steht nur in Internet Explorer 7 mit Windows Vista zur Verfügung.

Diese Tabelle enthält eine einfache Beschreibung für diese Einstellung. Weitere Informationen zu dieser Einstellung finden Sie auf der Registerkarte **Erklärung** der Einstellung im Gruppenrichtlinienobjekt-Editor.

Der geschützte Modus ist für die folgenden Sicherheitsbereiche und -zonen in Internet Explorer 7 verfügbar:
* Internet

* Intranet

* Zone des lokalen Computers

* Sperrung der Zone des Internets

* Sperrung der Zone des Intranets

* Sperrung der Zone des lokalen Computers

* Sperrung der Zone eingeschränkter Sites

* Sperrung der Zone vertrauenswürdiger Sites

* Zone eingeschränkter Sites

* Zone vertrauenswürdiger Sites



#### ActiveX-Auswahlmöglichkeit

Internet Explorer 7 stellt in Verbindung mit Windows Vista einen leistungsfähigen neuen Sicherheitsmechanismus für die ActiveX-Plattform zur Verfügung, der zum Schutz von Benutzerinformationen und Computersystemen beitragen soll. Durch die ActiveX-Auswahlmöglichkeit werden automatisch alle Steuerelemente deaktiviert, die vom Benutzer nicht ausdrücklich zugelassen wurden. Dies mindert den potenziellen Missbrauch von vorinstallierten Steuerelementen.

In Windows Vista warnt die Informationsleiste Benutzer, bevor diese auf ein zuvor installiertes ActiveX-Steuerelemente zugreifen können, das noch nicht im Internet verwendet wurde. Dieser Benachrichtigungsmechanismus ermöglicht es dem Benutzer, für jedes Steuerelement jeweils einzeln den Zugriff zu erlauben oder zu verbieten. Dadurch wird die verfügbare Angriffsfläche weiter verkleinert. Böswillige Benutzer können keine Websites verwenden, um automatisierte Angriffe mit ActiveX-Steuerelementen zu starten, deren Verwendung im Internet nie vorgesehen war.


#### Schutz vor domänenübergreifenden Skriptangriffen

Neue Schutzmechanismen gegen domänenübergreifende Skriptangriffe tragen dazu bei, die Möglichkeiten schädlicher Websites zum Ausnutzen von Sicherheitsanfälligkeiten in anderen Websites zu begrenzen. Vor der Einführung des Schutzes vor domänenübergreifenden Skriptangriffen konnte ein Benutzer beispielsweise eine Seite auf einer schädlichen Website besuchen, die wiederum ein neues Browserfenster mit einer legitimen Seite (wie eine Banking-Website) öffnete, in der der Benutzer zur Eingabe von Kontoinformationen aufgefordert wurde. Diese Informationen konnten dann von einem Skript ausgelesen und dem Angreifer zur Verfügung gestellt werden. Mit Internet Explorer 7 trägt der Schutz vor domänenübergreifenden Skriptangriffen dazu bei, dass diese Arten von Angriffen nicht erfolgreich sind.


#### Sicherheitsstatusleiste

Die neue Sicherheitsstatusleiste in Internet Explorer 7 hilft Benutzern, schnell zwischen authentischen Websites und verdächtigen oder schädlichen Websites zu unterscheiden. Zur Bereitstellung dieser Informationen verbessert die Sicherheitsstatusleiste den Zugriff auf Informationen zu digitalen Zertifikaten, mit denen sichere Websites (HTTPS) leichter identifiziert werden können.

Die Sicherheitsstatusleiste bietet Benutzern klarere und auffälligere optische Hinweise, aus denen die Sicherheit und Identität von Websites hervorgeht. Die Technologie unterstützt auch Informationen über HA-Zertifikate (High Assurance), um sichere Websites (HTTPS) klar zu identifizieren, bei denen stärkere Identifizierungsmaßnahmen vorhanden sind.


#### Phishingfilter

Phishing ist eine Technik, mit der viele Angreifer versuchen, Computerbenutzer durch Tricks zur Preisgabe von persönlichen oder finanziellen Informationen über eine E-Mail-Nachricht oder Website zu verleiten. Phisher geben sich als legitime Personen oder Unternehmen aus, um Personen dazu zu bringen, persönliche Informationen wie Kennwörter für Konten oder Kreditkartennummern anzugeben. Der Phishingfilter in Internet Explorer 7 weist Benutzer auf verdächtige oder für Phishing bekannte Websites hin, um so das Browsen im Internet sicherer zu machen. Der Filter analysiert den Inhalt der Website auf bekannte Phishingtechniken und verwendet ein globales Netzwerk von Datenquellen, um die Vertrauenswürdigkeit von Websites zu beurteilen.

Entwickler, die betrügerische E-Mails, Onlinewerbung und Websites erstellen, nutzen mangelnde Kommunikation und unzureichenden Informationsaustausch aus. Der neue Phishingfilter in Internet Explorer 7 verwendet einen Onlinedienst, der den Filter jede Stunde mehrmals aktualisiert. Er fasst die aktuellsten Informationen der Branche über betrügerische Websites zusammen und teilt diese Informationen Benutzern von Internet Explorer 7 mit, um diese proaktiv zu warnen und zu ihrem Schutz beizutragen.

Der Phishingfilter kombiniert clientseitige Überprüfungen auf verdächtige Merkmale von Websites mit einem optionalen Onlinedienst. Der Filter trägt auf dreifache Weise zum Schutz vor Phishing-Betrug bei:
* Er vergleicht die Adressen der Websites, die ein Benutzer besuchen möchte, mit einer Liste bestätigter legitimer Websites, die auf dem Computer des Benutzers gespeichert ist.

* Er analysiert Websites, die Benutzer besuchen möchten, indem er diese auf für Phishingsites gängige Merkmale untersucht.

* Er sendet die Adresse der Website, die ein Benutzer zu öffnen versucht, an einen von Microsoft unterhaltenen Onlinedienst, der die Adresse sofort mit einer häufig aktualisierten Liste mit Phishingsites abgleicht. Diese Websites wurden von seriösen Quellen als betrügerisch eingestuft und an Microsoft gemeldet.


Selbst wenn die Website dem Phishingfilterdienst unbekannt ist, kann Internet Explorer 7 das Verhalten der Website untersuchen und dem Benutzer melden, wenn verdächtige Aktivitäten erfolgen. Dazu zählt beispielsweise das Sammeln von Informationen zu Benutzern ohne ein SSL-Zertifikat (Secure Socket Layer). Auf diese Weise kann der Phishingfilter Websites bereits daran hindern, Benutzerinformationen zu sammeln, bevor eine Site offiziell gemeldet wurde.

Der Phishingfilter ist in Internet Explorer 7 standardmäßig so konfiguriert, dass die Benutzer anfänglich gefragt werden, ob sie den Filter aktivieren oder deaktivieren möchten. Die im vorherigen Kapitel beschriebenen Gruppenrichtlinieneinstellungen enthalten keine Einstellungen, die dieses Standardverhalten ändern. Es ist den Administratoren jedoch möglich, das Verhalten des Phishingfilters mit einer Gruppenrichtlinie zu steuern.

Sie können die Gruppenrichtlinieneinstellungen für den Phishingfilter in folgendem Verzeichnis des Gruppenrichtlinienobjekt-Editors überprüfen und konfigurieren:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\Internet Explorer**

Die folgende Tabelle beschreibt diese Einstellung.

**Tabelle 2.7 Einstellung für den Phishingfilter**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Verwaltung der Phishingfilter deaktivieren *

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht es dem Benutzer, einen Phishingfilter zu aktivieren, der eine Warnung ausgibt, falls die besuchte Website für betrügerische Versuche zum Sammeln persönlicher Informationen durch „Phishing“ bekannt ist.  
Standardmäßig wird der Benutzer aufgefordert, den Betriebsmodus für den Phishingfilter auszuwählen.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


*Um diese Einstellung nutzen zu können, muss der Computer Internet Explorer 7 unter einem der folgenden Betriebssysteme ausführen: Windows Vista, Windows XP SP2 oder Windows Server 2003 Service Pack 1 (SP1).

Diese Tabelle enthält eine einfache Beschreibung für diese Einstellung. Weitere Informationen zu dieser Einstellung finden Sie auf der Registerkarte **Erklärung** der Einstellung im Gruppenrichtlinienobjekt-Editor.

Microsoft empfiehlt, für diese Einstellung **Aktiviert** und für den Betriebsmodus **Automatisch** auszuwählen. Allerdings sollten Administratoren in diesem Zusammenhang berücksichtigen, dass bei dieser Konfiguration der Browser automatisch Informationen an Microsoft sendet, ohne den Benutzer zu fragen.


#### Zusätzliche Sicherheitsfunktionen

Internet Explorer enthält eine Reihe von spezialisierten Sicherheitsfunktionen, die zum Schutz vor Malware beitragen. Sie können all diese Einstellungen über Gruppenrichtlinien verwalten.

Sie können die für Internet Explorer 7 verfügbaren Gruppenrichtlinieneinstellungen für Sicherheitsfunktionen in folgendem Verzeichnis des Gruppenrichtlinienobjekt-Editors überprüfen und konfigurieren:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\Internet Explorer\Sicherheitsfunktionen**

Dieser Abschnitt enthält einen Überblick über diese Einstellungen in Internet Explorer 7. Eine vollständige Liste mit allen Gruppenrichtlinieneinstellungen für Internet Explorer 7 finden Sie im Gruppenrichtlinienobjekt-Editor.

**Hinweis**:   Alle Funktionen in diesem Abschnitt können auch mit Computern genutzt werden, auf denen Internet Explorer 6.0 oder höher mit den folgenden Betriebssystemen ausgeführt wird: Windows XP SP2 und Windows Server 2003 SP1.

#### Add-On-Verwaltung

Sie können mit den Richtlinieneinstellungen in diesem Abschnitt die Add-Ons beschränken, die von Internet Explorer 7 verwendet werden können. Die Einstellungen in der folgenden Tabelle dienen zum Verwalten von Add-Ons.

**Tabelle 2.8 Einstellungen für die Add-On-Verwaltung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Add-on-Liste

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht es Ihnen, eine Liste von Add-Ons zu verwalten.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind

</td>

<td style="border:1px solid black;">


Bei dieser Richtlinieneinstellung können nur die von Ihnen angegebenen Add-Ons mit Internet Explorer 7 ausgeführt werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Alle Prozesse

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Sie bestimmen, ob sich Benutzereinstellungen auf Prozesse (gemäß Einstellung in der Add-On-Verwaltung) oder Richtlinieneinstellungen auswirken.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Sie bestimmen, ob sich Benutzereinstellungen auf die aufgeführten Prozesse (gemäß Eingabe in der Add-On-Verwaltung) oder Richtlinieneinstellungen auswirken.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Sicherheitseinschränkung für Binärverhalten

Internet Explorer enthält verschiedene Arten von dynamischem Binärverhalten. Hierbei handelt es sich um Komponenten, die spezifische Funktionalität für die HTML-Elemente einkapseln, an die sie angefügt wurden. Sie können diese Verhaltenweisen mithilfe der Einstellungen in der folgenden Tabelle beschränken.

**Tabelle 2.9 Einstellungen zur Sicherheitseinschränkung für Binärverhalten**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Diese Einstellung steuert, ob die Einstellung für die Sicherheitseinschränkung für Binärverhalten verhindert oder zugelassen wird.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Nicht** **konfiguriert** oder **Aktiviert** festlegen, werden binäre Verhaltensweisen für Prozesse in Windows-Explorer und Internet Explorer verhindert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Administratoren Anwendungen definieren, für die diese Sicherheitsfunktion verhindert oder zugelassen wird.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Vom Administrator zugelassenes Verhalten

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen, wird damit eine Liste der Verhalten definiert, die in jeder Zone zugelassen sind, für die das Binär- und Skriptverhalten auf "Vom Administrator zugelassen" festgelegt ist.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Die vorherige Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Konsistente Mime-Verarbeitung

Internet Explorer verwendet MIME-Daten (Multipurpose Internet Mail Extensions), um Vorgehensweisen für die Behandlung von Dateien zu ermitteln, die über einen Webserver empfangen werden. Die folgende Tabelle enthält Informationen zu den Gruppenrichtlinieneinstellungen für MIME, die für Internet Explorer 7 verfügbar sind.

**Tabelle 2.10 Einstellungen für konsistente MIME-Verarbeitung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Durch diese Einstellung wird festgelegt, ob Internet Explorer erfordert, dass alle von Webservern bereitgestellten Dateitypinformationen konsistent sind.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Durch diese Einstellung wird festgelegt, ob Internet Explorer konsistente MIME-Daten für alle empfangenen Dateien erfordert.  
Wenn Sie für diese Richtlinieneinstellung **Nicht** **konfiguriert** oder **Aktiviert** festgelegt haben, erfordert Internet Explorer konsistente MIME-Daten für alle empfangenen Dateien.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Administratoren Anwendungen definieren, für die diese Sicherheitsfunktion verhindert oder zugelassen wird.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Informationsleiste

Mit den Richtlinieneinstellungen in diesem Abschnitt können Sie bestimmen, ob die Informationsleiste bei eingeschränkter Datei- oder Codeinstallation für andere Prozesse als Internet Explorer-Prozesse angezeigt wird. Standardmäßig wird die Informationsleiste für Internet Explorer-Prozesse angezeigt, jedoch nicht für Prozesse, wenn Datei- oder Codeinstallationen beschränkt sind. Die folgende Tabelle enthält Informationen zu den Einstellungen, mit denen Sie dieses Verhalten ändern können.

**Tabelle 2.11 Einstellungen für die Informationsleiste**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen, wird die Informationsleiste für alle Prozesse angezeigt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Deaktiviert** festlegen, wird die Informationsleiste nicht für Internet Explorer-Prozesse angezeigt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Richtlinieneinstellung können Sie festlegen, ob die Informationsleiste für spezifische Prozesse angezeigt wird, wenn Datei- oder Codeinstallationen eingeschränkt sind.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


#### Sperrung der Zone des lokalen Computers

Internet Explorer weist jeder geöffneten Webseite Zonenbeschränkungen zu, die sich nach dem Speicherort der Website richten (Internet, Intranet, Zone des lokalen Computers usw.). Webseiten auf dem lokalen Computer weisen die geringsten Sicherheitseinschränkungen auf und befinden sich in der Zone des lokalen Computers. Die Sicherheitseinstellung für die Zone des lokalen Computers gilt für alle lokalen Dateien und Inhalte. Diese Funktion trägt dazu bei, Angriffe abzumildern, wenn die Zone des lokalen Computers als Angriffsmittel zum Laden von schädlichem HTML-Code verwendet wird.

**Tabelle 2.12 Einstellungen für die Sperrung der Zone des lokalen Computers**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen, gelten die Sicherheitseinstellungen für die Zone des lokalen Computers für alle lokalen Dateien und Inhalte, die von anderen Prozessen als Internet Explorer oder den in einer Prozessliste definierten Prozessen verarbeitet werden.  
Standardmäßig gelten die Sicherheitseinstellungen für die Zone des lokalen Computers nicht für lokale Dateien oder Inhalte, die von anderen Prozessen als Internet Explorer oder den in einer Prozessliste definierten Prozessen verarbeitet werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Nicht** **konfiguriert** oder **Aktiviert** festlegen, gelten die Sicherheitseinstellungen für die Zone des lokalen Computers für alle lokalen Dateien und Inhalte, die von Internet Explorer verarbeitet werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen und einen Prozessnamen mit einem Wert von **1** definieren, gelten die Sicherheitseinstellungen für die Zone des lokalen Computers. Wenn Sie einen Wert von **0** definieren, gelten die Sicherheitseinstellungen für die Zone des lokalen Computers nicht.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Sicherheitsfunktion für MIME-Ermittlung

Diese Funktion trägt dazu bei, die Heraufstufung einer Datei eines bestimmten Dateityps zu einem gefährlicheren Dateityp zu verhindern. In der folgenden Tabelle werden die Einstellungen aufgeführt, die für diese Funktion verfügbar sind.

**Tabelle 2.13 Einstellungen für die Sicherheitsfunktion für MIME-Ermittlung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen, ist die Sicherheitsfunktion für MIME-Ermittlung für alle Prozesse aktiviert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Deaktiviert** festlegen, wird bei der MIME-Ermittlung in Internet Explorer-Prozessen die Heraufstufung einer Datei eines bestimmten Typs zu einem gefährlicheren Dateityp zugelassen.  
Das Standardverhalten (**Nicht** **konfiguriert**) lässt keine Heraufstufung zu.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Richtlinieneinstellung können Administratoren Anwendungen definieren, für die sie das Ausführen dieser Sicherheitsfunktion verhindern bzw. nicht zulassen möchten.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Sicherheitseinschränkung für MK-Protokoll

Die Richtlinieneinstellung „Sicherheitseinschränkung für MK-Protokoll“ verringert die Angriffsfläche, indem das MK-Protokoll blockiert wird. Wenn diese Einstellung aktiviert ist, können keine Ressourcen verwendet werden, die mit dem MK-Protokoll gehostet werden.

**Tabelle 2.14 Einstellungen für die Sicherheitseinschränkung für das MK-Protokoll**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Standardmäßig ist diese Einschränkung für alle Prozesse deaktiviert. Wenn Sie für diese Richtlinieneinstellung jedoch **Aktiviert** festlegen, wird das MK-Protokoll für alle Prozesse blockiert. Jegliche Verwendung des MK-Protokolls wird blockiert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Deaktiviert** festgelegt haben, können Anwendungen die API des MK-Protokolls verwenden. Ressourcen, die mit dem MK-Protokoll gehostet werden, können für Prozesse in Windows-Explorer und Internet Explorer verwendet werden.  
Die Standardeinstellung verhindert die Verwendung des MK-Protokolls für Windows-Explorer und Internet Explorer, und die mithilfe des MK-Protokolls gehosteten Ressourcen werden blockiert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Richtlinieneinstellung können Administratoren Anwendungen definieren, für die diese Sicherheitsfunktion verhindert oder zugelassen werden soll.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Netzwerkprotokollsperrung

Sie können Internet Explorer 7 so konfigurieren, dass aktive Inhalte, die über eingeschränkte Protokolle erhalten wurden, nicht auf unsichere Weise ausgeführt werden können. Diese Richtlinieneinstellung legt fest, ob das Beschränken von Inhalten verhindert oder zugelassen werden soll, die über eingeschränkte Protokolle erhalten werden.

**Tabelle 2.15 Einstellungen für die Netzwerkprotokollsperrung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen, ist das Beschränken von Inhalten, die über eingeschränkte Protokolle erhalten werden, für alle Prozesse außer Windows-Explorer oder Internet Explorer zulässig. Wenn Sie für diese Richtlinieneinstellung **Deaktiviert** festlegen, wird das Beschränken von Inhalten, die über eingeschränkte Protokolle erhalten werden, für alle Prozesse außer Windows-Explorer oder Internet Explorer verhindert. Die Standardeinstellung (**Nicht** **konfiguriert**) erzwingt diese Richtlinie nicht für andere Prozesse als Windows-Explorer und Internet Explorer.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen, ist das Beschränken von Inhalten, die über eingeschränkte Protokolle erhalten werden, für Prozesse in Windows-Explorer oder Internet Explorer zulässig. Wenn Sie für diese Richtlinieneinstellung **Deaktiviert** festlegen, wird das Beschränken von Inhalten, die über eingeschränkte Protokolle erhalten werden, für Prozesse in Windows-Explorer oder Internet Explorer verhindert. Die Standardeinstellung (**Nicht konfiguriert**) hat zur Folge, dass Internet Explorer diese Einstellung ignoriert.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Administratoren Anwendungen definieren, für die sie das Beschränken von Inhalten, die über eingeschränkte Protokolle erhalten werden, verhindern und zulassen möchten.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

Für jede Zone kann die Sicherheitseinschränkung „Netzwerkprotokollsperrung“ konfiguriert werden, um zu verhindern, dass aktive Inhalte, die über eingeschränkte Protokolle erhalten werden, auf unsichere Weise ausgeführt werden. Hierzu erfolgt entweder eine Abfrage an den Benutzer oder eine einfache Deaktivierung der Inhalte.

**Hinweis**:   Wenn Sie eine Richtlinie für eine Zone sowohl in der Computerkonfiguration als auch der Benutzerkonfiguration festlegen, beschränkt diese Maßnahme beide Protokolllisten für diese Zone.

**Tabelle 2.16 Einstellungen für eingeschränkte Protokolle pro Sicherheitszone**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Eingeschränkte Protokolle der Internetzone

</td>

<td style="border:1px solid black;">


Wenn diese Einstellung aktiviert ist, wird eine Liste der Protokolle erstellt, die für die Internetzone eingeschränkt sind.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Eingeschränkte Protokolle der Intranetzone

</td>

<td style="border:1px solid black;">


Wenn diese Einstellung aktiviert ist, wird eine Liste der Protokolle erstellt, die für die Intranetzone eingeschränkt sind.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Eingeschränkte Protokolle der Zone des lokalen Computers

</td>

<td style="border:1px solid black;">


Wenn diese Einstellung aktiviert ist, wird eine Liste der Protokolle erstellt, die für die Zone des lokalen Computers eingeschränkt sind.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Eingeschränkte Protokolle der Zone eingeschränkter Sites

</td>

<td style="border:1px solid black;">


Wenn diese Einstellung aktiviert ist, wird eine Liste der Protokolle erstellt, die für die Zone der eingeschränkten Sites eingeschränkt sind.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Eingeschränkte Protokolle der Zone vertrauenswürdiger Sites

</td>

<td style="border:1px solid black;">


Wenn diese Einstellung aktiviert ist, wird eine Liste der Protokolle erstellt, die für die Zone der vertrauenswürdigen Sites eingeschränkt sind.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Objektzwischenspeicherungsschutz

Diese Richtlinieneinstellung legt fest, ob ein Verweis auf ein Objekt zugänglich ist, wenn der Benutzer innerhalb derselben Domäne oder zu einer neuen Domäne navigiert.

**Tabelle 2.17 Einstellungen für den Objektzwischenspeicherungsschutz**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Einstellung **Deaktiviert** oder **Nicht** **konfiguriert** festlegen, wird der Objektverweis beibehalten, wenn innerhalb von Domänen oder über Domänen hinaus in der Zone der eingeschränkten Sites navigiert wird.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Einstellung **Nicht konfiguriert** beibehalten oder für die Einstellung **Aktiviert** festlegen, kann auf einen Objektverweis nicht mehr zugegriffen werden, wenn innerhalb von Domänen oder über Domänen hinaus für Internet Explorer-Prozesse navigiert wird.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Administratoren Anwendungen definieren, für die diese Sicherheitsfunktion verhindert oder zugelassen wird.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Schutz vor Zonenanhebung

Internet Explorer versieht jede Webseite, die geöffnet wird, mit Einschränkungen. Die Einschränkungen hängen vom Speicherort der Webseite ab (Internet, Intranet, Zone des lokalen Computers usw.). Beispielsweise weisen Webseiten auf dem lokalen Computer die geringsten Sicherheitseinschränkungen auf und befinden sich in der Zone des lokalen Computers. Dadurch wird die Zone des lokalen Computers zu einem bevorzugten Ziel für böswillige Benutzer.

**Tabelle 2.18 Einstellungen für den Schutz vor Zonenanhebung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Richtlinieneinstellung **Aktiviert** festlegen, können Sie Zonen für alle Prozesse vor der Zonenanhebung schützen.  
Wenn Sie für diese Einstellung **Nicht** **konfiguriert** beibehalten oder **Deaktiviert** festlegen, werden außer Internet Explorer-Prozessen oder den Prozessen in der Prozessliste keine Prozesse diesbezüglich geschützt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Einstellung **Nicht** **konfiguriert** beibehalten oder **Aktiviert** festlegen, kann jede Zone vor der Zonenanhebung durch Internet Explorer-Prozesse geschützt werden.  
Wenn Sie für diese Richtlinieneinstellung **Deaktiviert** festlegen, wird dieser Schutz nicht auf Internet Explorer-Prozesse angewendet.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Richtlinieneinstellung können Administratoren Anwendungen definieren, für die diese Sicherheitsfunktion verhindert oder zugelassen werden soll.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### ActiveX-Installation einschränken

Diese Richtlinieneinstellungen wenden Einschränkungen auf die Installation von ActiveX-Steuerelementen an.

**Tabelle 2.19 Einstellungen für das Einschränken von ActiveX-Installationen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht es Anwendungen, die das Browsersteuerelement hosten, die automatische Aufforderung zur Installation des ActiveX-Steuerelements zu blockieren.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht das Blockieren von Aufforderungen zur Installation von ActiveX-Steuerelementen für Internet Explorer-Prozesse.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Administratoren eine Liste von Programmdateien definieren, für die die automatische Aufforderung zur Installation von ActiveX-Steuerelementen zugelassen oder blockiert wird. Standardmäßig ist diese Sicherheitsfunktion zugelassen.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Dateidownload einschränken

Diese Richtlinieneinstellungen wenden Einschränkungen auf Dateidownloads an, die automatisch eingeleitet werden, ohne dass ein Benutzer den Download veranlasst.

**Tabelle 2.20 Einstellungen für die Einschränkung von Dateidownloads**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Anwendungen, die das Browsersteuerelement hosten, automatische Aufforderungen für Dateidownloads blockieren, die nicht vom Benutzer veranlasst wurden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Diese Einstellung ermöglicht es, Aufforderungen für nicht vom Benutzer veranlasste Dateidownloads zu blockieren.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Einstellung können Administratoren eine Liste von Programmdateien erstellen, bei denen das Blockieren der automatischen Aufforderung für nicht vom Benutzer veranlasste Dateidownloads zugelassen oder nicht zugelassen werden soll.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

#### Sicherheitseinschränkungen für Skriptfenster

Internet Explorer lässt zu, dass Skripts verschiedene Arten von Fenstern programmatisch öffnen, in der Größe anpassen und neu positionieren. Die Funktion „Sicherheitseinschränkungen für Skriptfenster“ schränkt Popupfenster ein und hindert Skripts am Anzeigen von Fenstern, in denen die Titel- und Statusleisten für den Benutzer nicht sichtbar sind bzw. die Titel- und Statusleisten anderer Fenster verbergen.

**Tabelle 2.21 Einstellungen für Sicherheitseinschränkungen für Skriptfenster**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Richtlinienobjekt

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


Alle Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Einstellung **Nicht** **konfiguriert** beibehalten oder **Deaktiviert** festlegen, werden Skriptfenster nicht eingeschränkt. Wenn Sie für diese Richtlinieneinstellung jedoch **Aktiviert** festlegen, werden Skriptfenster für alle Prozesse eingeschränkt.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internet Explorer-Prozesse

</td>

<td style="border:1px solid black;">


Wenn Sie für diese Einstellung **Nicht** **konfiguriert** beibehalten oder **Aktiviert** festlegen, gelten Popupfenster- und andere Einschränkungen für Prozesse in Windows-Explorer und Internet Explorer. Wenn Sie für diese Richtlinieneinstellung hingegen **Deaktiviert** festlegen, können Skripts weiterhin Popupfenster erstellen sowie Fenster, mit denen andere Fenster eventuell verborgen werden.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert ‡

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessliste

</td>

<td style="border:1px solid black;">


Mit dieser Richtlinieneinstellung können Administratoren Anwendungen definieren, für die diese Sicherheitsfunktion verhindert oder zugelassen werden soll.

</td>

<td style="border:1px solid black;">


Nicht konfiguriert

</td>

</tr>

</table>


Diese Tabelle enthält eine einfache Beschreibung für jede Einstellung. Weitere Informationen zu einer spezifischen Einstellung finden Sie auf der Registerkarte **Erklärung** der jeweiligen Einstellung im Gruppenrichtlinienobjekt-Editor.

[Zum Seitenanfang](#mainsection)  



### Weitere Informationen

Weitere Informationen zu den neuen und verbesserten Sicherheitsfunktionen und Technologien in Windows Vista finden Sie unter den folgenden Ressourcen:
* [Tool zum Entfernen bösartiger Software](http://www.microsoft.com/germany/technet/sicherheit/tools/msrt.mspx)

* [Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch06.mspx) (Kapitel 6 des *Windows XP-Sicherheitshandbuchs*)

* [User Account Control](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/uacppr.mspx)

* [Schutz vor nicht autorisierter Software mit Richtlinien für Softwareeinschränkung](http://www.microsoft.com/germany/technet/prodtechnol/winxppro/maintain/rstrplcy.mspx)

* [Windows Defender](http://www.microsoft.com/germany/athome/security/spyware/software/default.mspx)

* [Windows-Firewall](http://www.microsoft.com/technet/network/wf/default.mspx) (engl.)

* [Windows Server 2003 R2 – Group Policy](http://www.microsoft.com/windowsserver2003/technologies/management/grouppolicy/default.mspx) (engl.)

* [Windows Vista – Verbesserungen aus den Bereichen Sicherheit und Datenschutz](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/evaluate/feat/secfeat.mspx)

* [Windows XP – Command Shell Overview](http://www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/ntcmds_shelloverview.mspx) (engl.)

 
[Zum Seitenanfang](#mainsection)
 

#### In diesem Beitrag
* [Übersicht](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/default.mspx)
* [Kapitel 1: Implementieren der Sicherheitsbasis](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx)
* Kapitel 2: Schutz vor Malware
* [Kapitel 3: Schutz von vertraulichen Daten](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)
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

[![](https://technet.microsoft.com/de-de/Dd443673.pageLeft(de-de,TechNet.10).gif "Dd443673.pageLeft(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx)
3 von 7[![](https://technet.microsoft.com/de-de/Dd443673.pageRight(de-de,TechNet.10).gif "Dd443673.pageRight(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)

</td>

</tr>

</table>
