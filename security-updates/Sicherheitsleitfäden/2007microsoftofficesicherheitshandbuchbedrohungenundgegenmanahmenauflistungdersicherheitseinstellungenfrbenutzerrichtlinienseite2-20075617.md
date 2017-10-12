---
Title: 2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2
TOCTitle: 2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2
ms:assetid: b322971a-8efe-40a3-ba33-30a25cae5219
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443674(v=TechNet.10)
ms:contentKeyID: 20075617
---


# 2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen


### Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2
Veröffentlicht: 11. Nov 2007
 

Die Einstellungen im folgenden Abschnitt sind nach Namen aufgeführt.
Auf dieser Seite
[Informationen zu Benutzerrichtlinieneinstellungen](#ecd)  ## Informationen zu Benutzerrichtlinieneinstellungen

Für jede Einstellung werden neben einer Beschreibung auch Informationen über die betroffenen Anwendungen, das behandelte Sicherheitsrisiko, die Art und Weise, in der das Sicherheitsrisiko behandelt wird, und eventuelle andere Erwägungen bereitgestellt. Darüber hinaus ist für jede Einstellung eine Tabelle enthalten, die den Speicherort der Einstellung in der Gruppenrichtlinie, die ADM-Datei mit der Einstellung sowie die empfohlene Konfiguration für EC- und SSLF-Umgebungen aufführt.

### Eingabeaufforderung für Outlook-Objektmodell beim Zugriff auf Adressinformationen mithilfe von „UserProperties.Find“ konfigurieren

Betrifft: **Outlook**

Diese Einstellung steuert, was geschieht, wenn ein Programm unter Verwendung der UserProperties.Find-Methode des Outlook-Objektmodells einen Zugriffsversuch auf Adressinformationen unternimmt.

#### Sicherheitsrisiko

Wenn eine nicht vertrauenswürdige Anwendung auf Adressinformationen zugreift, könnte die Anwendung damit Zugriff auf vertrauliche Daten erhalten und diese Daten möglicherweise ändern.

Wenn eine nicht vertrauenswürdige Anwendung unter Verwendung der UserProperties.Find-Methode einen Zugriffsversuch auf Adressinformationen unternimmt, greift Outlook 2007 auf die im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters konfigurierte Einstellung zurück. Diese Einstellung legt fest, wann Outlook den Benutzern eine Warnung zu programmgesteuerten Zugriffsversuchen ausgibt:
* Nur, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird (die Standardeinstellung)
* Immer
* Niemals

Wenn ausgewählt ist, dass niemals Warnungen ausgegeben werden sollen, gewährt Outlook automatisch den programmgesteuerten Zugriff auf alle Programme, die diesen anfordern. Dadurch könnte ein schädliches Programm Zugriff auf vertrauliche Informationen erhalten.
Hinweis:
Bei der beschriebenen Standardfunktionalität wird vorausgesetzt, dass Sie nicht der Empfehlung gefolgt sind, die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ zu aktivieren, um sicherzustellen, dass Outlook-Sicherheitseinstellungen durch die Gruppenrichtlinie konfiguriert werden. Wenn Gruppenrichtlinien-Sicherheitseinstellungen für Outlook verwendet werden, wird der Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters nicht verwendet. In dieser Situation besteht die Standardeinstellung darin, den Benutzern eine Eingabeaufforderung auf Grundlage der Computersicherheit zu senden. Dies entspricht der Option „Nur wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird“ im Vertrauensstellungscenter, und hat keine Auswirkungen auf die Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus vier verschiedenen Optionen auswählen, wenn ein nicht vertrauenswürdiges Programm mithilfe der UserProperties.Find-Methode des Outlook-Objektmodells einen Zugriffsversuch auf Adressinformationen unternimmt:
* **Eingabeaufforderung für Benutzer**. Der Benutzer wird aufgefordert, jeden Zugriffsversuch zu genehmigen.
* **Automatisch genehmigen**. Outlook erfüllt automatisch alle programmgesteuerten Zugriffsanforderungen aller Programme. Durch diese Option entsteht möglicherweise ein erhebliches Sicherheitsrisiko. Sie wird daher nicht empfohlen.
* **Automatisch ablehnen**. Outlook verweigert automatisch alle programmgesteuerten Zugriffsanforderungen von allen Programmen.
* **Benutzer basierend auf der Computersicherheit auffordern**. Outlook sendet Benutzern nur eine Eingabeaufforderung, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird.

**Tabelle 1.66. Eingabeaufforderung für Outlook-Objektmodell beim Zugriff auf Adressinformationen mithilfe von „UserProperties.Find“ konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


Outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Automatisch ablehnen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1454

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **Benutzer basierend auf der Computersicherheit auffordern** wird die Standardkonfiguration von Outlook 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.
Wichtig:

Sie müssen ebenfalls die Einstellung „Outlook-Sicherheitsmodus“ unter „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen, damit diese Einstellung angewendet wird.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Eingabeaufforderung für Outlook-Objektmodell beim Zugriff auf ein Adressbuch konfigurieren

Betrifft: **Outlook**

Diese Einstellung steuert, was geschieht, wenn ein nicht vertrauenswürdiges Programm unter Verwendung des Outlook-Objektmodells einen Zugriffsversuch auf ein Adressbuch unternimmt.

#### Sicherheitsrisiko

Wenn eine nicht vertrauenswürdige Anwendung auf das Adressbuch zugreift, könnte die Anwendung damit Zugriff auf vertrauliche Daten erhalten und diese Daten möglicherweise ändern.

Wenn eine nicht vertrauenswürdige Anwendung programmgesteuert einen Zugriffsversuch auf Adressinformationen unternimmt, greift Outlook 2007 auf die im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters konfigurierte Einstellung zurück. Diese Einstellung legt fest, wann Outlook den Benutzern eine Warnung zu programmgesteuerten Zugriffsversuchen ausgibt:
* Nur, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird (die Standardeinstellung)
* Immer
* Niemals

Wenn ausgewählt ist, dass niemals Warnungen ausgegeben werden sollen, gewährt Outlook automatisch den programmgesteuerten Zugriff auf alle Programme, die diesen anfordern. Dadurch könnte ein schädliches Programm Zugriff auf vertrauliche Informationen erhalten.
Hinweis:

Bei der beschriebenen Standardfunktionalität wird vorausgesetzt, dass Sie nicht der Empfehlung gefolgt sind, die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ zu aktivieren, um sicherzustellen, dass Outlook-Sicherheitseinstellungen durch die Gruppenrichtlinie konfiguriert werden. Wenn Gruppenrichtlinien-Sicherheitseinstellungen für Outlook verwendet werden, wird der Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters nicht verwendet. In dieser Situation besteht die Standardeinstellung darin, den Benutzern eine Eingabeaufforderung auf Grundlage der Computersicherheit zu senden. Dies entspricht der Option „Nur wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird“ im Vertrauensstellungscenter, und hat keine Auswirkungen auf die Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus vier verschiedenen Optionen auswählen, wenn ein nicht vertrauenswürdiges Programm unter Verwendung des Outlook-Objektmodells einen Zugriffsversuch auf ein Adressbuch unternimmt:
* **Eingabeaufforderung für Benutzer**. Der Benutzer wird aufgefordert, jeden Zugriffsversuch zu genehmigen.
* **Automatisch genehmigen**. Outlook erfüllt automatisch alle programmgesteuerten Zugriffsanforderungen aller Programme. Durch diese Option entsteht möglicherweise ein erhebliches Sicherheitsrisiko. Sie wird daher nicht empfohlen.
* **Automatisch ablehnen**. Outlook verweigert automatisch alle programmgesteuerten Zugriffsanforderungen von allen Programmen.
* **Benutzer basierend auf der Computersicherheit auffordern**. Outlook greift auf die Einstellung im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters zurück, wie oben beschrieben.

**Tabelle 1.65. Eingabeaufforderung für Outlook-Objektmodell beim Zugriff auf ein Adressbuch konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


Outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Automatisch ablehnen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1004

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **Benutzer basierend auf der Computersicherheit auffordern** wird die Standardkonfiguration von Outlook 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.
Wichtig:

Sie müssen ebenfalls die Einstellung „Outlook-Sicherheitsmodus“ unter „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen, damit diese Einstellung angewendet wird.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Eingabeaufforderung für Outlook-Objektmodell beim Zugriff auf die Formula-Eigenschaft eines UserProperty-Objekts konfigurieren

Betrifft: **Outlook**

Diese Einstellung steuert, was geschieht, wenn ein Benutzer in Outlook 2007 ein benutzerdefiniertes Formular entwirft und versucht, ein Adressinformationsfeld an ein benutzerdefiniertes Kombinations- oder Formelfeld zu binden.

#### Sicherheitsrisiko

Ein benutzerdefiniertes Formular in Outlook könnte zum Zugriff auf vertrauliche Adressbuchdaten und zum potenziellen Ändern dieser Daten verwendet werden.

Wenn ein Benutzer versucht, in einem benutzerdefinierten Formular ein Adressinformationsfeld an ein benutzerdefiniertes Kombinations- oder Formelfeld zu binden, greift Outlook 2007 standardmäßig auf die im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters konfigurierte Einstellung zurück. Diese Einstellung legt fest, wann Outlook den Benutzern eine Warnung zu programmgesteuerten Zugriffsversuchen ausgibt:
* Nur, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird (die Standardeinstellung)
* Immer
* Niemals

Wenn ausgewählt ist, dass niemals Warnungen ausgegeben werden sollen, gewährt Outlook automatisch den programmgesteuerten Zugriff auf alle Programme, die diesen anfordern. Dadurch könnte ein schädliches Programm Zugriff auf vertrauliche Informationen erhalten.
Hinweis:

Bei der beschriebenen Standardfunktionalität wird vorausgesetzt, dass Sie nicht der Empfehlung gefolgt sind, die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ zu aktivieren, um sicherzustellen, dass Outlook-Sicherheitseinstellungen durch die Gruppenrichtlinie konfiguriert werden. Wenn Gruppenrichtlinien-Sicherheitseinstellungen für Outlook verwendet werden, wird der Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters nicht verwendet. In dieser Situation besteht die Standardeinstellung darin, den Benutzern eine Eingabeaufforderung auf Grundlage der Computersicherheit zu senden. Dies entspricht der Option „Nur wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird“ im Vertrauensstellungscenter, und hat keine Auswirkungen auf die Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus vier verschiedenen Optionen auswählen, wenn ein nicht vertrauenswürdiges Programm mithilfe der UserProperties.Find-Methode des Outlook-Objektmodells einen Zugriffsversuch auf Adressinformationen unternimmt:
* **Eingabeaufforderung für Benutzer**. Der Benutzer wird aufgefordert, jeden Zugriffsversuch zu genehmigen.
* **Automatisch genehmigen**. Outlook erfüllt automatisch alle programmgesteuerten Zugriffsanforderungen aller Programme. Durch diese Option entsteht möglicherweise ein erhebliches Sicherheitsrisiko. Sie wird daher nicht empfohlen.
* **Automatisch ablehnen**. Outlook verweigert automatisch alle programmgesteuerten Zugriffsanforderungen von allen Programmen.
* **Benutzer basierend auf der Computersicherheit auffordern**. Outlook sendet Benutzern nur eine Eingabeaufforderung, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird.

**Tabelle 1.67. Eingabeaufforderung für Outlook-Objektmodell beim Zugriff auf die Formula-Eigenschaft eines UserProperty-Objekts konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


Outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Automatisch ablehnen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1573

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **Benutzer basierend auf der Computersicherheit auffordern** wird die Standardkonfiguration von Outlook 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.
Wichtig:

Sie müssen ebenfalls die Einstellung „Outlook-Sicherheitsmodus“ unter „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen, damit diese Einstellung angewendet wird.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Eingabeaufforderung für Outlook-Objektmodell beim Ausführen von „Speichern unter“ konfigurieren

Betrifft: **Outlook**

Diese Einstellung steuert, was geschieht, wenn ein nicht vertrauenswürdiges Programm versucht, unter Verwendung des Befehls **Speichern unter** ein Element programmgesteuert zu speichern.

#### Sicherheitsrisiko

Wenn eine nicht vertrauenswürdige Anwendung mithilfe des Befehls **Speichern unter** ein Element programmgesteuert speichert, könnte die Anwendung dem Posteingang, dem öffentlichen Ordner oder einem Adressbuch eines Benutzers schädliche Daten hinzufügen.

Wenn eine nicht vertrauenswürdige Anwendung versucht, den Befehl **Speichern unter** zu verwenden, greift Outlook 2007 auf die im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters konfigurierte Einstellung zurück. Diese Einstellung legt fest, wann Outlook den Benutzern eine Warnung zu programmgesteuerten Zugriffsversuchen ausgibt:
* Nur, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird (die Standardeinstellung)
* Immer
* Niemals

Wenn ausgewählt ist, dass niemals Warnungen ausgegeben werden sollen, gewährt Outlook automatisch den programmgesteuerten Zugriff auf alle Programme, die diesen anfordern. Dadurch könnte ein schädliches Programm Zugriff auf vertrauliche Informationen erhalten.
Hinweis:

Bei der beschriebenen Standardfunktionalität wird vorausgesetzt, dass Sie nicht der Empfehlung gefolgt sind, die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ zu aktivieren, um sicherzustellen, dass Outlook-Sicherheitseinstellungen durch die Gruppenrichtlinie konfiguriert werden. Wenn Gruppenrichtlinien-Sicherheitseinstellungen für Outlook verwendet werden, wird der Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters nicht verwendet. In dieser Situation besteht die Standardeinstellung darin, den Benutzern eine Eingabeaufforderung auf Grundlage der Computersicherheit zu senden. Dies entspricht der Option „Nur wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird“ im Vertrauensstellungscenter, und hat keine Auswirkungen auf die Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus vier verschiedenen Optionen auswählen, wenn ein nicht vertrauenswürdiges Programm versucht, ein Element mithilfe des Befehls **Speichern unter** programmgesteuert zu speichern:
* **Eingabeaufforderung für Benutzer**. Der Benutzer wird aufgefordert, jeden Zugriffsversuch zu genehmigen.
* **Automatisch genehmigen**. Outlook erfüllt automatisch alle programmgesteuerten Zugriffsanforderungen aller Programme. Durch diese Option entsteht möglicherweise ein erhebliches Sicherheitsrisiko. Sie wird daher nicht empfohlen.
* **Automatisch ablehnen**. Outlook verweigert automatisch alle programmgesteuerten Zugriffsanforderungen von allen Programmen.
* **Benutzer basierend auf der Computersicherheit auffordern**. Outlook sendet Benutzern nur eine Eingabeaufforderung, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird.

**Tabelle 1.68. Eingabeaufforderung für Outlook-Objektmodell beim Ausführen von „Speichern unter“ konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Automatisch ablehnen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1568

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **Benutzer basierend auf der Computersicherheit auffordern** wird die Standardkonfiguration von Outlook 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.
Wichtig:

Sie müssen ebenfalls die Einstellung „Outlook-Sicherheitsmodus“ unter „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen, damit diese Einstellung angewendet wird.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Eingabeaufforderung für Outlook-Objektmodell beim Lesen von Adressinformationen konfigurieren

Betrifft: **Outlook**

Diese Einstellung steuert, was geschieht, wenn ein nicht vertrauenswürdiges Programm einen Zugriffsversuch auf ein Empfängerfeld unternimmt, z. B. das Feld **An:**, und dabei das Outlook-Objektmodell verwendet.

#### Sicherheitsrisiko

Wenn eine nicht vertrauenswürdige Anwendung auf Empfängerfelder zugreift, könnte die Anwendung damit Zugriff auf vertrauliche Daten erhalten und diese Daten möglicherweise ändern. Dies führt u. U. dazu, dass E-Mail an einen falschen Empfänger gesendet wird.

Wenn eine nicht vertrauenswürdige Anwendung einen Zugriffsversuch auf Empfängerfelder unternimmt, greift Outlook 2007 auf die im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters konfigurierte Einstellung zurück. Diese Einstellung legt fest, wann Outlook den Benutzern eine Warnung zu programmgesteuerten Zugriffsversuchen ausgibt:
* Nur, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird (die Standardeinstellung)
* Immer
* Niemals
 

Wenn ausgewählt ist, dass niemals Warnungen ausgegeben werden sollen, gewährt Outlook automatisch den programmgesteuerten Zugriff auf alle Programme, die diesen anfordern. Dadurch könnte ein schädliches Programm Zugriff auf vertrauliche Informationen erhalten.
Hinweis:

Bei der beschriebenen Standardfunktionalität wird vorausgesetzt, dass Sie nicht der Empfehlung gefolgt sind, die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ zu aktivieren, um sicherzustellen, dass Outlook-Sicherheitseinstellungen durch die Gruppenrichtlinie konfiguriert werden. Wenn Gruppenrichtlinien-Sicherheitseinstellungen für Outlook verwendet werden, wird der Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters nicht verwendet. In dieser Situation besteht die Standardeinstellung darin, den Benutzern eine Eingabeaufforderung auf Grundlage der Computersicherheit zu senden. Dies entspricht der Option „Nur wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird“ im Vertrauensstellungscenter, und hat keine Auswirkungen auf die Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus vier verschiedenen Optionen auswählen, wenn ein nicht vertrauenswürdiges Programm versucht, mithilfe des Outlook-Objektmodells auf ein Empfängerfeld zuzugreifen:
* **Eingabeaufforderung für Benutzer**. Der Benutzer wird aufgefordert, jeden Zugriffsversuch zu genehmigen.
* **Automatisch genehmigen**. Outlook erfüllt automatisch alle programmgesteuerten Zugriffsanforderungen aller Programme. Durch diese Option entsteht möglicherweise ein erhebliches Sicherheitsrisiko. Sie wird daher nicht empfohlen.
* **Automatisch ablehnen**. Outlook verweigert automatisch alle programmgesteuerten Zugriffsanforderungen von allen Programmen.

**Benutzer basierend auf der Computersicherheit auffordern**. Outlook sendet Benutzern nur eine Eingabeaufforderung, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird.

**Tabelle 1.69. Eingabeaufforderung für Outlook-Objektmodell beim Lesen von Adressinformationen konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Automatisch ablehnen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1273

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **Benutzer basierend auf der Computersicherheit auffordern** wird die Standardkonfiguration von Outlook 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.
Wichtig:

Sie müssen ebenfalls die Einstellung „Outlook-Sicherheitsmodus“ unter „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen, damit diese Einstellung angewendet wird.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Eingabeaufforderung für Outlook-Objektmodell beim Antworten auf Besprechungs- und Aufgabenanfragen

Betrifft: **Outlook**

Diese Einstellung steuert, was geschieht, wenn ein nicht vertrauenswürdiges Programm versucht, unter Verwendung der Response-Methode eines Tasks oder einer Besprechungsanfrage in Outlook 2007 programmgesteuert eine E-Mail zu senden.

#### Sicherheitsrisiko

Wenn eine nicht vertrauenswürdige Anwendung programmgesteuert auf Tasks bzw. Besprechungsanfragen antwortet, könnte die Anwendung sich als der Benutzer ausgeben und eine Benutzerantwort auf den Task oder die Besprechungsanfrage mit falschen Informationen senden.

Wenn eine nicht vertrauenswürdige Anwendung versucht, programmgesteuert auf Tasks oder Besprechungsanfragen zu antworten, greift Outlook 2007 auf die im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters konfigurierte Einstellung zurück. Diese Einstellung legt fest, wann Outlook den Benutzern eine Warnung zu programmgesteuerten Zugriffsversuchen ausgibt:
* Nur, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird (die Standardeinstellung)
* Immer
* Niemals

Wenn ausgewählt ist, dass niemals Warnungen ausgegeben werden sollen, gewährt Outlook automatisch den programmgesteuerten Zugriff auf alle Programme, die diesen anfordern. Dadurch könnte ein schädliches Programm Zugriff auf vertrauliche Informationen erhalten.
Hinweis:

Bei der beschriebenen Standardfunktionalität wird vorausgesetzt, dass Sie nicht der Empfehlung gefolgt sind, die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ zu aktivieren, um sicherzustellen, dass Outlook-Sicherheitseinstellungen durch die Gruppenrichtlinie konfiguriert werden. Wenn Gruppenrichtlinien-Sicherheitseinstellungen für Outlook verwendet werden, wird der Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters nicht verwendet. In dieser Situation besteht die Standardeinstellung darin, den Benutzern eine Eingabeaufforderung auf Grundlage der Computersicherheit zu senden. Dies entspricht der Option „Nur wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird“ im Vertrauensstellungscenter, und hat keine Auswirkungen auf die Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus vier verschiedenen Optionen auswählen, wenn ein nicht vertrauenswürdiges Programm versucht, mithilfe der Response-Methode eines Tasks oder einer Besprechungsanfrage programmgesteuert eine E-Mail zu senden:
* **Eingabeaufforderung für Benutzer**. Der Benutzer wird aufgefordert, jeden Zugriffsversuch zu genehmigen.
* **Automatisch genehmigen**. Outlook erfüllt automatisch alle programmgesteuerten Zugriffsanforderungen aller Programme. Durch diese Option entsteht möglicherweise ein erhebliches Sicherheitsrisiko. Sie wird daher nicht empfohlen.
* **Automatisch ablehnen**. Outlook verweigert automatisch alle programmgesteuerten Zugriffsanforderungen von allen Programmen.
* **Benutzer basierend auf der Computersicherheit auffordern**. Outlook sendet Benutzern nur eine Eingabeaufforderung, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird.

**Tabelle 1.70. Eingabeaufforderung für Outlook-Objektmodell beim Antworten auf Besprechungs- und Aufgabenanfragen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


Outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Automatisch ablehnen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1172

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **Benutzer basierend auf der Computersicherheit auffordern** wird die Standardkonfiguration von Outlook 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.
Hinweis:

Sie müssen ebenfalls die Einstellung „Outlook-Sicherheitsmodus“ unter „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen, damit diese Einstellung angewendet wird.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Eingabeaufforderung für Outlook-Objektmodell beim Senden von E-Mail konfigurieren

Betrifft: **Outlook**

Diese Einstellung steuert, was geschieht, wenn ein nicht vertrauenswürdiges Programm unter Verwendung des Outlook-Objektmodells versucht, programmgesteuert eine E-Mail zu senden.

#### Sicherheitsrisiko

Wenn eine nicht vertrauenswürdige Anwendung programmgesteuert eine E-Mail sendet, könnte die Anwendung böswilligen Code in der E-Mail senden, sich als ein Benutzer ausgeben oder einen Denial-of-Service-Angriff ausführen, indem eine große Menge an E-Mails an einen Benutzer oder eine Gruppe von Benutzern gesendet wird.

Wenn eine nicht vertrauenswürdige Anwendung versucht, programmgesteuert eine E-Mail zu senden, greift Outlook 2007 auf die im Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters konfigurierte Einstellung zurück. Diese Einstellung legt fest, wann Outlook den Benutzern eine Warnung zu programmgesteuerten Zugriffsversuchen ausgibt:
* Nur, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird (die Standardeinstellung)
* Immer
* Niemals

Wenn ausgewählt ist, dass niemals Warnungen ausgegeben werden sollen, gewährt Outlook automatisch den programmgesteuerten Zugriff auf alle Programme, die diesen anfordern. Dadurch könnte ein schädliches Programm Zugriff auf vertrauliche Informationen erhalten.
Hinweis:

Bei der beschriebenen Standardfunktionalität wird vorausgesetzt, dass Sie nicht der Empfehlung gefolgt sind, die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ zu aktivieren, um sicherzustellen, dass Outlook-Sicherheitseinstellungen durch die Gruppenrichtlinie konfiguriert werden. Wenn Gruppenrichtlinien-Sicherheitseinstellungen für Outlook verwendet werden, wird der Abschnitt „Programmgesteuerter Zugriff“ des Vertrauensstellungscenters nicht verwendet. In dieser Situation besteht die Standardeinstellung darin, den Benutzern eine Eingabeaufforderung auf Grundlage der Computersicherheit zu senden. Dies entspricht der Option „Nur wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird“ im Vertrauensstellungscenter, und hat keine Auswirkungen auf die Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus vier verschiedenen Optionen auswählen, wenn ein nicht vertrauenswürdiges Programm versucht, mithilfe des Outlook-Objektmodells programmgesteuert eine E-Mail zu senden:
* **Eingabeaufforderung für Benutzer**. Der Benutzer wird aufgefordert, jeden Zugriffsversuch zu genehmigen.
* **Automatisch genehmigen**. Outlook erfüllt automatisch alle programmgesteuerten Zugriffsanforderungen aller Programme. Durch diese Option entsteht möglicherweise ein erhebliches Sicherheitsrisiko. Sie wird daher nicht empfohlen.
* **Automatisch ablehnen**. Outlook verweigert automatisch alle programmgesteuerten Zugriffsanforderungen von allen Programmen.
* **Benutzer basierend auf der Computersicherheit auffordern**. Outlook sendet Benutzern nur eine Eingabeaufforderung, wenn die Antivirensoftware veraltet ist oder nicht ausgeführt wird.

**Tabelle 1.71. Eingabeaufforderung für Outlook-Objektmodell beim Senden von E-Mail konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Automatisch ablehnen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1590

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **Benutzer basierend auf der Computersicherheit auffordern** wird die Standardkonfiguration von Outlook 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.
Wichtig:

Wenn diese Einstellung aktiviert ist, müssen Sie ebenfalls die Einstellung „Outlook-Sicherheitsmodus“ unter „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Vertrauenswürdige Add-Ins konfigurieren

Betrifft: **Outlook**

Mithilfe dieser Einstellung kann eine Liste vertrauenswürdiger Add-Ins festgelegt werden, die ohne Einschränkung durch Outlook 2007-Sicherheitsmaßnahmen ausgeführt werden können.

#### Sicherheitsrisiko

Das Outlook-Objektmodell enthält Einstiegspunkte zum Zugriff auf Outlook-Daten, zum Speichern von Daten in angegebenen Speicherorten und zum Senden von E-Mail-Nachrichten, die alle von böswilligen Anwendungsentwicklern ausgenutzt werden könnten. Zum Schutz dieser Einstiegspunkte warnt der Objektmodellschutz (Object Model Guard) Benutzer und fordert sie zu einer Bestätigung auf, wenn nicht vertrauenswürdiger Code, einschließlich Add-Ins, mithilfe des Objektmodells versucht, E-Mail-Adressinformationen abzurufen, Daten außerhalb von Outlook zu speichern, bestimmte Aktionen auszuführen und E-Mail-Nachrichten zu senden.

Um bei der Verwendung von Add-Ins übermäßig häufige Sicherheitswarnungen zu vermeiden, können Administratoren eine Liste mit vertrauenswürdigen Add-Ins festlegen, die ohne Anzeige von Aufforderungen automatisch auf das Outlook-Objektmodell zugreifen können. Diese Liste vertrauenswürdiger Add-Ins sollte mit Vorsicht behandelt werden, da beim Hinzufügen eines schädlichen Add-Ins dieses Add-In auf die Liste zugreifen und vertrauliche Informationen weiterleiten kann.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, wird eine Liste vertrauenswürdiger Add-Ins und Hashes bereitgestellt, die Administratoren durch Hinzufügen und Entfernen von Einträgen ändern können. Standardmäßig ist diese Liste leer. Geben Sie zum Erstellen eines neuen Eintrags einen DLL-Dateinamen in der Spalte **Wertname** sowie das Hashergebnis in der Spalte **Wert** ein.

**Tabelle 1.72. Vertrauenswürdige Add-Ins konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Programmatische Sicherheit\Vertrauenswürdige Add-Ins

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


outlk12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Deaktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-786

</td>

</tr>

</table>

#### Auswirkung

Die Liste der vertrauenswürdigen Add-Ins ist standardmäßig leer und wird nicht verwendet. Die empfohlenen Einstellungen für EC- und SSLF-Umgebungen dürften daher nicht zu Nutzbarkeitsproblemen führen. Wenn Benutzer jedoch mit Add-Ins arbeiten, die auf das Outlook-Objektmodell zugreifen, werden diesen möglicherweise wiederholt Aufforderungen angezeigt, wenn der Administrator diese Einstellung nicht aktiviert und die Add-Ins der Liste hinzufügt.
Hinweis:

Sie können Exchange-Sicherheitsformulareinstellungen auch konfigurieren, indem Sie die Einstellung „Outlook-Sicherheitsmodus“ in „Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen.

Weitere Informationen zum Objektmodellschutz (Object Model Guard) finden Sie unter [Sicherheitsverhalten des Outlook-Objektmodells](http://go.microsoft.com/fwlink/?linkid=87941)   (möglicherweise in englischer Sprache) in der MSDN Outlook-Entwicklerreferenz.

### Verhalten der schrittweisen Aktualisierung von Windows SharePoint Services steuern

Betrifft: **InfoPath**

Diese Einstellung steuert, ob Formulare und Formularvorlagen während eines schrittweisen Updates den von Windows SharePoint® Services bereitgestellten URL-Umleitungen folgen.

#### Sicherheitsrisiko

Während eines schrittweisen Updates in Windows SharePoint Services bleiben aktualisierte Sites unter ihren ursprünglichen URLs verfügbar (zum Beispiel http://&lt;Unternehmensname&gt;/Sites/SiteA), während Sites, die noch aktualisiert werden, unter einer temporären Domänen-URL gespeichert werden (zum Beispiel http://&lt;Unternehmensname_alt&gt;/Sites/SiteB).

Standardmäßig leitet InfoPath 2007 Benutzeranforderungen für Sites, die noch nicht aktualisiert wurden, automatisch an die temporäre URL weiter, wenn diese sich im lokalen Intranet befindet, blockiert die Anforderung aber, wenn sich die URL an einem anderen Speicherort befindet. InfoPath fordert vor dem Umleiten von Formularen oder Formularvorlagen an andere Intranetsites Benutzer zur Bestätigung auf.

Wenn diese Einschränkung aufgehoben wird, werden alle Anforderungen an noch nicht aktualisierte Sites unabhängig vom Speicherort an ihre Ziele umgeleitet. Diese Funktionalität bewirkt möglicherweise, dass Anforderungen für eine sichere Site an eine unsichere Site umgeleitet werden (Anforderungen an eine Intranetsite könnten beispielsweise an eine nicht verschlüsselte Internetsite umgeleitet werden), was die Sicherheit vertraulicher Informationen gefährden kann.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei verschiedenen Umleitungsoptionen auswählen:
* **URL-Umleitungen an Internet- und Intranetspeicherorte zulassen**. Bei Auswahl dieser Optionen könnte die Sicherheit vertraulicher Informationen aufgrund schlecht geplanter schrittweiser Upgrades möglicherweise gefährdet werden.
* **URL-Umleitungen an Intranetspeicherorte zulassen**. Diese Option ist die Standardkonfiguration in InfoPath 2007. Umleitungen an das lokale Intranet werden zugelassen, Umleitungen an andere Speicherorte werden blockiert.
* **Alle URL-Umleitungen blockieren**. Durch diese Option wird verhindert, dass InfoPath Umleitungen verwendet.

**Tabelle 1.73. Verhalten der schrittweisen Aktualisierung von Windows SharePoint Services steuern**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


inf12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (URL-Umleitungen an Intranetspeicherorte zulassen)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Alle URL-Umleitungen blockieren)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-704

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Auswahl von **URL-Umleitungen an Intranetspeicherorte zulassen** wird die Standardkonfiguration in InfoPath 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden. Wenn der Administrator jedoch alle Umleitungen blockiert, können Benutzer während eines schrittweisen Upgrades nicht auf Sites zugreifen.

### Steuern des Verhaltens beim Öffnen von Formularen in der Sicherheitszone „Internet“

Betrifft: **InfoPath**

Mithilfe dieser Richtlinie können Sie festlegen, ob InfoPath 2007 ein Formular aus dem Internet öffnet, wenn die Speicherortinformationen des Formulars und des lokal zwischengespeicherten Formulars nicht übereinstimmen.

#### Sicherheitsrisiko

Wenn InfoPath-Lösungen lokal geöffnet werden, wird der Speicherort des Formulars überprüft, damit Updates für das Formular heruntergeladen werden können. Wenn ein Benutzer ein Formular aus einem Speicherort im Internet lokal speichert und dann dasselbe Formular aus einem anderen Speicherort im Internet öffnet, wird der Zwischenspeicher mit den neuen Speicherortinformationen aktualisiert. Wenn der Benutzer dann das erste Formular von seinem Speicherort aus öffnet, stimmen das lokal gespeicherte Formular und das lokal zwischengespeicherte Formular nicht überein. Diese Situation tritt normalerweise ein, wenn Entwickler Formulare an einen neuen Speicherort verschieben. Wenn aber beim Verwenden des zwischengespeicherten Orts keine Warnung ausgegeben wird, könnte dies von einem Angreifer ausgenutzt werden, der Formulare an einen neuen Speicherort umleiten könnte. Bei diesem Angriffstyp handelt es sich um eine Form vom Signal übertragendem Angriff.

Wenn die Speicherortinformationen des zwischengespeicherten Formulars nicht mit denen des gespeicherten Formulars übereinstimmen, kann das Formular standardmäßig nicht geöffnet werden, ohne dass der Benutzer zur Bestätigung aufgefordert wird.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei verschiedenen Optionen auswählen, die gelten, wenn InfoPath 2007-Benutzer versuchen, Formulare mit unterschiedlichen Speicherortinformationen zu öffnen.
* **Zulassen**. Das Formular wird ohne Bestätigungsaufforderung an den Benutzer geöffnet.
* **Eingabeaufforderung**. Benutzer erhalten eine Bestätigungsaufforderung und müssen entscheiden, ob sie das Dokument öffnen.
* **Blockieren**. Benutzer erhalten eine Bestätigungsaufforderung, bevor sie entscheiden, ob sie das Formular öffnen (diese Funktionalität entspricht der Option „Eingabeaufforderung“).

**Tabelle 1.74. Steuern des Verhaltens beim Öffnen von Formularen in der Sicherheitszone „Internet“**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit

</td>

</tr>

<td>


**ADM-Datei**

</td>

<td>


inf12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Blockieren)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Blockieren)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1479

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Klicken auf **Blockieren** wird die Standardkonfiguration in InfoPath 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.

