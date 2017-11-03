---
TOCTitle: 'RMS – Häufig gestellte Fragen: Vorlagen für Benutzerrechterichtlinien'
Title: 'RMS – Häufig gestellte Fragen: Vorlagen für Benutzerrechterichtlinien'
ms:assetid: '01515f08-9844-4c1a-9ab5-a5a60a901b50'
ms:contentKeyID: 18118744
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720175(v=WS.10)'
---

RMS – Häufig gestellte Fragen: Vorlagen für Benutzerrechterichtlinien
=====================================================================

RMS-Vorlagen – Häufig gestellte Fragen
--------------------------------------

-   [Kann ich eine RMS-Standardvorlage für alle innerhalb einer Organisation erstellten Inhalte erzwingen, sodass ein Unternehmen das Vorhandensein bestimmter Mindestrechte sicherstellen kann?](#bkmk_57)
-   [Wo sind die RMS-Vorlagen für Benutzerrechterichtlinien gespeichert?](#bkmk_58)
-   [Beim Erstellen von Vorlagen werden Benutzeraliase und Verteilerlisten (Distribution Lists oder DLs) mit ihnen verknüpft. Wie kann eine Organisation mit mehreren Abteilungen Vorlagen mit denselben Basisrechten zur Verfügung stellen, diese Rechte aber je nach Inhalt unterschiedlichen Gruppen gewähren?](#bkmk_59)
-   [Sind die einem Dokument zugeordneten Rechte statisch? Wenn eine Datei gesendet wurde, ist es möglich, die Rechte später noch zu ändern, auch wenn die Veröffentlichungslizenz in die Datei eingebettet ist und sich nicht auf dem RMS-Richtlinienserver befindet?](#bkmk_60)

<span id="BKMK_57"></span>
#### Kann ich eine RMS-Standardvorlage für alle innerhalb einer Organisation erstellten Inhalte erzwingen, sodass ein Unternehmen das Vorhandensein bestimmter Mindestrechte sicherstellen kann?

Ja. Mit dem RMS-SDK (Software Development Kit) kann eine Anwendung entwickelt werden, mit der die jeweils erforderlichen Vorlagen erzwungen werden können. Das Erzwingen von Vorlagen für Inhalte wird von der IRM-Implementierung (Information Rights Management, Verwaltung von Informationsrechten) in Office 2003 und später jedoch nicht unterstützt.

<span id="BKMK_58"></span>
#### Wo sind die RMS-Vorlagen für Benutzerrechterichtlinien gespeichert?

Der Speicherort der Vorlagen wird von der RMS-fähigen Anwendung bestimmt. Bei Office 2003 und später erfolgt die Festlegung des Speicherorts als Benutzereinstellung in der Registrierung an folgender Position:

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\11.0\\Common\\DRM\\AdminTemplatePath**

\- oder -

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\12.0\\Common\\DRM\\AdminTemplatePath** bei Microsoft Office 2007.

> [!NOTE]
> Wenn dieser Eintrag auf einen lokalen Ordner auf dem Client verweist, müssen die Vorlagendateien auf den Client kopiert werden. Wenn er hingegen auf eine Netzwerkfreigabe verweist, ist der Speicherort nicht verfügbar, solange der Benutzer offline ist. 

<span id="BKMK_59"></span>
#### Beim Erstellen von Vorlagen werden Benutzeraliase und Verteilerlisten (Distribution Lists oder DLs) mit ihnen verknüpft. Wie kann eine Organisation mit mehreren Abteilungen Vorlagen mit denselben Basisrechten zur Verfügung stellen, diese Rechte aber je nach Inhalt unterschiedlichen Gruppen gewähren?

Es gibt zwei Lösungen für diese Situation:

-   Erstellen Sie eine Vorlage, beispielsweise mit dem Namen „Nur für den internen Gebrauch“, die für alle Angestellten in der Unternehmenseinheit lizenziert ist. Verwenden Sie diese Vorlage dann für E-Mails, die an bestimmte Personen adressiert sind. Der Vorteil ist, dass für jede Unternehmenseinheit nur eine Vorlage für E-Mails benötigt wird und diese auf die Benutzer beschränkt werden kann, an die Sie die Vorlage senden. Der Nachteil ist, dass auch jeder außerhalb der ursprünglichen Empfängergruppe die E-Mail dennoch lesen kann.
-   Als Alternative dazu können Sie mehrere Vorlagen erstellen, einschließlich einer für jede Verteilerliste. Dies ermöglicht eine weitaus präzisere Steuerung, bedeutet aber auch, dass die IT-Abteilung mehrere Vorlagen unterstützen muss.

<span id="BKMK_60"></span>
#### Sind die einem Dokument zugeordneten Rechte statisch? Wenn eine Datei gesendet wurde, ist es möglich, die Rechte später noch zu ändern, auch wenn die Veröffentlichungslizenz in die Datei eingebettet ist und sich nicht auf dem RMS-Richtlinienserver befindet?

Ja, dies ist bei Verwendung einer RMS-Vorlage für Benutzerrechterichtlinien möglich: Wenn Inhalt mithilfe einer RMS-Vorlage für Benutzerrechterichtlinien veröffentlicht wird, bleibt die Definition der Richtlinien auf dem Server und kann von einem Administrator geändert werden, nachdem der Inhalt veröffentlicht wurde. Wenn ein Benutzer eine Lizenz für den Inhalt anfordert, werden die in der Lizenz gewährten Rechte gemäß den aktuell auf dem Server definierten Richtlinien erteilt. Wenn die Rechte nach dem Ausstellen einer Nutzungslizenz für einen Benutzer geändert werden, bleiben dem Benutzer die Rechte erhalten, die zum Zeitpunkt der Lizenzausstellung gültig waren. Wenn Sie die Möglichkeit haben möchten, eine neue Vorlage für Benutzerrechterichtlinien anzuwenden, nachdem der Inhalt veröffentlicht wurde, aktivieren Sie eine Ablaufrichtlinie für die Vorlage, und geben Sie dann folgende Option an: **Nutzungslizenzen für Inhalte müssen erneuert werden alle: n Tage**. Geben Sie für n die Anzahl der Tage an, nach deren Ablauf ein Benutzer eine neue Nutzungslizenz anfordern muss.