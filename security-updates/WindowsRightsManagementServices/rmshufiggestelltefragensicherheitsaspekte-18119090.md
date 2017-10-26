---
TOCTitle: 'RMS – Häufig gestellte Fragen: Sicherheitsaspekte'
Title: 'RMS – Häufig gestellte Fragen: Sicherheitsaspekte'
ms:assetid: 'ff433834-79aa-481f-bd39-3393be12a26f'
ms:contentKeyID: 18119090
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747757(v=WS.10)'
---

RMS – Häufig gestellte Fragen: Sicherheitsaspekte
=================================================

RMS-Sicherheitsaspekte – Häufig gestellte Fragen
------------------------------------------------

-   [Was ist das Administratorkonto?](#bkmk_43)
-   [Ist RMS eine Sicherheitslösung?](#bkmk_44)
-   [Welche Mechanismen wurden vorgesehen, um zu verhindern, dass Empfänger auf ihren Clientcomputern die Uhr zurückstellen, um ihren Zugriff auf ein durch Rechte geschütztes Dokument zu verlängern, nachdem ihre Nutzungslizenz abgelaufen ist?](#bkmk_45)
-   [Können Mitglieder der Gruppe „Domänen-Admins“ Dokumente lesen, die für Benutzer in ihrer Domäne bestimmt sind?](#bkmk_46)
-   [Jede Lockbox kann alle Zertifikate und Lizenzen, die im System erstellt wurden, authentifizieren und feststellen, dass sie jeweils von einem bei Microsoft registrierten Dienst stammen. Vor welchem Risiko schützt dieser Umstand?](#bkmk_47)
-   [Wenn es jemandem gelingt, ein Dokument „mit roher Gewalt“ (Brute Force Attack) zu öffnen, kann er mit dem darin enthaltenen Schlüssel dann auch andere Dokumente öffnen?](#bkmk_48)
-   [Sind aufgrund von Exportbeschränkungen für Verschlüsselungstechnologien Teile der Schlüssel auch außerhalb des Unternehmens sichtbar, in dem sie implementiert sind?](#bkmk_49)
-   [Wie wird verhindert, dass Angreifer die Außerbetriebsetzungsfunktion von außerhalb des Systems aktivieren?](#bkmk_50)
-   [Kann ein Benutzer Bildschirmaufnahmen von durch Rechte geschützten Inhalten erstellen?](#bkmk_51)
-   [Können Administratoren, die mit RMS zusammenhängende Dateien sichern, sich Zugriff auf durch Rechte geschützte Inhalte verschaffen?](#bkmk_52)
-   [Enthält die von Windows verwendete Auslagerungsdatei zu irgendeinem Zeitpunkt den unverschlüsselten Inhalt, sodass Inhalt eventuell „offengelegt“ wird?](#bkmk_53)
-   [Ist es möglich einzuschränken, welche Administratoren Zugriff auf die verschiedenen RMS-Verwaltungsfunktionen haben sollen?](#bkmk_54)
-   [Können mit RMS einzelne Dokumente geschützt werden, sobald sie auf der Festplatte des Benutzers oder in einem gemeinsamen Ordner erstellt werden?](#bkmk_55)
-   [Werden beim Öffnen einer Datei auch die Datei für automatische Speicherung sowie die temporäre Datei verschlüsselt?](#bkmk_56)
-   [Beim Empfang einer durch Rechte geschützten E-Mail hat es den Anschein, als hätte die E-Mail einen Anhang. Ich kann den Anhang speichern, obwohl die E-Mail angeblich nicht gespeichert werden kann. Ist dies ein Fehlverhalten von RMS?](#bkmk_562)

<span id="BKMK_43"></span>
#### Was ist das Administratorkonto?

RMS (Rights Management Services, Rechteverwaltungsdienste) unterstützt eine spezielle Administratorengruppe, die über Vollzugriff auf die gesamten durch Rechte geschützten Inhalte verfügt. Den Mitgliedern der Administratorengruppe werden volle Besitzerrechte in allen Nutzungslizenzen erteilt, die vom RMS-Cluster ausgestellt wurden, auf dem die Administratorengruppe konfiguriert ist. Dies bedeutet, dass Mitglieder dieser Gruppe alle geschützten Dateien beliebig entschlüsseln und ihren Schutz entfernen können. Ein Mitglied dieser Gruppe kann beispielsweise den Schutz von Dateien entfernen, die von einem gekündigten Mitarbeiter veröffentlicht wurden, damit ein neuer Besitzer die Dateien veröffentlichen und verwalten kann.

<span id="BKMK_44"></span>
#### Ist RMS eine Sicherheitslösung?

Nein, RMS ist keine Sicherheitslösung. Wenn es mit einer RMS-fähigen Anwendung, wie z. B. Office 2007, verwendet wird, erfüllt es die Funktion einer Lösung zur Durchsetzung von Richtlinien. Wenn ein Benutzer nicht zum Anzeigen von Daten berechtigt ist, kann er mittels „roher Gewalt“ (Brute Force Attack) versuchen, die Verschlüsselung zu brechen. Obwohl die Verschlüsselung robust ist, kann sie – wie alle Softwareverschlüsselungsschemas – geknackt werden. Wenn ein Benutzer jedoch zum Anzeigen der Daten berechtigt ist, kann er sie manuell kopieren oder ein digitales Abbild davon erstellen und diese Informationen unberechtigten Benutzern zur Verfügung stellen.

<span id="BKMK_45"></span>
#### Welche Mechanismen wurden vorgesehen, um zu verhindern, dass Empfänger auf ihren Clientcomputern die Uhr zurückstellen, um ihren Zugriff auf ein durch Rechte geschütztes Dokument zu verlängern, nachdem ihre Nutzungslizenz abgelaufen ist?

RMS erkennt, ob die Uhr auf einem Clientsystem zurückgestellt oder vorgestellt wurde, und verhindert, dass der Benutzer den Inhalt abrufen kann. Darüber hinaus kann RMS auch feststellen, ob eine messbare Zeitabweichung zwischen dem RMS-Server und dem Client vorliegt.

<span id="BKMK_46"></span>
#### Können Mitglieder der Gruppe „Domänen-Admins“ Dokumente lesen, die für Benutzer in ihrer Domäne bestimmt sind?

Mitglieder der Gruppe „Domänen-Admins“ können Inhalte lesen, die für ein Benutzerkonto geschützt wurden, wenn sie ein Mitglied der RMS-Administratorengruppe sind oder die Identität des Benutzers annehmen. Da die Mitglieder der Gruppe „Domänen-Admins“ die Benutzerkonten in der Domäne steuern können, gibt es kein Mittel gegen Mitglieder der Gruppe „Domänen-Admins“, die das in sie gesetzte Vertrauen missbrauchen.

Es hat sich bewährt, der Administratorengruppe nur die Mitglieder der Gruppe „Domänen-Admins“ hinzuzufügen, die auch tatsächlich Zugriff auf durch Rechte geschützte Inhalte benötigen. Bei Erteilung einer Lizenz für ein Mitglied der Administratorengruppe wird im Ereignisprotokoll der Anwendung auf dem RMS-Server ein Ereignis mit der Ereignis-ID 49 vermerkt. Die Ereignis-ID 49 besagt: **Einem Benutzer, der zur RMS-Administratorengruppe gehört, wurde eine Lizenz gewährt. Der Benutzer hat die folgende E-Mail-Adresse: &lt;Benutzeralias&gt;“**. **Benutzeralias** steht dabei für das E-Mail-Konto des Benutzers.

Ebenso wie bei anderen Gruppen, die für die Beschränkung des Zugriffs auf Ressourcen verwendet werden, sollten Sie auch hier Warnmeldungen definieren und Sicherheitsüberprüfungen ausführen, um zu verhindern, dass ein Benutzer unberechtigt Mitglied der Administratorengruppe wird.

<span id="BKMK_47"></span>
#### Jede Lockbox kann alle Zertifikate und Lizenzen, die im System erstellt wurden, authentifizieren und feststellen, dass sie jeweils von einem bei Microsoft registrierten Dienst stammen. Vor welchem Risiko schützt dieser Umstand?

Ohne die Möglichkeit zur Überprüfung der Integrität von Zertifikaten könnte ein Benutzer ein für einen anderen Benutzer ausgestelltes Rechtekontozertifikat (Rights Account Certificate oder RAC) fälschen und eine Nutzungslizenz für Inhalte abrufen oder eine Anwendung erstellen, mit der die Schutzfunktionen eines Dokuments entfernt werden.

<span id="BKMK_48"></span>
#### Wenn es jemandem gelingt, ein Dokument „mit roher Gewalt“ (Brute Force Attack) zu öffnen, kann er mit dem darin enthaltenen Schlüssel dann auch andere Dokumente öffnen?

Jeder durch Rechte geschützte Inhalt wird mit einem anderen zufällig erstellten symmetrischen Schlüssel verschlüsselt. Deshalb ist der Schlüssel eines jeden Dokuments eindeutig und kann nicht zum Entschlüsseln anderer Dokumente verwendet werden.

<span id="BKMK_49"></span>
#### Sind aufgrund von Exportbeschränkungen für Verschlüsselungstechnologien Teile der Schlüssel auch außerhalb des Unternehmens sichtbar, in dem sie implementiert sind?

Anwendungen, die vom Microsoft-Vertrauensstamm signiert wurden, unterliegen dem Microsoft-Vertrauensstamm zum Signieren von Schlüsseln. Von diesem Punkt an werden Schlüssel jedoch weder durch Microsoft noch durch die Implementierung eines Kunden offengelegt.

<span id="BKMK_50"></span>
#### Wie wird verhindert, dass Angreifer die Außerbetriebsetzungsfunktion von außerhalb des Systems aktivieren?

Der Angreifer benötigt die Anmeldeinformationen eines Benutzerkontos mit Administratorberechtigungen für den RMS-Cluster. Standardmäßig ist die RMS-Verwaltungsschnittstelle nur lokal auf dem RMS-Server verfügbar. Das Risiko lässt sich minimieren, indem sichergestellt wird, dass die Schnittstelle auch weiterhin nur lokal verfügbar ist, dass RDP (Remote Desktop Protocol) deaktiviert ist und dass der Server physisch sicher ist.

<span id="BKMK_51"></span>
#### Kann ein Benutzer Bildschirmaufnahmen von durch Rechte geschützten Inhalten erstellen?

Wenn in den RMS-Rechten festgelegt ist, dass die Kopierfunktion nicht zulässig ist, wird unter Windows die Tastenkombination Alt+Druck von RMS deaktiviert. In einer Umgebung mit nicht verwalteten Desktops kann ein Benutzer jedoch nicht von Microsoft stammende Produkte verwenden, um den Bildschirminhalt als Bild zu kopieren.

<span id="BKMK_52"></span>
#### Können Administratoren, die mit RMS zusammenhängende Dateien sichern, sich Zugriff auf durch Rechte geschützte Inhalte verschaffen?

Nein, sie können zwar die Sicherung vornehmen, haben jedoch keinen Zugriff auf die Dateien.

<span id="BKMK_53"></span>
#### Enthält die von Windows verwendete Auslagerungsdatei zu irgendeinem Zeitpunkt den unverschlüsselten Inhalt, sodass Inhalt eventuell „offengelegt“ wird?

Wenn der RMS-Client entschlüsselten Inhalt zurück an die Anwendung sendet, kann dieser Inhalt in der Auslagerungsdatei enthalten sein. In den Empfehlungen zur RMS-Anwendungsentwicklung im RMS-SDK werden Maßnahmen genannt, um dies zu verhindern; sie müssen jedoch von der RMS-fähigen Anwendung umgesetzt werden.

<span id="BKMK_54"></span>
#### Ist es möglich einzuschränken, welche Administratoren Zugriff auf die verschiedenen RMS-Verwaltungsfunktionen haben sollen?

Ja, Sie können verschiedene RMS-Administratorengruppen in Active Directory erstellen, den Gruppen Benutzer hinzufügen und dann die entsprechende Zugriffssteuerungsliste (Access Control List, ACL) für die Verwaltungsseiten erstellen. In der Standardkonfiguration der Zugriffssteuerungslisten für die RMS-Verwaltungswebsite hat beispielsweise nur der Benutzer Zugriff auf die Seite „Sicherheitseinstellungen“, der den Server auch bereitgestellt hat.

<span id="BKMK_55"></span>
#### Können mit RMS einzelne Dokumente geschützt werden, sobald sie auf der Festplatte des Benutzers oder in einem gemeinsamen Ordner erstellt werden?

RMS kann zwar dazu verwendet werden, die auf dem lokalen Computer eines Benutzers gespeicherten Dokumente zu schützen, das verschlüsselnde Dateisystem (Encrypting File System, EFS) eignet sich jedoch besser dafür. EFS schützt Dokumente transparent, während in RMS manuelle Eingriffe (in Form einiger Mausklicks) erforderlich sind, um ein Dokument zu schützen.

<span id="BKMK_56"></span>
#### Werden beim Öffnen einer Datei auch die Datei für automatische Speicherung sowie die temporäre Datei verschlüsselt?

Ja, alle temporären Dateien werden verschlüsselt.

<span id="BKMK_562"></span>
#### Beim Empfang einer durch Rechte geschützten E-Mail hat es den Anschein, als hätte die E-Mail einen Anhang. Ich kann den Anhang speichern, obwohl die E-Mail angeblich nicht gespeichert werden kann. Ist dies ein Fehlverhalten von RMS?

Nein, dies ist kein Fehlverhalten. Der angezeigte Anhang ist die verschlüsselte Nachricht, bevor der RMS-Client sie entschlüsselt hat. Sie ist noch immer durch Rechte geschützt und kann nach dem Entschlüsseln nicht gespeichert werden.