### Steuern des Verhaltens beim Öffnen von Formularen in der Sicherheitszone „Intranet“

Betrifft: **InfoPath**

Mithilfe dieser Richtlinie können Sie festlegen, ob InfoPath 2007 ein Formular aus dem lokalen Intranet öffnet, wenn die Speicherortinformationen des Formulars und des lokal zwischengespeicherten Formulars nicht übereinstimmen.

#### Sicherheitsrisiko

Wenn InfoPath-Lösungen lokal geöffnet werden, wird der Speicherort des Formulars überprüft, damit Updates für das Formular heruntergeladen werden können. Wenn ein Benutzer ein Formular aus einem Speicherort im Intranet lokal speichert und dann dasselbe Formular aus einem anderen Speicherort im lokalen Intranet öffnet, wird der Zwischenspeicher mit den neuen Speicherortinformationen aktualisiert. Wenn der Benutzer dann das erste Formular von seinem Speicherort aus öffnet, stimmen das lokal gespeicherte Formular und das lokal zwischengespeicherte Formular nicht überein. Diese Situation tritt normalerweise ein, wenn Entwickler Formulare an einen neuen Speicherort verschieben. Wenn aber beim Verwenden des zwischengespeicherten Orts keine Warnung ausgegeben wird, könnte dies von einem Angreifer ausgenutzt werden, der Formulare an einen neuen Speicherort umleiten könnte. Bei diesem Angriffstyp handelt es sich um eine Form vom Signal übertragendem Angriff.

