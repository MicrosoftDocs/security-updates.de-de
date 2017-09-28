---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch:Kapitel 5: Entwerfen und Implementieren von Sicherhe'
Title: '2007 Microsoft Office-Sicherheitshandbuch:Kapitel 5: Entwerfen und Implementieren von Sicherhe'
ms:assetid: '6de5a362-72f8-4937-84ef-54ec91e040e6'
ms:contentKeyID: 20075605
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443661(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch
=========================================

### Kapitel 5: Entwerfen und Implementieren von Sicherheitseinstellungen

Veröffentlicht: 11. Nov 2007

In diesem Kapitel erhalten Sie Informationen zum Planen der Bereitstellung von Sicherheitseinstellungen für sechs 2007 Microsoft® Office-Programme in zwei unterschiedlichen Umgebungen: einer Unternehmensclient-Umgebung (Enterprise Client, EC) und einer Hochsicherheitsumgebung (Specialized Security - Limited Functionality, SSLF). Für eine erfolgreiche Bereitstellung sollten Sie alle Abschnitte dieses Kapitels durchlesen. In jedem Abschnitt wird ein wichtiger Schritt des Planungsprozesses behandelt. Wenn Sie einen Abschnitt überspringen, könnte die Bereitstellung fehlerhaft sein und eine unsichere Umgebung zur Folge haben.

In der folgenden Abbildung ist der gesamte Planungsprozess für die Bereitstellung dargestellt.

![](images/Dd443661.4fee92d9-5b6f-4e51-b8ac-148ea0ec636d(de-de,TechNet.10).gif)

**Abbildung 5.1. Planen der Bereitstellung von Sicherheitseinstellungen für die 2007 Office-Version**

##### Auf dieser Seite

[](#edaa)[Auswählen der Sicherheitseinstellungen für Ihre Umgebung](#edaa)
[](#ecaa)[Entwerfen einer Gruppenrichtlinieninfrastruktur](#ecaa)
[](#ebaa)[Vorbereiten der Bereitstellung von EC- oder SSLF-Einstellungen](#ebaa)

#### Auswählen der Sicherheitseinstellungen für Ihre Umgebung

Sie können in der 2007 Office-Version zwar Sicherheitseinstellungen für eine Vielzahl von Umgebungen konfigurieren, dieses Handbuch stellt jedoch Informationen für zwei spezifische Umgebungen bereit: eine EC-Umgebung und eine SSLF-Umgebung. In diesem Abschnitt erhalten Sie Anweisungen und Informationen, die Ihnen helfen sollen, die geeignete Sicherheitsumgebung für Ihr Unternehmen auszuwählen.

### Die EC-Umgebung

Die EC-Umgebung steht für Unternehmen mit typischen Sicherheitsanforderungen. Sie eignet sich für mittlere und große Unternehmen, die ein ausgewogenes Verhältnis von Sicherheit und Funktionalität wünschen.

Bei der EC-Umgebung wird vorausgesetzt, dass die Clientcomputer zu einer Active Directory® Domain Services (AD DS)-Umgebung gehören und dass sie nur mit anderen Computern kommunizieren, auf denen eines der folgenden Betriebssysteme ausgeführt wird:

-   Windows Server® 2003 mit Service Pack 1 (SP1) oder höher
-   Windows Vista® in einer AD DS-Umgebung
-   Windows® XP in einer AD DS-Umgebung

Weiterhin wird angenommen, dass die betrieblichen Ziele des Unternehmens eine ausgewogene Sicherheitsstrategie erfordern: Die Mitarbeiterproduktivität ist genauso wichtig wie die Sicherheit der Desktopumgebung. Um eine solche ausgewogene Sicherheitsstrategie zu ermöglichen, werden beim Implementieren von EC-Sicherheitseinstellungen die meisten Produktivitätsfunktionen und -technologien der 2007 Office-Version aktiviert. Diese Funktionen und Technologien weisen jedoch aufgrund bestimmter Sicherheitseinschränkungen nicht unbedingt sämtliche Funktionalität auf.

### Die SSLF-Umgebung

Die SSLF-Umgebung steht für weniger typische Unternehmen, bei denen Sicherheit von höchster Bedeutung ist. Sie eignet sich nur für mittelgroße und große Unternehmen mit äußerst strengen Sicherheitsstandards, bei denen Sicherheit einen höheren Stellenwert einnimmt als Anwendungsfunktionalität. SSLF-Einstellungen können in einem größeren Unternehmen auch auf eine bestimmte Untergruppe von Computern angewendet werden, beispielsweise in einer Abteilung, in der besonders vertrauliche Daten bearbeitet werden. Wie bei der EC-Umgebung wird auch in der SSLF-Umgebung vorausgesetzt, dass sich die Clientcomputer in einer AD DS-Umgebung befinden und nur mit Computern kommunizieren, auf denen eines der folgenden Betriebssysteme ausgeführt wird:

-   Windows Server 2003 mit Service Pack 1 (SP1) oder höher in einer AD DS-Umgebung
-   Windows Vista in einer AD DS-Umgebung
-   Windows XP in einer AD DS-Umgebung

Weiterhin wird bei der SSLF-Umgebung angenommen, dass die betrieblichen Ziele des Unternehmens eine erweiterte Sicherheitsstrategie erfordern: Die Mitarbeiterproduktivität ist nicht so wichtig wie die Sicherheit der Desktopumgebung. Zur Vereinfachung dieser Sicherheitsstrategie sind beim Implementieren von SSLF-Sicherheitseinstellungen viele Produktivitätsfunktionen und -technologien der 2007 Office-Version deaktiviert oder arbeiten mit reduzierter Funktionalität.

Die folgende Abbildung zeigt das relative Verhältnis von Sicherheit, Risiko und Funktionalität für EC-Sicherheitseinstellungen, SSLF-Einstellungen und die Standardsicherheitskonfiguration der 2007 Office-Version.

![](images/Dd443661.0c0264cd-34d5-44c9-9d21-b19a5ad12066(de-de,TechNet.10).gif)

**Abbildung 5.2. Vergleich von Risiko, Sicherheit und Produktivität für EC- und SSLF-Einstellungen**

[](#mainsection)[Zum Seitenanfanq](#mainsection)

#### Entwerfen einer Gruppenrichtlinieninfrastruktur

Wenn Sie Sicherheitseinstellungen für EC- bzw. SSLF-Umgebungen bereitstellen möchten, müssen Sie zunächst eine Gruppenrichtlinieninfrastruktur planen und entwerfen. Zu diesem Zweck müssen Sie die Struktur Ihrer Organisationseinheiten (Organizational Units, OUs) und anschließend die Struktur der Gruppenrichtlinienobjekte (Group Policy Objects, GPOs) entwerfen.

### Entwurf von Organisationseinheiten für Sicherheitsrichtlinien

Eine Organisationseinheit ist ein Container innerhalb einer Active Directory-Domäne. Organisationseinheiten können Benutzer, Gruppen, Computer und andere Organisationseinheiten enthalten. Wenn eine Organisationseinheit andere Organisationseinheiten beinhaltet, handelt es sich um eine übergeordnete Organisationseinheit. Eine Organisationseinheit innerhalb einer übergeordneten Organisationseinheit wird als untergeordnete Organisationseinheit bezeichnet.

Ein GPO ist ein Active Directory-Objekt, das Gruppenrichtlinieneinstellungen und andere Eigenschaften enthält. Sie können ein Gruppenrichtlinienobjekt mit einer Organisationseinheit verknüpfen. Hierdurch werden die Einstellungen des Gruppenrichtlinienobjekts auf die Benutzer und Gruppen in dieser Organisationseinheit sowie in ihren untergeordneten Organisationseinheiten angewendet. Für Verwaltungszwecke können Sie Administratorrechte an die einzelnen Organisationseinheiten delegieren.

Organisationseinheiten bieten eine einfache und effektive Möglichkeit, Benutzer und Computer zu gruppieren und so Verwaltungsgrenzen einzurichten. Mithilfe des Assistenten zum Erstellen neuer Delegierungen, der Bestandteil des Snap-Ins „Active Directory-Benutzer und -Computer“ der Microsoft Management Console (MMC) ist, kann die Steuerung einer Gruppe oder einzelner Organisationseinheiten delegiert werden.

### Empfohlener Entwurf für Organisationseinheiten

Eines der Hauptziele des Entwurfs von Organisationseinheiten in jeder Umgebung ist es, eine Grundlage für die durchgängige Implementierung von Gruppenrichtlinien zu schaffen, die für alle Clientcomputer in Active Directory gelten. Dadurch wird gewährleistet, dass alle diese Computer den Sicherheitsstandards des Unternehmens entsprechen. Der Organisationseinheitsentwurf muss außerdem eine geeignete Struktur für die verschiedenen Sicherheitseinstellungen für bestimmte Typen von Benutzern in einem Unternehmen bereitstellen. Entwickler benötigen beispielsweise eine andere Art von Zugriff auf ihre Computer als normale Benutzer. Die folgende Abbildung enthält ein Beispiel einer einfachen Organisationseinheitsstruktur, das für die Erläuterung von Gruppenrichtlinien in diesem Kapitel ausreichend ist. Die Organisationseinheitsstruktur für Ihre Unternehmensumgebung wird sich von dieser Struktur unterscheiden.

![](images/Dd443661.3bcd76c9-e12b-47d3-af74-aaadf03791fe(de-de,TechNet.10).gif)

**Abbildung 5.3. Beispiel für eine Organisationseinheitsstruktur**

Diese Organisationseinheitsstruktur enthält die folgenden Organisationseinheiten:

-   **Abteilung.** Da es innerhalb eines Unternehmens oft unterschiedliche Sicherheitsanforderungen gibt, ist es sinnvoll, in der Umgebung Organisationseinheiten für Abteilungen zu erstellen. Mithilfe eines solchen Ansatzes können Sie Sicherheitseinstellungen über ein Gruppenrichtlinienobjekt auf Computer und Benutzer in den jeweiligen Abteilungsorganisationseinheiten anwenden.
-   **Domänencontroller.** Enthält die Computerkonten für Computer, die als Domänencontroller fungieren.
-   **Windows Vista-Benutzer.** Enthält die Benutzerkonten für Benutzer, die sich bei Windows Vista-Computern anmelden.
-   **Windows Vista-Computer.** Enthält die Computerkonten für Computer, auf denen Windows Vista ausgeführt wird.
-   **Windows XP-Benutzer.** Enthält die Benutzerkonten für Benutzer, die sich bei Windows XP-Computern anmelden.
-   **Windows XP-Computer.** Enthält die Computerkonten für Computer, auf denen Windows XP ausgeführt wird.

### Entwurf von GPOs für Sicherheitsrichtlinien

GPOs werden auf Domänenebene gespeichert. Die Einstellungen innerhalb eines GPOs können also auf Benutzer und Computer angewendet werden, die sich in Standorten, Domänen und Organisationseinheiten befinden. Durch Verwendung von domänenbasierten GPOs (und Gruppenrichtlinieneinstellungen) anstelle eines manuellen oder skriptbasierten Konfigurationsprozesses können Sicherheitseinstellungen auf effiziente Weise für eine Vielzahl von Computern und Benutzern verwaltet und aktualisiert werden. Eine manuelle oder skriptbasierte Konfiguration ist ineffizient, da entweder ein von einem Techniker geschriebenes Skript erforderlich ist oder jeder Clientcomputer einzeln von einem Techniker konfiguriert werden muss. Eine solche Konfiguration ist darüber hinaus möglicherweise ineffektiv und nicht durchsetzbar, da lokal konfigurierte Einstellungen durch Benutzer, Administratoren und Skripts geändert werden können.

Wenn Sie Gruppenrichtlinieneinstellungen über domänenbasierte GPOs konfigurieren, haben die Gruppenrichtlinieneinstellungen Vorrang vor allen lokalen Einstellungen und können nicht lokal durch Benutzer oder Skripts geändert werden. In der folgenden Abbildung wird die Rangfolge angezeigt, nach der GPOs auf einen Computer angewendet werden. In diesem Beispiel ist der Computer Mitglied der untergeordneten Organisationseinheit. Gruppenrichtlinien werden zuerst aus der lokalen Sicherheitsrichtlinie der jeweiligen Clientcomputer angewendet. Nach dem Anwenden der lokalen Sicherheitsrichtlinie werden Gruppenrichtlinienobjekte auf Standortebene, auf Domänenebene und dann auf Organisationseinheitsebene angewendet.

![](images/Dd443661.2e80f885-2f88-4bd2-be67-862515aa2353(de-de,TechNet.10).gif)

**Abbildung 5.4. Rangfolge, nach der GPOs auf einen Computer angewendet werden**

Bei Computern, auf denen die Betriebssysteme Windows Vista oder Windows XP ausgeführt werden und die in mehreren Organisationseinheitsebenen verschachtelt sind, werden GPOs von der übergeordneten Organisationseinheit in der Hierarchie der Reihenfolge nach bis zur niedrigsten untergeordneten Organisationseinheit angewendet. Das letzte Gruppenrichtlinienobjekt wird aus der Organisationseinheit angewendet, die den Clientcomputer enthält. Diese Reihenfolge der Verarbeitung von Gruppenrichtlinienobjekten – lokale Sicherheitsrichtlinie, Standort, Domäne, übergeordnete Organisationseinheit und untergeordnete Organisationseinheit – ist von Bedeutung, da Gruppenrichtlinienobjekte, die später im Prozess angewendet werden, zuvor angewendete überschreiben. Gruppenrichtlinienobjekte für Benutzer werden in gleicher Weise angewendet.

Beim Entwerfen von Gruppenrichtlinien sollten Sie die folgenden Punkte berücksichtigen:

-   Der Administrator muss die Reihenfolge festlegen, in der mehrere Gruppenrichtlinienobjekte mit einer Organisationseinheit verknüpft werden. Andernfalls werden die Gruppenrichtlinien standardmäßig in der Reihenfolge angewendet, in der sie mit der Organisationseinheit verknüpft wurden. Wenn in mehreren Richtlinien die gleiche Einstellung festgelegt wird, hat die Richtlinie Vorrang, die sich in der Richtlinienliste für den Container am weitesten oben befindet.
-   Ein Gruppenrichtlinienobjekt kann mit der Option Erzwungen konfiguriert werden. Wenn Sie diese Option auswählen, können die in diesem Gruppenrichtlinienobjekt festgelegten Einstellungen nicht von anderen Gruppenrichtlinienobjekten außer Kraft gesetzt werden.
-   Die Option Richtlinienvererbung deaktivieren kann für Active Directory, einen Standort, eine Domäne oder eine Organisationseinheit festgelegt werden. Durch diese Option werden die GPO-Einstellungen aus in der Active Directory-Hierarchie höher stehenden GPOs gesperrt, sofern für diese nicht die Option Erzwungen ausgewählt wurde. Das bedeutet, dass die Option Erzwungen Vorrang vor der Option Richtlinienvererbung deaktivieren hat.
-   Gruppenrichtlinieneinstellungen gelten für Benutzer und Computer und basieren auf dem Speicherort des jeweiligen Benutzer- oder Computerobjekts in Active Directory. In einigen Fällen kann es erforderlich sein, Richtlinien auf ein Benutzerobjekt auf Grundlage des Speicherorts des Computerobjekts anstelle des Speicherorts des Benutzerobjekts anzuwenden. Mithilfe der Loopbackfunktion für Gruppenrichtlinien kann der Administrator Gruppenrichtlinieneinstellungen für Benutzer auf Grundlage des Computers anwenden, an dem der Benutzer angemeldet ist. Im Microsoft Knowledge Base-Artikel Loopbackverarbeitung von Gruppenrichtlinien finden Sie weitere Informationen zu dieser Option.

### Empfohlener GPO-Entwurf

Wenn Sie den oben beschriebenen Organisationseinheitsentwurf verwenden, müssen Sie zur Bereitstellung beider in diesem Handbuch beschriebenen Sicherheitsumgebungen GPOs einsetzen.

Für die EC-Umgebung wäre Folgendes erforderlich:

-   Ein GPO für EC-Benutzerkonfigurationseinstellungen
-   Ein GPO für EC-Computerkonfigurationseinstellungen
-   Für die SSLF-Umgebung wäre ebenso Folgendes erforderlich:
-   Ein GPO für SSLF-Benutzerkonfigurationseinstellungen
-   Ein GPO für SSLF-Computerkonfigurationseinstellungen

In der folgenden Abbildung wird aufgezeigt, wie diese GPOs mit einer einfachen Organisationseinheitsstruktur verknüpft werden können.

![](images/Dd443661.9bf48a62-970c-4265-8b6e-efdc85040653(de-de,TechNet.10).gif)

**Abbildung 5.5. Verknüpfen von GPOs mit einer einfachen Organisationseinheitsstruktur**

In diesem Beispiel werden die EC-Sicherheitseinstellungen auf Computer angewendet, auf denen entweder Windows Vista oder Windows XP ausgeführt wird. Die Sicherheitseinstellungen werden dabei in der folgenden Reihenfolge angewendet:

1.  Lokale Richtlinien werden auf alle Windows Vista- und Windows XP-basierten Computer angewendet.
2.  Domänensicherheitseinstellungen werden auf alle Windows Vista- und Windows XP-basierten Computer aus dem Gruppenrichtlinienobjekt der Domäne angewendet.
3.  Sicherheitseinstellungen werden auf Windows Vista- und Windows XP-basierte Computer aus dem GPO der EC-Benutzerkonfiguration und dem GPO der EC-Computerkonfiguration angewendet.

Da in diesem Beispiel nur ein Standort vorhanden ist, wird kein GPO auf Standortebene angewendet. Wenn mehrere Standorte vorhanden sind, werden die Einstellungen des Gruppenrichtlinienobjekts auf Standortebene im Anschluss an die lokalen Richtlinien angewendet.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

#### Vorbereiten der Bereitstellung von EC- oder SSLF-Einstellungen

Zum Bereitstellen von EC- oder SSLF-Sicherheitseinstellungen müssen Sie den [GPOAccelerator](http://go.microsoft.com/fwlink/?linkid=103569) herunterladen und ausführen. In Kapitel 4 des *Leitfadens zur Verwendung von GPOAccelerator* (möglicherweise in englischer Sprache) finden Sie eine schrittweise Anleitung zum Bereitstellen der Einstellungen für EC- und SSLF-Umgebungen.

![](images/Dd443661.important(de-de,TechNet.10).gif) **Wichtig:**

Durch das Bereitstellen von Sicherheitseinstellungen über die Gruppenrichtlinie kann es auf Clientcomputern zu unerwarteten Ergebnissen kommen. Testen Sie daher alle Sicherheitseinstellungen vor der Bereitstellung in der Produktion zunächst in einer Testumgebung.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### In diesem Beitrag

-   [Überblick](https://technet.microsoft.com/de-de/library/ab515417-1c5b-44a1-b871-152c2a3b6d9b(v=TechNet.10))
-   [Kapitel 1: Sicherheit in der 2007 Office-Version](https://technet.microsoft.com/de-de/library/b9767904-ac34-4263-89e7-3c3e82eff607(v=TechNet.10))
-   [Kapitel 2: Vertraulichkeitseinstellungen](https://technet.microsoft.com/de-de/library/5204bf0f-65b9-403e-9d94-958dbd1553e1(v=TechNet.10))
-   [Kapitel 3: Integritätseinstellungen](https://technet.microsoft.com/de-de/library/1e5968df-c831-421f-99f1-3799520a7132(v=TechNet.10))
-   [Kapitel 4: Verfügbarkeitseinstellungen](https://technet.microsoft.com/de-de/library/fe08a815-c260-4218-aea7-3f2f8447f81c(v=TechNet.10))
-   Kapitel 5: Entwerfen und Implementieren von Sicherheitseinstellungen

**Download**

[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://www.microsoft.com/downloads/details.aspx?familyid=a12eca33-a20d-45e2-895c-5e021f3ae4c5&displaylang=en)[GPOAccelerator herunterladen](http://www.microsoft.com/downloads/details.aspx?familyid=a46f1dbe-760c-4807-a82f-4f02ae3c97b0&displaylang=en)
**Update-Benachrichtigungen**

[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://technet.microsoft.com/hi-in/solutionaccelerators/bb687756(en-us).aspx)
**Feedback**

[Senden Sie uns Ihre Kommentare und Anregungen](https://technet.microsoft.com/de-de/library/secwish%40microsoft.com(v=TechNet.10))
 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><div>
<a href="#mainsection"></a><a href="#mainsection">Zum Seitenanfanq</a>
</div></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/fe08a815-c260-4218-aea7-3f2f8447f81c(v=TechNet.10)"><img src="images/Dd443661.pageLeft(de-de,TechNet.10).gif" /></a> 6 von 6</td>
</tr>
</tbody>
</table>