Wenn die Speicherortinformationen des zwischengespeicherten Formulars nicht mit denen des gespeicherten Formulars übereinstimmen, kann das Formular standardmäßig nicht geöffnet werden, ohne dass der Benutzer zur Bestätigung aufgefordert wird.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei verschiedenen Optionen auswählen, die gelten, wenn InfoPath 2007-Benutzer versuchen, Formulare mit unterschiedlichen Speicherortinformationen zu öffnen.
* **Zulassen**. Das Formular wird ohne Bestätigungsaufforderung an den Benutzer geöffnet.
* **Eingabeaufforderung**. Benutzer erhalten eine Bestätigungsaufforderung und müssen entscheiden, ob sie das Dokument öffnen.
* **Blockieren**. Benutzer erhalten eine Bestätigungsaufforderung, bevor sie entscheiden, ob sie das Formular öffnen (diese Funktionalität entspricht der Option „Eingabeaufforderung“).

**Tabelle 1.74. Steuern des Verhaltens beim Öffnen von Formularen in der Sicherheitszone „Intranet“**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


inf12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Blockieren)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Blockieren)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1360

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Klicken auf **Blockieren** wird die Standardkonfiguration in InfoPath 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.

### Steuern des Verhaltens beim Öffnen von Formularen in der Sicherheitszone „Vertrauenswürdige Sites“

Betrifft: **InfoPath**

Mithilfe dieser Richtlinie können Sie festlegen, ob InfoPath 2007 ein Formular aus der Sicherheitszone für vertrauenswürdige Sites öffnet, wenn die Speicherortinformationen des Formulars und des lokal zwischengespeicherten Formulars nicht übereinstimmen.

#### Sicherheitsrisiko

Wenn InfoPath-Lösungen lokal geöffnet werden, wird der Speicherort des Formulars überprüft, damit Updates für das Formular heruntergeladen werden können. Wenn ein Benutzer ein Formular aus einem Speicherort in der Zone der vertrauenswürdigen Sites lokal speichert und dann dasselbe Formular aus einem anderen Speicherort in der Zone der vertrauenswürdigen Sites öffnet, wird der Zwischenspeicher mit den neuen Speicherortinformationen aktualisiert. Wenn der Benutzer dann das erste Formular von seinem Speicherort aus öffnet, stimmen das lokal gespeicherte Formular und das lokal zwischengespeicherte Formular nicht überein. Diese Situation tritt normalerweise ein, wenn Entwickler Formulare an einen neuen Speicherort verschieben. Wenn aber beim Verwenden des zwischengespeicherten Orts keine Warnung ausgegeben wird, könnte dies von einem Angreifer ausgenutzt werden, der Formulare an einen neuen Speicherort umleiten könnte. Bei diesem Angriffstyp handelt es sich um eine Form vom Signal übertragendem Angriff.

Wenn die Speicherortinformationen des zwischengespeicherten Formulars nicht mit denen des gespeicherten Formulars übereinstimmen, kann das Formular standardmäßig nicht geöffnet werden, ohne dass der Benutzer zur Bestätigung aufgefordert wird.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei verschiedenen Optionen auswählen, die gelten, wenn InfoPath 2007-Benutzer versuchen, Formulare mit unterschiedlichen Speicherortinformationen zu öffnen.
* **Zulassen**. Das Formular wird ohne Bestätigungsaufforderung an den Benutzer geöffnet.
* **Eingabeaufforderung**. Benutzer erhalten eine Bestätigungsaufforderung und müssen entscheiden, ob sie das Dokument öffnen.
* **Blockieren**. Benutzer erhalten eine Bestätigungsaufforderung, bevor sie entscheiden, ob sie das Formular öffnen (diese Funktionalität entspricht der Option „Eingabeaufforderung“).

**Tabelle 1.74. Steuern des Verhaltens beim Öffnen von Formularen in der Sicherheitszone „Vertrauenswürdige Sites“**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


inf12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Blockieren)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Blockieren)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-893

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung und Klicken auf **Blockieren** wird die Standardkonfiguration in InfoPath 2007 erzwungen. Daher sollten für die meisten Benutzer keine Nutzbarkeitsprobleme verursacht werden.

### Steuern des Verhaltens beim Öffnen von InfoPath-E-Mail-Formularen, die Code oder Skript enthalten

Betrifft: **InfoPath**

Diese Einstellung steuert, wie InfoPath 2007 E-Mails behandelt, die Code oder Skript enthalten.

#### Sicherheitsrisiko

InfoPath 2007 sendet Benutzern vor dem Öffnen von InfoPath-E-Mail-Formularen, die Code oder Skript enthalten, standardmäßig Benachrichtigungen und Eingabeaufforderungen. Wenn diese Einschränkung aufgehoben wird, öffnet InfoPath E-Mail-Formulare, die Code oder Skript enthalten, ohne eine Eingabeaufforderung an die Benutzer, wodurch auf den Computern der Benutzer schädlicher Code ausgeführt werden könnte.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei verschiedenen Optionen für Eingabeaufforderungen an die Benutzer auswählen:
* **Nie ausführen**. InfoPath öffnet keine E-Mail-Formulare, die Code oder Skript enthalten.
* **Bestätigung vor dem Ausführen**. Wenn Benutzer versuchen, E-Mail-Formulare zu öffnen, die Code oder Skript enthalten, zeigt InfoPath eine Benachrichtigung an und ermöglicht den Benutzern die Auswahl, ob das Formular geöffnet werden soll. Diese Option ist die Standardkonfiguration.
* **Ausführen ohne Bestätigung**. InfoPath öffnet alle E-Mail-Formulare, die Code oder Skript enthalten, ohne eine Eingabeaufforderung an den Benutzer zu senden. Diese Option könnte möglicherweise dazu führen, dass schädlicher Code auf dem Computer des Benutzers ausgeführt wird.

**Tabelle 1.77. Steuern des Verhaltens beim Öffnen von InfoPath-E-Mail-Formularen, die Code oder Skript enthalten**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


inf12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Bestätigung vor dem Ausführen)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Nie ausführen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1315

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für die SSLF-Umgebung ist **Nie ausführen**, wodurch jegliches Ausführen von Code in InfoPath-E-Mail-Formularen verhindert wird. Berücksichtigen Sie vor der Auswahl dieser Konfiguration die Verwendung solcher Formulare in Ihrem Unternehmen.

### Steuerelementbloggen

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Benutzer Blogeinträge mit Word 2007 verfassen und veröffentlichen können.

#### Sicherheitsrisiko

Die Bloggingfunktion in Word 2007 ermöglicht Benutzern das Verfassen von Blogeinträgen und ein direktes Veröffentlichen von Word aus, ohne Verwendung zusätzlicher Software.

Standardmäßig können Benutzer Blogeinträge an alle kompatiblen Blogdienstanbieter veröffentlichen, z. B. Windows Live Spaces, Blogger, SharePoint- oder Communityserver-Sites und andere. Wenn es in Ihrem Unternehmen Richtlinien zum Veröffentlichen von Blogeinträgen gibt, führt ein Zulassen der Bloggingfunktion in Word 2007 möglicherweise dazu, dass Benutzer diese Richtlinien verletzen.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei verschiedenen Blogging-Steuerungsoptionen auswählen:
* **Aktiviert**. Benutzer können Blogeinträge verfassen und von Word 2007 bei einem beliebigen verfügbaren Blogdienstanbieter veröffentlichen. Diese Option ist die Standardkonfiguration in Word 2007.
* **Nur SharePoint-Bloggen**. Benutzer können Blogeinträge nur auf SharePoint-Sites veröffentlichen.
* **Deaktiviert**. Die Bloggingfunktion in Word ist ganz deaktiviert.

**Tabelle 1.78. Steuerelementbloggen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Verschiedenes

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


office12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Bloggen vollständig deaktiviert)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1241

</td>

</tr>

</table>

#### Auswirkung

Durch die empfohlene SSLF-Konfiguration wird die Bloggingfunktion in Word 2007 deaktiviert, was zu Beeinträchtigungen für Benutzer führen kann, die Word zum Verfassen und Veröffentlichen von Blogeinträgen verwenden. Benutzer, die einen legitimen Grund für das Veröffentlichen von Blogeinträgen haben, müssen ein anderes Tool verwenden.

### Benutzerdefinierter Code

Betrifft: **InfoPath**

Diese Einstellung steuert, ob Benutzer InfoPath 2007-Formulare entwerfen können, die benutzerdefinierten Code verwenden.

#### Sicherheitsrisiko

Standardmäßig können Benutzer neue InfoPath 2007-Formulare entwerfen, die benutzerdefinierten Code verwenden, um Formularen Interaktivität und andere Funktionen hinzuzufügen. Entwickler können in C# und Visual Basic .NET verfassten verwalteten Code sowie in Jscript und VBScript verfasste Skripts hinzufügen.

Ein unerfahrener oder böswilliger Benutzer könnte ein Formular mit schädlichem Code entwerfen, das die Computer von Benutzern beschädigt oder vertrauliche Daten gefährdet.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer Formularvorlagen keinen verwalteten Code und keine Skripts hinzufügen.

**Tabelle 1.79. Benutzerdefinierter Code**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Eingeschränkte Features

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


inf12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1564

</td>

</tr>

</table>

#### Auswirkung

Das Aktivieren dieser Einstellung könnte bei Designern von InfoPath 2007-Formularen zu Problemen führen, da kein benutzerdefinierter Code in Formularen verwenden werden kann. Eventuell sollten Sie durch eine Umfrage in Ihrem Unternehmen ermitteln, ob sich aus dieser Einstellung Beeinträchtigungen für Formulardesigner ergeben.
  
In diesem Beitrag
* [Überblick](http://wwwppe/germany/technet/security/guidance/clientsecurity/2007office/tandc/default.mspx)
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1](http://wwwppe/germany/technet/security/guidance/clientsecurity/2007office/tandc/098bfa81-7deb-4e48-95bb-b95c9c101831.mspx)
* Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3](http://wwwppe/germany/technet/security/guidance/clientsecurity/2007office/tandc/e7b89b01-fe2c-4f83-83c7-728b051c2460.mspx)
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4](http://wwwppe/germany/technet/security/guidance/clientsecurity/2007office/tandc/e45554ae-6a26-4ee5-aa2d-a6e8154520c3.mspx)
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5](http://wwwppe/germany/technet/security/guidance/clientsecurity/2007office/tandc/e8fadc8a-6e74-4f2d-bbf3-4671655239f0.mspx)
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6](http://wwwppe/germany/technet/security/guidance/clientsecurity/2007office/tandc/a1e4da59-0887-4ec3-bd6d-79b88d296a63.mspx)
* [Sicherheitseinstellungen für Computerrichtlinien](http://wwwppe/germany/technet/security/guidance/clientsecurity/2007office/tandc/b4cb1f63-0e94-4404-abe7-3891a5f482e5.mspx)
 
Download
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)Update-Benachrichtigungen
[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)Feedback
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007 microsoft office-sicherheitshandbuch, bedrohungen und gegenmaßnahmen: sicherheitseinstellungen in 2007 office system)  
 

<table>

<tr>

<td>

[Zum Seitenanfanq](#mainsection)  

</td>

<td>

[](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10)"><img AltText="Dd443674.pageLeft(de-de,TechNet.10).gif)  3 von 8[](https://technet.microsoft.com/de-de/library/f3af8a5d-5067-4add-917b-f7ab8cdca16c(v=TechNet.10)"><img AltText="Dd443674.pageRight(de-de,TechNet.10).gif)  
</td>

</tr>

</table>




