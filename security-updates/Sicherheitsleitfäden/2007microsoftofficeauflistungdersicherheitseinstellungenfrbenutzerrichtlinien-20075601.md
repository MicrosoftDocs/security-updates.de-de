---
Title: 2007 Microsoft Office-Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien
TOCTitle: 2007 Microsoft Office-Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien
ms:assetid: 2e2c33dc-f4b7-41a4-a54b-1e08dcf57479
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443657(v=TechNet.10)
ms:contentKeyID: 20075601
---


# 2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen


### Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1
Veröffentlicht: 11. Nov 2007
 

Die Einstellungen im folgenden Abschnitt sind nach Namen aufgeführt.

#### Auf dieser Seite
[Informationen zu Benutzerrichtlinieneinstellungen](#ecd)

## Informationen zu Benutzerrichtlinieneinstellungen

Für jede Einstellung werden neben einer Beschreibung auch Informationen über die betroffenen Anwendungen, das behandelte Sicherheitsrisiko, die Art und Weise, in der das Sicherheitsrisiko behandelt wird, und andere Erwägungen bereitgestellt. Darüber hinaus ist für jede Einstellung eine Tabelle verfügbar, die den Speicherort der Einstellung in der Gruppenrichtlinie, die ADM-Datei mit der Einstellung, die empfohlene Konfiguration für EC- und SSLF-Umgebungen sowie zugehörige CCE-Bezeichner (Common Configuration Enumeration) aufführt.

### Zugriff auf veröffentlichte Kalender

Betrifft: **Outlook**

Die Einstellung bestimmt, welche Einschränkungen für Benutzer gelten, die ihre Kalender auf Microsoft® Office Online- oder WebDAV-Servern von Drittanbietern veröffentlichen.

#### Sicherheitsrisiko

Standardmäßig können Benutzer Kalender für andere freigeben, indem sie sie beim Microsoft Office Online-Freigabedienst für Kalender oder auf einem Server, der das WebDAV-Protokoll (World Wide Web Distributed Authoring and Versioning) unterstützt, veröffentlichen. Bei Office Online können Benutzer auswählen, ob der Zugriff auf ihre Kalender auf eingeladene Benutzer eingeschränkt oder ob allen Benutzern, die die URL für den Kalender kennen, uneingeschränkter Zugriff gewährt werden soll. DAV-Zugriffsbeschränkungen können nur mithilfe von Server- und Ordnerberechtigungen durchgesetzt und müssen möglicherweise durch einen Serveradministrator eingerichtet und verwaltet werden.

Wenn ein Kalender für alle Benutzer von Office Online oder DAV-Servern von Drittanbietern sichtbar ist, könnten u. U. vertrauliche, in den Kalenderterminen enthaltene Informationen zugänglich werden.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, ist für auf Office Online veröffentlichte Kalender ein eingeschränkter Zugriff möglich, und Benutzer können keine Kalender an DAV-Server von Drittanbietern veröffentlichen.

**Tabelle 1.1. Zugriff auf veröffentlichte Kalender**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\Kalenderoptionen\Microsoft Office Online-Freigabedienst

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


Aktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1266

</td>

</tr>

</table>

#### Auswirkung

Durch die empfohlene Einstellung für SSLF-Umgebungen ändert sich die Standardkonfiguration für die meisten Benutzer. Die meisten Benutzer wollen aber wahrscheinlich ihre Kalender nicht für jeden Benutzer von Office Online verfügbar machen, daher dürften die Auswirkungen in den meisten Umgebungen minimal sein.

### ActiveX-Steuerelementinitialisierung

Betrifft: **2007 Office System**

Diese Einstellung gibt die Sicherheitsstufe für die Microsoft ActiveX®-Initialisierung für alle Microsoft Office-Anwendungen an.

#### Sicherheitsrisiko

ActiveX-Steuerelemente können sich direkt negativ auf einen Computer auswirken. Außerdem kann schädlicher Code eingesetzt werden, um ein ActiveX-Steuerelement zu manipulieren und einen Computer anzugreifen. Entwickler haben die Möglichkeit, ActiveX-Steuerelemente als „Sicher für Initialisierung“ (Safe For Initialization, SFI) zu kennzeichnen. SFI gibt an, dass ein Steuerelement bedenkenlos geöffnet und ausgeführt werden kann und dem Computer keinen Schaden zufügt, unabhängig davon, ob es permanente Datenwerte enthält oder nicht.

Wenn ein Steuerelement nicht als SFI gekennzeichnet ist, könnte es möglicherweise negative Auswirkungen auf den Computer haben. Weiterhin könnte dies bedeuten, dass das Steuerelement nicht in allen Situationen getestet wurde und die Entwickler sich nicht sicher sein können, ob es in Zukunft gefährdet sein könnte.

Wenn ein Steuerelement als SFI gekennzeichnet ist, lädt die Anwendung das Steuerelement standardmäßig im abgesicherten Modus und verwendet ggf. permanente Werte. Wenn das Steuerelement nicht als SFI gekennzeichnet ist, lädt die Anwendung es im nicht abgesicherten Modus und ggf. mit permanenten Werten, oder es werden die Standard-Einstellungen (für die erstmalige Initialisierung) verwendet. In beiden Fällen wird der Benutzer über die Statusleiste informiert, dass die Steuerelemente deaktiviert wurden, und muss auf die Nachricht reagieren.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren die ActiveX-Sicherheitsstufe auf eine Zahl zwischen 1 und 6 festlegen. Diese Sicherheitsstufen werden in der folgenden Tabelle erläutert:

**Tabelle 1.2. Konfigurierbare Sicherheitseinstellungen für ActiveX-Steuerelemente**

<table>

<tr>
<th>**Wert**</th>
<th>
**Erläuterung**
</th>

</tr>

<tr>

<td>


1

</td>

<td>


Das Steuerelement wird unabhängig davon, wie es gekennzeichnet ist, geladen, und die permanenten Werte werden ggf. verwendet. Bei dieser Einstellung erhält der Benutzer keine Aufforderung zu reagieren.

</td>

</tr>

<tr>

<td>


2

</td>

<td>


Wenn das Steuerelement als SFI gekennzeichnet ist, wird es im abgesicherten Modus geladen, und es werden ggf. permanente Werte verwendet. Wenn das Steuerelement nicht als SFI gekennzeichnet ist, wird es im nicht abgesicherten Modus geladen, und es werden ggf. permanente Werte verwendet, oder es werden die Standardeinstellungen (für die erstmalige Initialisierung) verwendet. Diese Stufe ähnelt der Standardkonfiguration, aber der Benutzer erhält keine Aufforderung zu reagieren.

</td>

</tr>

<tr>

<td>


3

</td>

<td>


Wenn das Steuerelement als SFI gekennzeichnet ist, wird es im nicht abgesicherten Modus geladen, und es werden ggf. permanente Werte verwendet. Wenn das Steuerelement nicht als SFI gekennzeichnet ist, erhält der Benutzer eine Aufforderung mit einer Nachricht, dass das Steuerelement als unsicher gekennzeichnet ist. Wenn der Benutzer bei der Aufforderung **Nein** auswählt, wird das Steuerelement nicht geladen. Andernfalls wird es mit den Standardeinstellungen (für die erstmalige Initialisierung) geladen.

</td>

</tr>

<tr>

<td>


4

</td>

<td>


Wenn das Steuerelement als SFI gekennzeichnet ist, wird es im abgesicherten Modus geladen, und es werden ggf. permanente Werte verwendet. Wenn das Steuerelement nicht als SFI gekennzeichnet ist, erhält der Benutzer eine Aufforderung mit einer Nachricht, dass das Steuerelement als unsicher gekennzeichnet ist. Wenn der Benutzer bei der Aufforderung **Nein** auswählt, wird das Steuerelement nicht geladen. Andernfalls wird es mit den Standardeinstellungen (für die erstmalige Initialisierung) geladen.

</td>

</tr>

<tr>

<td>


5

</td>

<td>


Wenn das Steuerelement als SFI gekennzeichnet ist, wird es im nicht abgesicherten Modus geladen, und es werden ggf. permanente Werte verwendet. Wenn das Steuerelement nicht als SFI gekennzeichnet ist, erhält der Benutzer eine Aufforderung mit einer Nachricht, dass das Steuerelement als unsicher gekennzeichnet ist. Wenn der Benutzer bei der Aufforderung **Nein** auswählt, wird das Steuerelement nicht geladen. Andernfalls wird es mit permanenten Werten geladen.

</td>

</tr>

<tr>

<td>


6

</td>

<td>


Wenn das Steuerelement als SFI gekennzeichnet ist, wird es im abgesicherten Modus geladen, und es werden ggf. permanente Werte verwendet. Wenn das Steuerelement nicht als SFI gekennzeichnet ist, erhält der Benutzer eine Aufforderung mit einer Nachricht, dass das Steuerelement als unsicher gekennzeichnet ist. Wenn der Benutzer bei der Aufforderung **Nein** auswählt, wird das Steuerelement nicht geladen. Andernfalls wird es mit permanenten Werten geladen.

</td>

</tr>

</table>

**Tabelle 1.3. ActiveX-Steuerelementinitialisierung**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen

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


Aktiviert (2)

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


CCE-908

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für die EC-Umgebung ist **Aktiviert**, und Sicherheitsstufe 2 ist ausgewählt. Diese Einstellung setzt die Standardkonfiguration durch und verursacht deshalb für die meisten Benutzer kaum Nutzbarkeitsprobleme.

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Manche ActiveX-Steuerelemente beachten die Registrierungseinstellung für den abgesicherten Modus nicht und laden daher möglicherweise permanente Daten, obwohl Sie die Einstellung so konfiguriert haben, dass das Steuerelement den abgesicherten Modus verwenden soll.

Diese Einstellung erhöht die Sicherheit für ActiveX-Steuerelemente, die korrekt als SFI gekennzeichnet sind. In Fällen von schädlichem oder schlecht entworfenem Code wird ein ActiveX-Steuerelement eventuell fälschlicherweise als SFI gekennzeichnet.

Die empfohlene Einstellung für die SSLF-Umgebung ist **Deaktiviert**, wodurch die Standardkonfiguration durchgesetzt wird. Daher ergeben sich für die meisten Benutzer keine größeren Nutzbarkeitsprobleme.

Einzelheiten zu dieser Richtlinie finden Sie im Abschnitt zu wichtigen Richtlinien im Thema zur [Funktionsweise von Richtlinien](http://r.office.microsoft.com/r/rlidofficeresourcekit?clid=1033&amp;p1=1)   (möglicherweise in englischer Sprache).

### E-Mail-Empfänger den Listen sicherer Absender der Benutzer hinzufügen

Betrifft: **Outlook**

Diese Einstellung bestimmt, ob die E-Mail-Adressen von Empfängern automatisch der Liste sicherer Absender in Microsoft Office Outlook® 2007 hinzugefügt werden.

#### Sicherheitsrisiko

Es kommt vor, dass Benutzer eine E-Mail-Nachricht senden, um sich von einer Adressenliste streichen zu lassen. Wenn der E-Mail-Empfänger dann automatisch der Liste sicherer Absender hinzugefügt wird, werden zukünftige Nachrichten von dieser Adresse nicht mehr im Ordner „Junk-E-Mail“ abgelegt, selbst wenn sie normalerweise als Junk-E-Mail angesehen würden.

Standardmäßig werden die Empfänger ausgehender Nachrichten nicht automatisch der Liste sicherer Absender eines Benutzers hinzugefügt. Diese Konfiguration kann jedoch in der Outlook 2007-Benutzeroberfläche angepasst werden.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, werden Empfänger ausgehender Nachrichten nicht automatisch der Liste sicherer Absender hinzugefügt. Der Benutzer muss dieser Liste explizit Adressen hinzufügen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Wenn diese Einstellung **aktiviert** ist, werden alle Empfänger ausgehender Nachrichten automatisch der Liste sicherer Absender hinzugefügt. Wenn Benutzer einem Absender von Junk-E-Mail antworten, wenn diese Einstellung **aktiviert** ist, werden alle zukünftigen Junk-E-Mails von dieser Adresse als sicher angesehen.

**Tabelle 1.4. E-Mail-Empfänger den Listen sicherer Absender der Benutzer hinzufügen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\Junk-E-Mail

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


Deaktiviert

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


CCE-1130

</td>

</tr>

</table>

#### Auswirkung

In den meisten Fällen wirkt sich ein Ändern dieser Einstellung nur minimal auf die Nutzbarkeit aus. Wenn Benutzer allerdings E-Mail-Nachrichten an viele Empfänger senden, wird durch ein manuelles Hinzufügen der Empfänger zur Liste sicherer Absender möglicherweise die Produktivität beeinträchtigt. In diesem Fall können Sie festlegen, dass die Einstellung für bestimmte Benutzergruppen aktiviert werden soll.

### Als Ebene 1 zu blockierende Dateierweiterungen hinzufügen

Betrifft: **Outlook**

Diese Einstellung steuert, welche Arten von Anlagen (nach Dateierweiterung) von Outlook 2007 nicht geliefert werden.

#### Sicherheitsrisiko

Schädlicher Code wird oft über E-Mails verbreitet. Einige Viren können Kopien ihrer selbst an andere Personen im Adressbuch oder in der Kontaktliste des Opfers senden. Diese potenziell schädlichen Dateien können die Computer unwissender Empfänger beeinträchtigen.

#### Gegenmaßnahme

Outlook 2007 verwendet zwei Sicherheitsebenen, um den Zugriff von Benutzern auf Dateien einzuschränken, die E-Mail-Nachrichten oder anderen Elementen angehängt sind. Dateien mit bestimmten Erweiterungen können als Ebene 1 (Benutzer können die Datei nicht anzeigen) oder Ebene 2 (Benutzer können die Datei öffnen, nachdem sie auf dem Datenträger gespeichert wurde) kategorisiert werden. Benutzer können Dateien aller Typen frei öffnen, die nicht als Ebene 1 oder Ebene 2 kategorisiert sind.

Standardmäßig klassifiziert Outlook eine Reihe von potenziell schädlichen Dateitypen (wie „.exe“, „.reg“ und „.vbs“) als Ebene 1 und blockiert die Zustellung von Dateien mit diesen Erweiterungen. (Die vollständige Auflistung finden Sie in der Liste der [Anlagedateitypen, die von Office 2007 gesperrt werden](http://technet2.microsoft.com/office/en-us/library/bc667b4c-1645-42be-8dc0-af56dc11ef5b1033.mspx)  .)

Wenn diese Einstellung **aktiviert** ist, können Administratoren zusätzliche Dateierweiterungen als Stufe 1 festlegen (also für die Zustellung blockieren). Die Erweiterungen werden in das dazu bereitgestellte Textfeld eingegeben und durch ein Semikolon getrennt.

**Tabelle 1.5. Als Ebene 1 zu blockierende Dateierweiterungen hinzufügen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Anlagensicherheit

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1617

</td>

</tr>

</table>

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Diese Einstellung wird nur verwendet, wenn die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ für **Outlook-Sicherheitsgruppenrichtlinie verwenden** konfiguriert ist. Weitere Informationen finden Sie unter „Outlook-Sicherheitsmodus“ weiter hinten in diesem Handbuch.

#### Auswirkung

Wenn die Einstellung **Anlagen der Ebene 1 anzeigen** aktiviert ist, blockiert Outlook 2007 den Zugriff auf keinerlei Dateitypen. Benutzer können auf Dateien der Ebene 1 genau wie auf Dateien der Ebene 2 durch Speichern auf einem Datenträger zugreifen.

Diese Einstellung wirkt sich möglicherweise auf die Nutzbarkeit aus, besonders, wenn zwischen Benutzern viele Dokumente per E-Mail versendet werden. Wenn ein Dateityp blockiert ist, müssen Benutzer Dateien dieses Typs durch andere Methoden austauschen, z. B. durch Hochladen an freigegebene Speicherorte.

### Als Ebene 2 zu blockierende Dateierweiterungen hinzufügen

Betrifft: **Outlook**

Diese Einstellung steuert, welche Arten von Anlagen (nach Dateierweiterung) auf einem Datenträger gespeichert werden müssen, bevor sie vom Benutzer geöffnet werden können.

#### Sicherheitsrisiko

Schädlicher Code wird oft über E-Mails verbreitet. Einige Viren können Kopien ihrer selbst an andere Personen im Adressbuch oder in der Kontaktliste des Opfers senden. Diese potenziell schädlichen Dateien können die Computer unwissender Empfänger beeinträchtigen.

Dateien mit bestimmten Erweiterungen können als Ebene 1 (Benutzer können die Datei nicht anzeigen) oder Ebene 2 (Benutzer können die Datei öffnen, nachdem sie auf dem Datenträger gespeichert wurde) kategorisiert werden. Benutzer können Dateien aller Typen frei öffnen, die nicht als Ebene 1 oder Ebene 2 kategorisiert sind.

Standardmäßig klassifiziert Outlook 2007 keine Dateierweiterungen als Stufe 2.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren eine Liste von Anlagendateitypen festlegen, die als Stufe 2 klassifiziert sind. Dadurch muss der Benutzer eine Entscheidung treffen, ob er die Anlage zur Anzeige herunterladen will. Durch diesen zusätzlichen Schritt werden die Benutzer dazu angehalten, sich Gedanken über die Anlagen zu machen, die sie herunterladen. Benutzer werden so u. U. davon abgehalten, verdächtige Anlagen zu öffnen.

**Tabelle 1.6. Als Ebene 2 zu blockierende Dateierweiterungen hinzufügen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Anlagensicherheit

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1155

</td>

</tr>

</table>

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Diese Einstellung wird nur verwendet, wenn die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ für **Outlook-Sicherheitsgruppenrichtlinie verwenden** konfiguriert ist. Weitere Informationen finden Sie unter „Outlook-Sicherheitsmodus“ weiter hinten in diesem Handbuch.

#### Auswirkung

Wenn ein Dateityp als Stufe 1 und als Stufe 2 aufgelistet ist, wird er als Stufe 1 behandelt, weil diese höhere Sicherheitsstufe stets Vorrang vor einer niedrigeren Stufe einnimmt.

Stufe 2 ist erheblich weniger sicher als Stufe 1. Erwägen Sie vor dem Klassifizieren eines Dateityps als Stufe 2 daher immer, ob der Dateityp nicht ein guter Kandidat für Stufe 1 ist.

### Dateitypen als Anlagen für Formulare zulassen

Betrifft: **InfoPath**

Diese Einstellung steuert, welche Dateitypen (nach Dateierweiterung) InfoPath 2007-Formularen als Anlagen hinzugefügt werden können.

#### Sicherheitsrisiko

Standardmäßig kann ein Benutzer alle Dateitypen an Formulare anhängen, außer potenziell unsicheren Dateien, die Viren enthalten können, z. B. BAT- oder EXE-Dateien. Eine vollständige Liste der von Microsoft Office InfoPath® 2007 standardmäßig nicht zugelassenen Dateitypen finden Sie im Abschnitt über Sicherheitsdetails unter dem Thema zum [Einfügen eines Dateianlagesteuerelements](http://office.microsoft.com/en-us/infopath/hp100809081033.aspx)   (möglicherweise in englischer Sprache) auf der Microsoft Office Online-Website.

Wenn InfoPath-Formularen unsichere Dateitypen hinzugefügt werden, können sie für Angriffe auf Computern verwendet werden, auf denen das Formular geöffnet wird. Diese unsicheren Dateitypen könnten beispielsweise aktiven Inhalt enthalten oder andere Sicherheitsrisiken einschleusen, die ein Angreifer ausnutzen kann.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist und „Benutzer können Formularen keine unsicheren Dateitypen anfügen“ **deaktiviert** bzw. nicht konfiguriert ist, können Administratoren festlegen, welche Dateierweiterungen von der Standardliste nicht zugelassener Dateitypen in InfoPath 2007 entfernt werden sollen und somit Benutzern ermöglichen, Dateien der festgelegten Typen an Formulare anzuhängen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Informationen zum Hinzufügen weiterer zu blockierender Dateitypen zu InfoPath finden Sie unter der Einstellung „Bestimmte Dateitypen als Anlagen für Formulare blockieren“ in diesem Handbuch.

**Tabelle 1.7. Dateitypen als Anlagen für Formulare zulassen**

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1259

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung kann als weitere Verteidigung gegen unsichere Dateianlagen angesehen werden. Wenn „Benutzer können Formularen keine unsicheren Dateitypen anfügen“ aktiviert ist, wie dies in den EC- und SSLF-Umgebungen der Fall ist, geschieht durch Aktivieren dieser Einstellung nichts: Alle hier angegebenen Dateierweiterungen werden als Anlagen an Formulare nicht zugelassen. Wenn es jedoch keinen legitimen geschäftlichen Grund gibt, aus dem Benutzer unsichere Dateitypen an Formulare anhängen müssen, sollte diese Einstellung nicht aktiviert werden.

Umgekehrt gilt: Wenn es einen legitimen Grund dafür gibt, Benutzern das Anhängen unsicherer Dateitypen an Formulare zu erlauben, sollte diese Einstellung aktiviert und die zulässigen Dateitypen angegeben und darüber hinaus die Einstellung „Benutzer können Formularen keine unsicheren Dateitypen anfügen“ deaktiviert werden.

### Mischung aus Richtlinien- und Benutzerspeicherorten zulassen

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob vertrauenswürdige Speicherorte durch Benutzer, das Office-Anpassungstool (OAT) und die Gruppenrichtlinie definiert werden können oder ob sie allein durch die Gruppenrichtlinie definiert werden.

#### Sicherheitsrisiko

Wenn Access 2007-, Excel 2007-, PowerPoint 2007- und Word 2007-Dateien von vertrauenswürdigen Speicherorten aus geöffnet werden, wird der Inhalt solcher Dateien aktiviert und ist aktiv. Benutzer werden nicht über mögliche Risiken in den Dateien informiert, beispielsweise unsignierte Makros, ActiveX-Steuerelemente oder Verknüpfungen zu Inhalt im Internet.

Standardmäßig können Benutzer jeden Speicherort als vertrauenswürdigen Speicherort festlegen, und es kann auf einem Computer eine Kombination aus vom Benutzer, durch das OAT und durch die Gruppenrichtlinie erstellten vertrauenswürdigen Speicherorten vorliegen.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, werden alle nicht durch die Gruppenrichtlinie erstellten vertrauenswürdigen Speicherorte deaktiviert, und die Benutzer können keine neuen vertrauenswürdigen Speicherorte im Vertrauensstellungscenter erstellen.

**Tabelle 1.8. Mischung aus Richtlinien- und Benutzerspeicherorten zulassen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen\Vertrauensstellungscenter

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


Deaktiviert

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


CCE-770

</td>

</tr>

</table>

#### Auswirkung

Durch Deaktivieren dieser Einstellung ergeben sich Beeinträchtigungen für Benutzer, die im Vertrauensstellungscenter eigene vertrauenswürdige Speicherorte definiert haben. Anwendungen behandeln diese Speicherorte dann genau wie andere nicht vertrauenswürdige Speicherorte. Benutzern werden also beim Öffnen von Dateien Warnungen in der Statusleiste zu aktivem Inhalt wie ActiveX-Steuerelementen und VBA-Makros angezeigt, und sie müssen auswählen, ob die Steuerelemente bzw. Makros aktiviert werden oder deaktiviert bleiben sollen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

InfoPath 2007 und Outlook 2007 erkennen vertrauenswürdige Speicherorte nicht und sind daher von dieser Einstellung nicht betroffen.

### PNG als Ausgabeformat zulassen

Betrifft: **2007 Office System**

Diese Einstellung bestimmt, ob Office-Anwendungen Grafiken im PNG-Format ausgeben können, wenn Dokumente als Webseiten gespeichert werden.

#### Sicherheitsrisiko

Excel 2007, PowerPoint 2007 und Word 2007 können Dateien im PNG-Format (Portable Network Graphics) speichern, um beim Speichern von Dokumenten als Webseiten die Qualität der Grafiken zu verbessern. Das PNG-Grafikdateiformat (.png) wird für eine Vielzahl von Grafiken verwendet, von kleinen Bildern (z. B. Aufzählungen und Banner) bis hin zu komplexen Bildern (z. B. Fotos) und bietet eine naturgetreuere Wiedergabe und kleinere Dateigrößen als einige andere Formate. PNG-Grafiken können jedoch von vielen älteren Webbrowsern wie Microsoft Internet Explorer® Version 5 oder früher nicht angezeigt werden.

Standardmäßig werden Grafiken in Office-Anwendungen nicht im PNG-Format gespeichert. Diese Funktionalität lässt sich ändern, indem Benutzer im Dialogfeld **Optionen** der Anwendung auf **Erweitert** und dann auf **Weboptionen** klicken und anschließend das Kontrollkästchen **PNG als Grafikformat zulassen** aktivieren.

Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf PNG-Dateien abzielen.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, können Office-Anwendungen keine Grafiken im PNG-Format ausgeben. Diese Konfiguration kann vom Benutzer nicht geändert werden.

**Tabelle 1.9. PNG als Ausgabeformat zulassen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…\Browser

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


Deaktiviert

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


CCE-711

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration durch und verursacht deshalb für die meisten Benutzer keine größeren Nutzbarkeitsprobleme.

### Skripts in einmaligen Outlook-Formularen zulassen

Betrifft: **Outlook**

Diese Einstellung steuert, ob Skripts in Outlook 2007-Formularen ausgeführt werden können, bei denen Skript und Layout in der Nachricht enthalten sind.

#### Sicherheitsrisiko

In Outlook-Formulare kann schädlicher Code eingebettet werden, der beim Öffnen des Formulars ausgeführt werden könnte.

Standardmäßig führt Outlook 2007 keine Skripts in Formularen aus, bei denen Skript und Layout in der Nachricht enthalten sind.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, werden Skripts in einmaligen Outlook 2007-Formularen nicht ausgeführt.

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Wenn diese Einstellung **aktiviert** ist, können Skripts in einmaligen Outlook-Formularen ausgeführt werden, wodurch die Sicherheit möglicherweise erheblich verringert wird.

**Tabelle 1.10. Skripts in einmaligen Outlook-Formularen zulassen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Benutzerdefinierte Formularsicherheit

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


Deaktiviert

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


CCE-1595

</td>

</tr>

</table>

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Diese Einstellung wird nur verwendet, wenn die Gruppenrichtlinieneinstellung „Outlook-Sicherheitsmodus“ für **Outlook-Sicherheitsgruppenrichtlinie verwenden** konfiguriert ist. Weitere Informationen finden Sie unter „Outlook-Sicherheitsmodus“ weiter hinten in diesem Handbuch.

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und verursacht deshalb für die meisten Benutzer keine größeren Nutzbarkeitsprobleme.

Das Ausführen von Skripts in einmaligen Outlook-Formularen zuzulassen kann ein erhebliches Risiko darstellen. Wenn Benutzer keinen legitimen Geschäftsgrund für diese Funktionalität besitzen, sollte diese Einstellung deaktiviert sein. Wenn Ihr Unternehmen Formulare mit Skripts verwendet, erwägen Sie eine Umgestaltung dieser Formulare.

### Vertrauenswürdige Speicherorte, die sich nicht auf dem Computer befinden, zulassen

Betrifft: **Access, Excel, PowerPoint, Word**

Diese Einstellung steuert, ob vertrauenswürdige Speicherorte innerhalb des Netzwerks verwendet werden können.

#### Sicherheitsrisiko

Standardmäßig werden Dateien aus vertrauenswürdigen Speicherorten, die im Vertrauensstellungscenter angegeben sind, als sicher angesehen. Inhalt, Code und Add-Ins aus vertrauenswürdigen Speicherorten werden unter minimaler Sicherheit geladen, und der Benutzer wird nicht zur Bestätigung aufgefordert.

Standardmäßig können Benutzer vertrauenswürdige Speicherorte auf Netzwerkfreigaben oder an anderen Remotespeicherorten festlegen, die nicht ihrer direkten Kontrolle unterstehen, indem sie das Kontrollkästchen **Vertrauenswürdige Speicherorte im Netzwerk zulassen (nicht empfohlen)** im Abschnitt **Vertrauenswürdige Speicherorte** des Vertrauensstellungscenters aktivieren. Wenn eine gefährliche Datei aus einem vertrauenswürdigen Speicherort geöffnet wird, unterliegt sie nicht den normalen Sicherheitsmaßnahmen und könnte den Computer oder die Daten des Benutzers gefährden.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, ignoriert die ausgewählte Anwendung alle im Abschnitt **Vertrauenswürdige Speicherorte** des Vertrauensstellungscenters aufgeführten Netzwerkspeicherorte.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Durch Aktivieren dieser Einstellung werden keine Netzwerkspeicherorte aus der Liste vertrauenswürdiger Speicherorte entfernt. Stattdessen wird die ausgewählte Anwendung gezwungen, die Speicherorte als nicht vertrauenswürdig zu behandeln und Benutzer daran zu hindern, der Liste neue Netzwerkspeicherorte hinzuzufügen.

**Tabelle 1.11. Vertrauenswürdige Speicherorte, die sich nicht auf dem Computer befinden, zulassen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Anwendungseinstellungen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


access12.adm, excel12.adm, ppt12.adm, word12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Deaktiviert

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


**CCE-IDs**

</td>

<td>


Access: CCE-780

Excel: CCE-1444

PowerPoint: CCE-747

Word: CCE-1355

</td>

</tr>

</table>

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Wenn Sie vertrauenswürdige Speicherorte auch über die Gruppenrichtlinie bereitstellen, sollten Sie überprüfen, ob es sich dabei um Remotespeicherorte handelt. Wenn Remotespeicherorte vorliegen und Sie über diese Einstellung keine Remotespeicherorte zulassen, werden die Richtlinienschlüssel, die auf Remotespeicherorte zeigen, auf den Clientcomputern ignoriert.

#### Auswirkung

Die Deaktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die der Liste **vertrauenswürdiger Speicherorte** Netzwerkstandorte hinzufügen. Diese Vorgehensweise wird allerdings nicht empfohlen (wie das Kontrollkästchen **Vertrauenswürdige Speicherorte im Netzwerk zulassen (nicht empfohlen)** ja besagt), es müsste also in der Praxis möglich sein, diese Einstellung in den meisten Fällen zu deaktivieren, ohne erhebliche Nutzbarkeitsprobleme für den Großteil der Benutzer zu verursachen.

### Benutzer können Anlagen auf Ebene 2 tiefer stufen

Betrifft: **Outlook**

Diese Einstellung steuert, ob Outlook 2007-Benutzer Anlagen durch Verwendung eines Registrierungsschlüssels auf Stufe 2 herunterstufen können, wodurch die Dateien auf einem Datenträger gespeichert und von diesem Speicherort geöffnet werden könnten.

#### Sicherheitsrisiko

Outlook 2007 verwendet zwei Sicherheitsebenen, um den Zugriff auf Dateien einzuschränken, die E-Mail-Nachrichten oder anderen Elementen angehängt sind. Dateien mit bestimmten Erweiterungen können als Ebene 1 (Benutzer können die Datei nicht anzeigen) oder Ebene 2 (Benutzer können die Datei öffnen, nachdem sie auf dem Datenträger gespeichert wurde) kategorisiert werden. Benutzer können Dateien aller Typen frei öffnen, die nicht als Ebene 1 oder Ebene 2 kategorisiert sind.

Standardmäßig erlaubt Outlook Benutzern nicht, Dateitypen von Stufe 1 auf Stufe 2 herunterzustufen. Wenn diese Einstellung **aktiviert** ist, können Benutzer eine Liste von Dateitypen der Stufe 1 erstellen, die auf Stufe 2 heruntergestuft werden sollen, indem die Dateitypen dem folgenden Registrierungsschlüssel hinzugefügt werden:

**HKEY_CURRENT_USER\Software\Microsoft\Office\Outlook\12.0\Security\Level1Remove**

Wenn Benutzer Dateien der Stufe 1 auf Stufe 2 herunterstufen können, sind sie in der Lage, durch Speichern auf einem Datenträger auf potenziell gefährliche Dateien zuzugreifen. Dadurch könnte schädlicher Code ihre Computer beeinträchtigen oder die Sicherheit vertraulicher Daten gefährden.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, können Benutzer Anlagen der Stufe 1 nicht auf Stufe 2 herunterstufen, und der Registrierungsschlüssel **HKEY_CURRENT_USER\Software\Microsoft\Office\Outlook\12.0\Security\Level1Remove** hat keine Auswirkungen.

**Tabelle 1.12. Benutzer können Anlagen auf Ebene 2 tiefer stufen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Anlagensicherheit

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


Deaktiviert

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


CCE-1388

</td>

</tr>

</table>

#### Auswirkung

Wenn Benutzern erlaubt wird, Anlagen auf Stufe 2 herunterzustufen, stellt dies möglicherweise ein erhebliches Risiko dar. Wenn Benutzer keinen legitimen Geschäftsgrund für diese Funktionalität besitzen, sollte diese Einstellung deaktiviert sein.

### Benutzer mit früheren Versionen von Office können mit Browsern lesen...

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob IRM-aktivierte (Information Rights Management) Dateien von Office-Anwendungen in einem Format gespeichert werden, die in Microsoft Internet Explorer mit dem Windows® Rights Management-Add-On angezeigt werden können.

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103504)  .

#### Sicherheitsrisiko

Das Windows Rights Management-Add-On für Internet Explorer bietet Benutzern, die nicht die 2007 Office-Version verwenden, die Möglichkeit, Dateien mit eingeschränkten Berechtigungen anzuzeigen, jedoch nicht zu ändern. Standardmäßig werden IRM-aktivierte Dateien in einem Format gespeichert, das bei Verwendung des Windows Rights Management-Add-Ons nicht angezeigt werden kann. Wenn diese Einstellung aktiviert ist, wird eine eingebettete HTML-Version des Inhalts mit verwalteten Rechten mit jeder IRM-aktivierten Datei gespeichert. Diese kann dann in Internet Explorer unter Verwendung des Add-Ons angezeigt werden. Durch diese Konfiguration erhöht sich die Größe von Dateien mit verwalteten Rechten in manchen Fällen erheblich.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, speichern Office-Anwendungen IRM-aktivierte Dateien nicht in einem Format, welches das Windows Rights Management-Add-On unterstützt.

**Tabelle 1.13. Benutzer mit früheren Versionen von Office können mit Browsern lesen...**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Eingeschränkte Berechtigungen verwalten

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


Deaktiviert

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


CCE-1612

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration durch und verursacht deshalb für die meisten Benutzer keine größeren Nutzbarkeitsprobleme.

### Gruppen in Office immer erweitern, wenn die Berechtigung für Dokumente eingeschränkt wird

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Gruppennamen automatisch erweitert werden, um alle Mitglieder der Gruppe anzuzeigen, wenn sie im Dialogfeld **Berechtigungen** aktiviert ist.

#### Sicherheitsrisiko

Wenn Benutzer bei Zuweisung von IRM-Berechtigungen (Information Rights Management) für Excel 2007-Arbeitsmappen, InfoPath 2007-Vorlagen, Outlook 2007-E-Mail-Nachrichten, PowerPoint 2007-Präsentationen oder Word 2007-Dokumente einen Gruppennamen im Dialogfeld **Berechtigungen** auswählen, werden die Mitglieder der Gruppe nicht angezeigt. Durch diese Funktionalität ist es möglich, dass Benutzer nicht geeigneten Personen unwissentlich Lese- oder Änderungsberechtigungen erteilen.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, wird das Dialogfeld automatisch erweitert, sodass alle Mitglieder der Gruppe angezeigt werden, wenn Benutzer im Dialogfeld **Berechtigungen** eine Gruppe auswählen.

**Tabelle 1.14. Gruppen in Office immer erweitern, wenn die Berechtigung für Dokumente eingeschränkt wird**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Eingeschränkte Berechtigungen verwalten

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


Aktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1409

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Namen im Dialogfeld **Berechtigungen** anders angezeigt. Dies dürfte für die meisten Benutzer jedoch keine größeren Nutzbarkeitsprobleme verursachen.

### Benutzer müssen zum Überprüfen der Berechtigung immer eine Verbindung herstellen

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Benutzer bei jedem Öffnen von Excel 2007-Arbeitsmappen, InfoPath 2007-Formularen oder -Vorlagen, Outlook 2007-E-Mail-Nachrichten, PowerPoint 2007-Präsentationen oder Word 2007-Dokumenten, die durch Information Rights Management (IRM) geschützt sind, eine Verbindung mit dem Internet oder einem lokalen Netzwerk herstellen müssen, um ihre Lizenzen zu bestätigen.

#### Sicherheitsrisiko

Standardmäßig müssen Benutzer keine Verbindung mit dem Netzwerk herstellen, um Berechtigungen zu überprüfen. Wenn Benutzer keine Bestätigung einholen müssen, wenn sie 2007 Office-Dokumente öffnen, können sie möglicherweise auf Dokumente zugreifen, nachdem ihre Lizenzen abgelaufen sind. Außerdem ist es nicht möglich, die Verwendung von Dateien mit eingeschränkten Berechtigungen zu protokollieren, wenn die Benutzerlizenzen nicht überprüft werden.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, müssen die Benutzer eine Verbindung herstellen, um ihre Berechtigungen bestätigen zu lassen.

**Tabelle 1.15. Benutzer müssen zum Überprüfen der Berechtigung immer eine Verbindung herstellen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Eingeschränkte Berechtigungen verwalten

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


Aktiviert

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


CCE-1493

</td>

</tr>

</table>

#### Auswirkung

Das Aktivieren dieser Einstellung kann zu Problemen für Benutzer führen, die Dateien mit verwalteten Rechten öffnen müssen, wenn sie nicht mit dem Internet verbunden sind, beispielsweise mobile Benutzer. Erwägen Sie vor dem Aktivieren dieser Einstellung die Durchführung einer Umfrage in Ihrem Unternehmen, um festzustellen, ob Benutzer Dateien mit verwalteten Rechten offline verwenden.

### Makrosicherheitseinstellungen auf Makros, Add-Ins und SmartTags anwenden

Betrifft: **Outlook**

Diese Einstellung steuert, ob Outlook 2007 die Makro-Sicherheitseinstellungen auch auf installierte COM-Add-Ins und Smarttags anwendet.

#### Sicherheitsrisiko

Angreifer können schädlichen Code in Add-Ins und Smarttags einfügen, um Ihre Computerumgebung anzugreifen. Standardmäßig unterliegen COM-Add-Ins und Smarttags nicht den gleichen Sicherheitseinschränkungen wie installierte Makros.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, werden die Makrosicherheitseinstellungen auch auf Add-Ins und Smarttags angewendet.

**Tabelle 1.16. Makrosicherheitseinstellungen auf Makros, Add-Ins und SmartTags anwenden**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Vertrauensstellungscenter

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


Aktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1462

</td>

</tr>

</table>

#### Auswirkung

Wenn diese Einstellung **aktiviert** ist und für Makros eine hohe Sicherheitsstufe ausgewählt wurde, werden Add-Ins und Smarttags mit erhöhten Sicherheitseinschränkungen ausgeführt. Diese Konfiguration wirkt sich möglicherweise auf Benutzer aus, die Add-Ins und Smarttags verwenden.

### Aktualisieren von automatischen Verknüpfungen bestätigen

Betrifft: **Excel**

Diese Einstellung steuert, ob Excel 2007 Benutzer zum Aktualisieren automatischer Verknüpfungen auffordert oder ob die Aktualisierung ohne Aufforderung im Hintergrund erfolgt.

#### Sicherheitsrisiko

Wenn eine Excel 2007-Arbeitsmappe Verknüpfungen zu anderen Dokumenten enthält und Benutzer nicht aufgefordert werden, diese zu bestätigen, könnte sich der Inhalt der Arbeitsmappe ohne Wissen des Benutzers ändern, da Änderungen an den verknüpften Dateien vorgenommen wurden.

Standardmäßig werden Benutzer aufgefordert, automatische Verknüpfungen zu aktualisieren.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, fordert Excel 2007 Benutzer zum Aktualisieren automatischer Verknüpfungen auf, wodurch die Standardkonfiguration durchgesetzt wird.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Wenn diese Einstellung **deaktiviert** ist, aktualisiert Excel automatische Verknüpfungen, ohne den Benutzer zu benachrichtigen oder zur Bestätigung aufzufordern. Hierdurch könnte die Integrität bestimmter Informationen in der Arbeitsmappe gefährdet werden.

**Tabelle 1.17. Aktualisieren von automatischen Verknüpfungen bestätigen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Erweitert

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert

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


CCE-1119

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in Excel 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

### Anlage sicherer temporärer Ordner

Betrifft: **Outlook**

Mit dieser Einstellung können Administratoren einen Ordnerpfad zum sicheren Ordner für temporäre Dateien angeben, anstatt den von Outlook 2007 zufällig generierten Pfad zu verwenden.

#### Sicherheitsrisiko

Der sichere Ordner für temporäre Dateien dient zum Speichern von Anlagen, wenn diese in einer E-Mail geöffnet werden. Standardmäßig generiert Outlook 2007 einen zufälligen Namen für den sicheren Ordner für temporäre Dateien und speichert ihn im Ordner „Temporäre Internetdateien“. Mithilfe dieser Einstellung können Sie einen bestimmten Pfad und Ordner zur Verwendung als sicheren Ordner für temporäre Dateien festlegen. Diese Konfiguration wird nicht empfohlen, weil dadurch die temporären Outlook-Dateien aller Benutzer am gleichen vorhersagbaren Standort gespeichert werden, was die Sicherheit beeinträchtigt. Wenn der Ordnername sehr gängig ist, könnte ein böswilliger Benutzer oder ein schädlicher Code diesen Speicherort angreifen, um Zugriff auf die Anlagen zu erhalten.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, weist Outlook 2007 dem sicheren Ordner für temporäre Dateien für die einzelnen Benutzer jeweils einen unterschiedlichen zufälligen Namen zu.

**Tabelle 1.18. Anlage sicherer temporärer Ordner**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie\Dialogfeld „Signaturstatus“

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


Deaktiviert

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


CCE-1591

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine größeren Nutzbarkeitsprobleme verursachen.

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Wenn für Outlook-Anlagen ein bestimmter Ordner verwendet werden muss, empfiehlt Microsoft ein lokales Verzeichnis (für die beste Leistung), ein Platzieren des Ordners unterhalb des Ordners für temporäre Internetdateien (um von der erhöhten Sicherheit dieses Ordners zu profitieren) sowie einen eindeutigen und schwer zu erratenden Ordnernamen.

### Authentifizierung mit Exchange Server

Betrifft: **Outlook**

Diese Einstellung steuert, welche Authentifizierungsmethoden Outlook 2007 für die Authentifizierung mit Microsoft Exchange Server verwendet.

#### Sicherheitsrisiko

Exchange Server unterstützt für die Authentifizierung das Kerberos-Authentifizierungsprotokoll sowie NTLM. Das Kerberos-Protokoll ist die sicherere Authentifizierungsmethode und wird von Windows 2000 Server und späteren Versionen unterstützt. Die NTLM-Authentifizierung wird in Umgebungen vor Windows 2000 unterstützt.

Standardmäßig versucht Outlook 2007, die Authentifizierung mithilfe des Kerberos-Authentifizierungsprotokolls vorzunehmen. Wenn dies nicht möglich ist (weil keine Windows 2000- oder spätere Domänencontroller verfügbar sind), wird zur Authentifizierung NTLM verwendet.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei verschiedenen Optionen auswählen, um die Authentifizierung von Outlook 2007 mit Microsoft Exchange Server zu steuern:
* **Kerberos-/NTLM-Management-Kennwortauthentifizierung**. Outlook versucht, die Authentifizierung mithilfe des Kerberos-Authentifizierungsprotokolls vorzunehmen. Wenn dieser Versuch fehlschlägt, versucht Outlook die Authentifizierung mit NTLM. Dies ist die Standardkonfiguration.

* **Kerberos-Kennwortauthentifizierung**. Outlook versucht, die Authentifizierung ausschließlich mit dem Kerberos-Protokoll vorzunehmen.

* **NTLM-Kennwortauthentifizierung**. Outlook versucht, die Authentifizierung ausschließlich mit NTLM vorzunehmen.


**Tabelle 1.19. Authentifizierung mit Exchange Server**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Kontoeinstellungen\Exchange

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


Aktiviert (Kerberos-/NTLM-Management-Kennwortauthentifizierung)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Kerberos-/NTLM-Management-Kennwortauthentifizierung)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1712

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für EC- und SSLF-Umgebungen setzt die Standardkonfiguration durch und sollte daher für die meisten Benutzer keine größeren Nutzbarkeitsprobleme verursachen.

### Profil automatisch basierend auf der primären SMTP-Adresse von Active Directory konfigurieren

Betrifft: **Outlook**

Diese Einstellung steuert, ob Benutzer, die Teil einer Domäne in einer Active Directory®-Umgebung sind, die primäre SMTP-Adresse ändern können, die bei der Kontoeinrichtung in Outlook 2007 verwendet wurde.

#### Sicherheitsrisiko

Wenn ein Benutzer Teil einer Domäne in einer Active Directory-Umgebung ist und für ihn kein E-Mail-Konto konfiguriert wurde, füllt Outlook 2007 das E-Mail-Adressfeld des Assistenten für ein neues Konto standardmäßig mit der primären SMTP-Adresse des Benutzers auf, der derzeit bei Active Directory angemeldet ist. Der Benutzer kann die Adresse ändern, um ein anderes Konto zu konfigurieren, oder aber auf **Weiter** klicken, um die Active Directory-Standardeinstellungen zu verwenden.

Wenn Benutzern ein Ändern dieser Adresse ermöglicht wird, könnten sie möglicherweise ihre Umgebung falsch konfigurieren oder ihre Identität falsch darstellen.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer die SMTP-Einstellungen, die Outlook 2007 beim Einrichten eines neuen Kontos von Active Directory erhält, nicht ändern.

**Tabelle 1.20. Profil automatisch basierend auf der primären SMTP-Adresse von Active Directory konfigurieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Kontoeinstellungen\Exchange

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


Aktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1281

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert**. Dies könnte Benutzer in seltenen Fällen daran hindern, Outlook 2007 wie gewünscht zu konfigurieren (zum Beispiel, wenn Active Directory während des Setups zeitweilig nicht verfügbar ist). Für die meisten Benutzer dürften jedoch keine größeren Nutzbarkeitsprobleme auftreten.

### Anlagen automatisch herunterladen

Betrifft: **Outlook**

Diese Einstellung steuert, ob Outlook 2007 Dateien herunterlädt, die an Internetkalendertermine angehängt sind.

#### Sicherheitsrisiko

An Internetkalendertermine angehängte Dateien könnten schädlichen Code enthalten, mit dem ein Computer angegriffen werden kann.

Standardmäßig lädt Outlook 2007 beim Abrufen von Internetkalenderterminen keine Anlagen herunter.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, lädt Outlook 2007 keine an Internetkalendertermine angehängten Dateien herunter. Diese Einstellung erzwingt das Standardverhalten.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Wenn diese Einstellung **aktiviert** ist, lädt Outlook automatisch alle Anlagen für Internetkalendertermine herunter. Dadurch werden Benutzer möglicherweise schädlichen Dateien ausgesetzt.

**Tabelle 1.21. Anlagen automatisch herunterladen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Kontoeinstellungen\Internetkalender

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


Deaktiviert

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


CCE-1682

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine größeren Nutzbarkeitsprobleme verursachen.

### Automatisch Inhalt für E-Mail von Personen in den Listen „Sichere Absender“ und „Sichere Empfänger“ herunterladen

Betrifft: **Outlook**

Diese Einstellung steuert, ob Outlook 2007 automatisch externen Inhalt in E-Mails herunterlädt, die von Sendern in der Liste sicherer Absender oder in der Liste sicherer Empfänger stammen.

#### Sicherheitsrisiko

Böswillige E-Mail-Absender können HTML-Nachrichten mit eingebetteten Webbeacons oder mit Bildern und anderen Inhalten von externen Servern versenden, mit denen verfolgt werden kann, ob bestimmte Empfänger eine Nachricht geöffnet haben. Durch Anzeige einer E-Mail-Nachricht mit einem Webbeacon wird bestätigt, dass die E-Mail-Adresse des Empfängers gültig ist, wodurch der Empfänger anfällig für zusätzliche Spam-Nachrichten und schädliche E-Mails wird. Zum Schutz der Benutzer vor Webbeacons kann Outlook 2007 so konfiguriert werden, dass die Anzeige externer Inhalte in E-Mail-Nachrichten automatisch blockiert wird. Da durch diese Konfiguration möglicherweise die Anzeige von erwünschtem Inhalt blockiert wird, kann Outlook auch so konfiguriert werden, dass externer Inhalt in E-Mails von allen Sendern, die auf der Liste sicherer Absender bzw. der Liste sicherer Empfänger aufgeführt sind, automatisch angezeigt wird.

Standardmäßig zeigt Outlook 2007 externen Inhalt in E-Mail-Nachrichten von Sendern automatisch an, wenn diese in der Liste sicherer Absender bzw. der Liste sicherer Empfänger des Benutzers aufgeführt sind, und blockiert automatisch externen Inhalt in anderen Nachrichten. Wenn versehentlich ein böswilliger Absender der Liste sicherer Absender oder der Liste sicherer Empfänger eines Benutzers hinzugefügt wird, zeigt Outlook externen Inhalt aller E-Mail-Nachrichten des böswilligen Absenders an. Dazu könnten auch Webbeacons gehören.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, lädt Outlook 2007 nicht automatisch Inhalt aus externen Servern für Nachrichten herunter, die von Personen aus der Liste sicherer Absender oder der Liste sicherer Empfänger stammen. Empfänger können auf der Basis jeder einzelnen Nachricht entscheiden, ob externe Inhalte heruntergeladen werden.

**Tabelle 1.22. Automatisch Inhalt für E-Mail von Personen in den Listen „Sichere Absender“ und „Sichere Empfänger“ herunterladen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Einstellungen für den automatischen Download von Bildern

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


CCE-725

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für die SSLF-Umgebung ist **Deaktiviert**, was bedeutet, dass Outlook 2007 nicht automatisch externen Inhalt von Nachrichten herunterlädt, die von Personen in der Liste sicherer Absender oder der Liste sicherer Empfänger stammen. Diese Konfiguration kann zu Beeinträchtigungen für Benutzer führen, die regelmäßig HTML-E-Mail-Nachrichten empfangen, die Grafiken oder andere externe Inhalte enthalten, da diese Inhalte für jede Nachricht einzeln heruntergeladen werden müssen.

### Automatisches Empfangen kleiner Updates zur Verbesserung der Zuverlässigkeit

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob die Microsoft Office-Diagnose aktiviert ist.

#### Sicherheitsrisiko

Durch die Office-Diagnose lässt sich die Benutzerfreundlichkeit verbessern, da in regelmäßigen Abständen eine kleine Datei mit aktualisierten Hilfeinformationen zu spezifischen Problemen auf den Computer heruntergeladen wird. Wenn die Office-Diagnose aktiviert ist, erfasst sie Informationen über bestimmte Fehler sowie die IP-Adresse des Computers. Wenn dann neue Hilfeinformationen zur Verfügung stehen, werden diese auf den Computer heruntergeladen, auf dem die jeweiligen Probleme aufgetreten sind. Außer der IP-Adresse des Computers, der das Update beantragt, übermittelt die Office-Diagnose keine personenbezogenen Informationen an Microsoft.

Bei der ersten Ausführung einer 2007 Office-Anwendung können Benutzer standardmäßig auswählen, ob sie Aktualisierungen von der Office-Diagnose erhalten möchten. Wenn Ihr Unternehmen Richtlinien für die Regelung der Verwendung externer Ressourcen wie die Office-Diagnose einsetzt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn eine Auswahl dieser Funktion zugelassen wird.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, erhalten die Benutzer keine Updates von der Office-Diagnose, um die Zuverlässigkeit von 2007 Office-Anwendungen zu verbessern.

**Tabelle 1.23. Automatisches Empfangen kleiner Updates zur Verbesserung der Zuverlässigkeit**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Datenschutz\Vertrauensstellungscenter

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


Deaktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-276

</td>

</tr>

</table>

#### Auswirkung

Durch Deaktivieren dieser Einstellung können Benutzer keine Informationen und Hinweise von Microsoft zum Beheben und Vermeiden von 2007 Office-Anwendungsfehlern erhalten. Dadurch könnte eine erhöhte Menge an Supportanforderungen für Desktops bei Ihrer Supportabteilung eingehen.

### Automatisierungssicherheit

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Makros in einer 2007 Office-Anwendung ausgeführt werden können, die programmgesteuert von einer anderen Anwendung geöffnet wird.

#### Sicherheitsrisiko

Wenn ein separates Programm zum programmgesteuerten Starten von Microsoft Office Excel 2007, PowerPoint 2007 oder Word 2007 verwendet wird, können alle Makros in der programmgesteuert geöffneten Anwendung ohne Blockieren ausgeführt werden. Diese Funktionalität könnte es einem Angreifer ermöglichen, automatisch schädlichen Code in Excel, PowerPoint oder Word auszuführen.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren aus drei Optionen zum Steuern des Makroverhaltens in Excel 2007, PowerPoint 2007 und Word 2007 auswählen, wenn die Anwendung programmgesteuert geöffnet wird:
* **Makros standardmäßig deaktivieren**. Alle Makros sind in der programmgesteuert geöffneten Anwendung deaktiviert.

* **Mit Makros (Standard)**. Makros können in der programmgesteuert geöffneten Anwendung ausgeführt werden. Durch diese Option wird die Standardkonfiguration in Excel, PowerPoint und Word erzwungen.

* **Makrosicherheitsstufe der Anwendung verwenden**. Die Makrofunktionalität wird von der Einstellung im Bereich „Makroeinstellungen“ des Vertrauensstellungscenters bestimmt.


**Tabelle 1.24. Automatisierungssicherheit**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen

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


Aktiviert (Makrosicherheitsstufe der Anwendung verwenden)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Makros standardmäßig deaktivieren)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1574

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert (Makros standardmäßig deaktivieren)**. Dies könnte zu Funktionalitätseinschränkungen führen, wenn eine externe Anwendung eine 2007 Office-Anwendung programmgesteuert öffnet, um ein Dokument oder eine Vorlage zu öffnen, die Makros enthält.

### Warnung für automatisches Wiederveröffentlichen

Betrifft: **Excel**

Diese Einstellung steuert, ob Excel 2007 vor dem Wiederveröffentlichen einer Arbeitsmappe auf dem World Wide Web eine Warnung anzeigt.

#### Sicherheitsrisiko

Automatisches Wiederveröffentlichen ist eine Funktion in Excel 2007, mit der Arbeitsmappen bei jedem Speichern automatisch neu im World Wide Web veröffentlicht werden können. Für ein erfolgreiches Veröffentlichen der Arbeitsmappe müssen gegebenenfalls die folgenden Änderungen vorgenommen werden:
* Externe Referenzen müssen in Werte umgewandelt werden.

* Ausgeblendete Formeln werden sichtbar.

* Die Option **Genauigkeit wie angezeigt festlegen**, die im Dialogfeld **Excel-Optionen** im Abschnitt **Erweitert** unter der Überschrift **Beim Berechnen dieser Arbeitsmappe** aufgeführt ist, steht nicht mehr zur Verfügung.


Aufgrund dieser Änderungen stimmt die Version auf der Webseite möglicherweise nicht mit der Version der Excel-Datei überein.

Wenn die Funktion für das automatische Wiederveröffentlichen aktiviert ist, wird jedes Mal, wenn der Benutzer eine veröffentlichte Arbeitsmappe speichert, standardmäßig ein Dialogfeld angezeigt. In diesem Dialogfeld kann der Benutzer die Funktion für das automatische Wiederveröffentlichen vorübergehend oder dauerhaft deaktivieren oder **Diese Meldung nicht mehr anzeigen** auswählen, damit das Dialogfeld nicht nach jedem Speichervorgang angezeigt wird. Wenn der Benutzer **Diese Meldung nicht mehr anzeigen** auswählt, werden die Daten nach jedem Speichervorgang weiterhin automatisch wiederveröffentlicht, ohne dass der Benutzer darüber informiert wird.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren bestimmen, ob die Warnung vor dem Veröffentlichen immer oder nie angezeigt werden soll.

**Tabelle 1.25. Warnung für automatisches Wiederveröffentlichen**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Aktiviert (Warnung immer vor dem Veröffentlichen anzeigen)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Warnung immer vor dem Veröffentlichen anzeigen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1334

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Konfiguration für EC- und SSLF-Umgebungen ist **Warnung immer vor dem Veröffentlichen anzeigen**. Diese Konfiguration erzwingt die Standardfunktionalität in Excel 2007 und solle daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

### Signal übertragende Elemente der Benutzeroberfläche für in InfoPath geöffnete Formulare

Betrifft: **InfoPath**

Diese Einstellung steuert, ob InfoPath 2007-Benutzern beim Öffnen eines InfoPath-Formulars, das eine Bedrohung durch Webbeacons enthält, eine Warnung angezeigt wird.

#### Sicherheitsrisiko

Böswillige Benutzer können InfoPath-Formulare mit eingebetteten Webbeacons erstellen, um eine Verbindung mit einem externen Server aufzunehmen, wenn ein Benutzer das Formular öffnet. Dabei könnten Informationen vom Formular gesammelt werden bzw. die vom Benutzer eingegebenen Informationen an einen externen Server gesendet werden, wodurch sie für weitere Angriffe anfällig werden.

Standardmäßig warnt InfoPath 2007 Benutzer vor potenziellen Bedrohungen durch Webbeacons.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen zur Verfügung, über die sie steuern können, wann InfoPath 2007-Benutzer eine Eingabeaufforderung zu Bedrohungen durch Webbeacons erhalten:
* **Signal übertragende Elemente der Benutzeroberfläche nie anzeigen**. InfoPath warnt Benutzer nicht vor potenziellen Bedrohungen durch Webbeacons.

* **Signal übertragende Elemente der Benutzeroberfläche immer anzeigen**. InfoPath warnt Benutzer unabhängig vom Speicherort der Formularvorlage vor potenziellen Bedrohungen durch Webbeacons.

* **Benutzeroberfläche anzeigen, falls die Formularvorlage aus der Internetzone stammt**. InfoPath warnt Benutzer vor potenziellen Bedrohungen durch Webbeacons, wenn sich die Formularvorlage in der Internetsicherheitszone von Internet Explorer befindet.


**Tabelle 1.26. Signal übertragende Elemente der Benutzeroberfläche für in InfoPath geöffnete Formulare**

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


Aktiviert (Benutzeroberfläche anzeigen, falls die Formularvorlage aus der Internetzone stammt)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Signal übertragende Elemente der Benutzeroberfläche immer anzeigen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1290

</td>

</tr>

</table>

#### Auswirkung

Bei Auswahl der empfohlenen Einstellungen für EC- und SSLF-Konfigurationen zeigt InfoPath 2007 Warnungen zu potenziellen Bedrohungen durch Webbeacons an, wenn sich die Formularvorlage in der Internetzone befindet. Außerdem zeigt InfoPath bei Auswahl der empfohlenen Einstellung für die SSLF-Konfiguration Warnungen zu potenziellen Bedrohungen durch Webbeacons selbst dann an, wenn diese aus dem lokalen Intranet stammen. In manchen Fällen werden dem Benutzer beim Öffnen von Formularen daher häufig Warnmeldungen angezeigt.

Es ist möglich, dass einige Formulare vollkommen legitim Signal übertragende Techniken verwenden. In diesem Fall sollten diese Formulare umgestaltet oder Benutzer über die angezeigte Warnmeldung informiert werden.

### Signal übertragende Elemente der Benutzeroberfläche für in InfoPath-Editor-ActiveX geöffnete Formulare

Betrifft: **InfoPath**

Diese Einstellung steuert, ob InfoPath 2007-Benutzern beim Öffnen eines InfoPath-Formularsteuerelements, das eine Bedrohung durch Webbeacons enthält, eine Warnung angezeigt wird.

#### Sicherheitsrisiko

InfoPath 2007 ermöglicht ein Hosten von InfoPath-Formularen als ActiveX-Steuerelemente in anderen Anwendungen. Diese Steuerelemente werden als InfoPath-Formularsteuerelemente bezeichnet.

Ein böswilliger Benutzer könnte einen Webbeacon in eines dieser Steuerelemente einfügen, mit dem beim Öffnen des Formulars durch den Benutzer eine Verbindung mit einem externen Server aufgenommen werden könnte. Dabei könnten Informationen vom Formular gesammelt werden bzw. die vom Benutzer eingegebenen Informationen an einen externen Server gesendet werden, wodurch sie für weitere Angriffe anfällig werden.

Standardmäßig warnen InfoPath-Formularsteuerelemente Benutzer vor potenziellen Bedrohungen durch Webbeacons.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen zur Verfügung, über die sie steuern können, wann Benutzer eine Eingabeaufforderung zu Bedrohungen durch Webbeacons erhalten:
* **Signal übertragende Elemente der Benutzeroberfläche nie anzeigen**. Das InfoPath-Formularsteuerelement warnt Benutzer nicht vor potenziellen Bedrohungen durch Webbeacons.

* **Signal übertragende Elemente der Benutzeroberfläche immer anzeigen**. Das InfoPath-Formularsteuerelement warnt Benutzer unabhängig vom Speicherort der Formularvorlage vor potenziellen Bedrohungen durch Webbeacons.

* **Benutzeroberfläche anzeigen, falls die Formularvorlage aus der Internetzone stammt**. Das InfoPath-Formularsteuerelement warnt Benutzer vor potenziellen Bedrohungen durch Webbeacons, wenn sich die Formularvorlage in der Internetsicherheitszone von Internet Explorer befindet.


**Tabelle 1.27. Signal übertragende Elemente der Benutzeroberfläche für in InfoPath-Editor-ActiveX geöffnete Formulare**

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


Aktiviert (Benutzeroberfläche anzeigen, falls die Formularvorlage aus der Internetzone stammt)

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Aktiviert (Signal übertragende Elemente der Benutzeroberfläche immer anzeigen)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1381

</td>

</tr>

</table>

#### Auswirkung

Bei Auswahl der empfohlenen Einstellungen für EC- und SSLF-Konfigurationen zeigen InfoPath 2007-Formularsteuerelemente Warnungen zu potenziellen Bedrohungen durch Webbeacons an, wenn sich die Formularvorlage in der Internetzone befindet. Außerdem zeigt das Steuerelement bei Auswahl der empfohlenen Einstellung für die SSLF-Konfiguration Warnungen zu potenziellen Bedrohungen durch Webbeacons selbst dann an, wenn diese aus dem lokalen Intranet stammen. In manchen Fällen werden dem Benutzer beim Öffnen von Formularen daher häufig Warnmeldungen angezeigt.

Es ist möglich, dass einige Formulare vollkommen legitim Signal übertragende Techniken verwenden. In diesem Fall sollten diese Formulare umgestaltet oder Benutzer über die angezeigte Warnmeldung informiert werden.

### Öffnen von Konvertern blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Benutzer Dokumente (z. B. WordPerfect-Dokumente) öffnen können, für die mit Word 2007 installierte externe Konverter erforderlich sind.

#### Sicherheitsrisiko

Standardmäßig erlaubt Word 2007 Benutzern das Öffnen einer beliebigen Datei, für die ein entsprechender Konverter installiert ist.

Wenn ein Sicherheitsrisiko für bestimmte Dateiformate entdeckt wird, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen von Dateien in den entsprechenden Formaten gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer keine Dateien öffnen, für die zum Öffnen in Word 2007 ein Konverter erforderlich ist. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf bestimmte Dateitypen abzielen.

**Tabelle 1.28. Öffnen von Konvertern blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


CCE-984

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, Dateien anzuzeigen oder zu bearbeiten, für die zum Öffnen in Word 2007 externe Konverter erforderlich sind. Wenn die Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen und diese Einstellung aktiviert ist, müssen sie ein anderes Tool verwenden, um diese Dateien in ein geeigneteres Format umzuwandeln. Benutzer, die nicht mit Dateien arbeiten, für die externe Konverter erforderlich sind, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Binary 12-Dateitypen blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Benutzer Excel-Arbeitsmappen öffnen können, die Binary 12-Dateitypen wie XLSB-Dateien verwenden.

#### Sicherheitsrisiko

Zusätzlich zu den in der 2007 Microsoft Office-Version veröffentlichten Office Open XML-Dateiformattypen wurde in Excel 2007 ein neues Binärdateiformat mit der Erweiterung XLSB eingeführt. Dieser Dateityp bringt im Vergleich zum XLSX-Dateityp in Office Open XML Leistungsverbesserungen mit sich und eignet sich daher für große, komplexe Arbeitsmappen. Wie bei den Open XML-Formaten in Excel können im Binärformat gespeicherte Dateien Makros enthalten.

Standardmäßig können Benutzer Binary 12-Dateien in Excel öffnen. Wenn ein Sicherheitsrisiko entdeckt wird, das diese Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateien gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer Binary 12 (XLSB)-Dateien in Excel 2007 nicht öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.29. Öffnen von Binary 12-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


CCE-1490

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, Binary 12-Dateien in Excel 2007 anzuzeigen oder zu bearbeiten. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit Binary 12-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Binärdateitypen blockieren

Betrifft: **Excel, PowerPoint, Word**

Diese Einstellung steuert, ob die ausgewählte Anwendung Dokumente öffnen kann, die Binärdateitypen verwenden, etwa solche, die in Office 2003 und früheren Versionen verwendet werden.

#### Sicherheitsrisiko

Binärdateitypen können schädlichen Code enthalten, der möglicherweise schwierig festzustellen ist. Die 2007 Office-Version unterstützt das Office Open XML-Format, mit dem durch schädlichen Code verursachte Probleme umgangen werden können. In manchen Fällen ist die Unterstützung von Binärdateiformaten allerdings erforderlich, um Abwärtskompatibilität mit früheren Versionen bereitzustellen.

Standardmäßig können Benutzer Binärdateiformate in Excel 2007, Word 2007 und PowerPoint 2007 öffnen. Die Dokumente weisen in der Regel die folgenden Dateierweiterungen auf:
* **Excel**. .xls, .xla, .xlt, .xlm, .xlw, .xlb

* **PowerPoint**. .ppt, .pot, .pps, .ppa

* **Word**. .doc, .dot


#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer keine Binärdateien in der ausgewählten Anwendung öffnen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Die Aktivierung dieser Einstellung verhindert nicht, dass Benutzer Dateien im XLSB-Format öffnen, einem neuen mit Excel 2007 eingeführten Binärdateiformat. Unter der Einstellung „Öffnen von Binary 12-Dateitypen blockieren“ in diesem Handbuch finden Sie Informationen dazu, wie Benutzer am Öffnen dieser Dateien gehindert werden können.

**Tabelle 1.30. Öffnen von Binärdateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Öffnen

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm, ppt12.adm, word12.adm

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


**CCE-IDs**

</td>

<td>


Excel: CCE-1512

PowerPoint: CCE-1348

Word: CCE-1654

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für die SSLF-Umgebung hindert Benutzer am Öffnen von Binärdateien, die in Office 2003 und früheren Versionen von Office-Anwendungen erstellt wurden. Viele Unternehmen verwenden diese Dateien nach wie vor bzw. tauschen Dateien mit anderen Unternehmen aus, in denen sie verwendet werden. Wenn Benutzer mit unternehmenswichtigen Office-Binärdateien arbeiten müssen, führt ein Aktivieren dieser Einstellung zu erheblichen Beeinträchtigungen, es sei denn, Sie können diese Dokumente mithilfe eines anderen Tools in geeignetere Formate umwandeln.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Konvertern blockieren

Betrifft: **PowerPoint**

Diese Einstellung steuert, ob PowerPoint 2007-Benutzer PowerPoint-Präsentationen öffnen können, die in Formaten aus PowerPoint-Versionen gespeichert wurden, die älter als PowerPoint 97 sind.

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

In diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103508)   finden Sie weitere Informationen zu dieser Einstellung.

#### Sicherheitsrisiko

Für PowerPoint 2007 ist ein Konvertierungstool erforderlich, um Präsentationen zu öffnen, die in PowerPoint-Versionen vor PowerPoint 97 gespeichert wurden, z. B. PowerPoint 95, PowerPoint 4.0 und andere.

Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können PowerPoint 2007-Benutzer keine Konverter zum Öffnen von Präsentationen verwenden, die in PowerPoint-Versionen vor PowerPoint 97 gespeichert wurden. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.31. Öffnen von Konvertern blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


ppt12.adm

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


CCE-1216

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung könnte zu unerwarteten Beeinträchtigungen führen, wenn Benutzer mit PowerPoint-Präsentationen arbeiten, an denen über Jahre hinweg keine Änderungen vorgenommen wurden, beispielsweise aus Dokumentarchiven oder alten Sicherungskopien. Berücksichtigen Sie beim Konfigurieren dieser Einstellung, ob Benutzer in Zukunft Zugriff auf solche Dateien benötigen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von DIF- und SYLK-Dateitypen blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Excel 2007 Dateien öffnen kann, die Dateitypen im Datenaustauschformat (Data Interchange Format, DIF) und Format für symbolische Verknüpfungen (Symbolic Link Format, SYLK) verwenden.

#### Sicherheitsrisiko

Bei DIF und SYLK handelt es sich um Nur-Text-Dateiformate, die zum Datenaustausch zwischen verschiedenen Anwendungen wie Excel 2007 verwendet werden. Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

Standardmäßig können Benutzer DIF- (.dif) und SYLK (.slk)-Dateien in Excel öffnen.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer DIF- und SYLK-Dateien in Excel 2007 nicht öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.32. Öffnen von DIF- und SYLK-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


CCE-554

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, DIF- und SYLK-Dateien in Excel 2007 anzuzeigen oder zu ändern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit DIF- oder SYLK-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Dateien mit früherer Version als der folgenden blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Word 2007-Benutzer Dokumente öffnen können, die in früheren Versionen von Word erstellt wurden.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer keine Dateien öffnen, die in einem Format vor Word 6.0 gespeichert wurden.

Wenn ein Sicherheitsrisiko entdeckt wird, das ältere Versionen des Word-Dateiformats betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, wird ein Dropdownmenü angezeigt, in dem die verschiedenen Word-Versionen in ungefährer chronologischer Reihenfolge angezeigt werden:
* Word 1.x für Windows

* Word 4.x für Macintosh

* Word 1.2 für Windows Japan

* Word 1.2 für Windows Korea

* Word 5.x für Macintosh

* Word 1.2 für Windows Taiwan

* Word 2.x für Windows

* Word 2.0 für Windows BiDi

* Word 2.0 für Windows Japan

* Word 2.0 für Windows Korea

* Word 2.0 für Windows Taiwan

* Word 6.0 für Windows

* Word 6.0 für Macintosh

* Word 95 veröffentlicht

* Word 95 Beta

* Word 97 für Windows

* Word 98 für Macintosh

* Word 2001 für Macintosh

* Word X für Macintosh

* Word 2000

* Word 2002

* Word 2003

* Word 2004 für Macintosh

* Word 2003 wie von Word 2007 gespeichert


Durch Auswahl einer Version aus dieser Liste wird in Word 2007 das Öffnen von Dateien blockiert, die in Versionen gespeichert sind, die in der Liste vor der angegebenen Versionen aufgeführt sind. Dateien mit weiter unten in der Liste angezeigten Versionen können geöffnet werden. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.33. Öffnen von Dateien mit früherer Version als der folgenden blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


Aktiviert (Word 2003 wie von Word 2007 gespeichert)

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1371

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung könnte zu unerwarteten Beeinträchtigungen führen, wenn Benutzer mit Word-Dokumenten arbeiten, an denen über Jahre hinweg keine Änderungen vorgenommen wurden, beispielsweise aus Dokumentarchiven oder alten Sicherungskopien. Berücksichtigen Sie beim Konfigurieren dieser Einstellung, ob Benutzer in Zukunft Zugriff auf solche Dokumente benötigen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Vorabversionen neuer Excel 2007-Dateiformate blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Excel 2007-Benutzer Open XML-Dateien öffnen können, die mit Vorabversionen von Excel 2007 gespeichert wurden.

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht in allen Fällen erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103509)  .

#### Sicherheitsrisiko

Benutzer können standardmäßig Dateien öffnen, die mit Vorabversionen des neuen Office Open XML-Formats gespeichert wurden. An diesem Format wurden vor der endgültigen Veröffentlichung von Excel 2007 kleinere Änderungen vorgenommen. Excel Open XML-Dateien weisen in der Regel die folgenden Dateierweiterungen auf:
* .xlsb

* .xlsx

* .xlsm

* .xltx

* .xltm

* .xlam


Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

Diese Dateitypen sind in Excel 2007 standardmäßig nicht blockiert.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Excel 2007-Benutzer keine Open XML-Dateien öffnen, die in Vorabversionen von Excel 2007 erstellt wurden. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.34. Öffnen von Vorabversionen neuer Excel 2007-Dateiformate blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


CCE-1331

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung könnte zu unerwarteten Beeinträchtigungen führen, wenn sich Ihr Unternehmen an einer Betabereitstellung der 2007 Microsoft Office-Version beteiligt hat. Wenn Ihr Unternehmen keine Beta- oder Releasekandidatversion von Excel 2007 bereitgestellt hat, sollte diese Einstellung für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von HTML- und XMLSS-Dateitypen blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Benutzer HTML- und XMLSS-Dateien in Excel 2007 öffnen können.

#### Sicherheitsrisiko

Standardmäßig können Benutzer mit Excel 2007 HTML- und XML Spreadsheet 2003 (XMLSS)-Dateien öffnen, die in der Regel die folgenden Dateierweiterungen aufweisen:
* .mht

* .mhtml

* .htm

* .html

* .xml

* .xmlss


Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer HTML- oder XMLSS-Dateien in Excel 2007 nicht öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.35. Öffnen von HTML- und XMLSS-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


CCE-1543

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, HTML- und XMLSS-Dateien in Excel 2007 anzuzeigen oder zu ändern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit HTML- und XMLSS-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von HTML-Dateitypen blockieren

Betrifft: **PowerPoint, Word**

Diese Einstellung steuert, ob Benutzer HTML-Dateien in den angegebenen Anwendungen öffnen können.

#### Sicherheitsrisiko

Standardmäßig können Benutzer mit PowerPoint 2007 und Word 2007 HTML-Dateien öffnen, die in der Regel die folgenden Dateierweiterungen aufweisen:
* .htm

* .html

* .mht

* .mhtml


Wenn ein Sicherheitsrisiko entdeckt wird, das HTML-Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen von HTML-Dateien gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer HTML-Dateien in keiner der angegebenen Anwendungen öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.36. Öffnen von HTML-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Öffnen

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


ppt12.adm, word12.adm

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


**CCE-IDs**

</td>

<td>


PowerPoint: CCE-1644

Word: CCE-1160

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, HTML-Dateien in Word 2007 und PowerPoint 2007 anzuzeigen oder zu bearbeiten. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit HTML-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen interner Dateitypen blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Word 2007-Benutzer Binärdateien öffnen können, die in Vorabversionen von Word gespeichert wurden.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer Word-Binärdateien (DOC und DOT) öffnen, die in Beta- oder Vorabversionen von Word gespeichert wurden, einschließlich Vorabversionen von Word 2007. Wenn ein Sicherheitsrisiko für diese Dateien entdeckt wird, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Word 2007-Benutzer keine binären Word-Dokumente öffnen, die mit Vorabversionen von Word gespeichert wurden. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.37. Öffnen interner Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


CCE-1503

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung kann zu unerwarteten Beeinträchtigungen führen, wenn die Benutzer in Ihrem Unternehmen in der Vergangenheit an einem Microsoft-Betaprogramm teilgenommen haben. Wenn Ihr Unternehmen noch nie Betaversionen von Word bereitgestellt hat, sollte diese Einstellung für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Open XML-Dateitypen blockieren

Betrifft: **Excel, PowerPoint, Word**

Diese Einstellung steuert, ob Benutzer Office Open XML-Dateien in den angegebenen Anwendungen öffnen können.

#### Sicherheitsrisiko

Die in der 2007 Microsoft Office-Version eingeführten Office Open XML-Dateiformattypen bieten im Vergleich zu den in Office 2003 unterstützten Binärdateitypen eine Reihe von Vorteilen, darunter das Potenzial, die Auswirkungen von schädlichem Code zu verringern. Dateien können als unfähig zur Ausführung von Code identifiziert werden und ignorieren daher eingebetteten Code. Außerdem lassen sich Dateien mit eingebettetem Code leichter identifizieren. Office Open XML-Dateien weisen in der Regel die folgenden Dateierweiterungen auf:
* **Excel**. .xlsx, .xlsm, .xltx, .xltm, .xlam

* **PowerPoint**. .pptx, .pptm, .potx, .potm, .ppsx, .ppsm, .ppam, .thmx, .xml

* **Word**. .docx, .docm, .dotx, .dotm, .xml


Wenn ein Sicherheitsrisiko entdeckt wird, das Office Open XML-Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer Open XML-Dateien in den angegebenen Anwendungen nicht öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.38. Öffnen von Open XML-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Öffnen

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm, ppt12.adm, word12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Deaktiviert

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


**CCE-IDs**

</td>

<td>


Excel: CCE-1468

PowerPoint: CCE-1701

Word: CCE-1504

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, Office Open XML-Dateien in den angegebenen Anwendungen anzuzeigen oder zu bearbeiten. Office Open XML ist das Standardformat der 2007 Microsoft Office-Version. Mit steigender Nutzung der 2007 Microsoft Office-Version und ihrer Nachfolger wird sich diese Art von Dateien immer mehr verbreiten.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Gliederungen blockieren

Betrifft: **PowerPoint**

Diese Einstellung steuert, ob Benutzer Nicht-PowerPoint-Dateien als Gliederungen in PowerPoint 2007 öffnen können.

#### Sicherheitsrisiko

Standardmäßig können Benutzer Präsentationsgliederungen in anderen Anwendungen erstellen und sie in PowerPoint 2007 als Gliederungsdateien öffnen. PowerPoint kann Gliederungsdateien mit den folgenden Dateierweiterungen öffnen:
* .rtf

* .txt

* .doc

* .wpd

* .docx

* .docm

* .wps


Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer keine Gliederungsdateien mit den aufgeführten Dateierweiterungen öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.39. Öffnen von Gliederungen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


ppt12.adm

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


CCE-1194

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung hat erhebliche Auswirkungen auf Benutzer, die daran gewöhnt sind, PowerPoint-Präsentationsgliederungen in anderen Programmen zu erstellen. Diese Benutzer müssen Gliederungen innerhalb von PowerPoint 2007 erstellen. Andere Benutzer sind von dieser Einstellung nicht betroffen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Vorabversionen neuer Excel 2007-Dateiformate über das Compatibility Pack für 2007 Office System und den Excel 2007-Konverter blockieren

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Benutzer mit dem Microsoft Office Compatibility Pack für Word-, Excel- und PowerPoint 2007-Dateiformate Office Open XML-Dateien öffnen können, die mit Vorabversionen von Excel 2007 gespeichert wurden.

#### Sicherheitsrisiko

Das Microsoft Office Compatibility Pack für Word-, Excel- und PowerPoint 2007-Dateiformate ermöglicht Benutzern von Microsoft Excel 2000, Microsoft Excel 2002 und Microsoft Office Excel 2003 das Öffnen von Dateien, die im Office Open XML-Format von Excel 2007 gespeichert sind. Excel Open XML-Dateien weisen in der Regel die folgenden Dateierweiterungen auf:
* .xlsx

* .xlsm

* .xltx

* .xltm

* .xlam


Standardmäßig werden mit dem Compatibility Pack keine Dateien geöffnet, die in Vorabversionen des neuen Office Open XML-Formats gespeichert wurden. An diesem Format wurden vor der endgültigen Veröffentlichung von Excel 2007 kleinere Änderungen vorgenommen. Wenn diese Konfiguration durch eine Änderung in der Registrierung oder eine andere Methode geändert wird, können Benutzer mit installiertem Compatibility Pack Dateien öffnen, die mit bestimmten Vorabversionen von Excel gespeichert wurden, mit anderen Versionen gespeicherte dagegen nicht. Dies führt zu einer inkonsistenten Dateiöffnungsfunktionalität.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer des Compatibility Pack keine Office Open XML-Dateien öffnen, die in Vorabversionen von Excel 2007 erstellt wurden.

**Tabelle 1.40. Öffnen von Vorabversionen neuer Excel 2007-Dateiformate über das Compatibility Pack für 2007 Office System und den Excel 2007-Konverter blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Office 2007-Konverter

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


Aktiviert

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


CCE-1431

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Vorabversionen neuer PowerPoint 2007-Dateiformate blockieren

Betrifft: **PowerPoint**

Diese Einstellung steuert, ob PowerPoint 2007-Benutzer Open XML-Dateien öffnen können, die mit Vorabversionen von PowerPoint 2007 gespeichert wurden.

#### Sicherheitsrisiko

Standardmäßig können PowerPoint 2007-Benutzer Dateien öffnen, die mit Vorabversionen des neuen Office Open XML-Formats gespeichert wurden. An diesem Format wurden vor der endgültigen Veröffentlichung von PowerPoint 2007 kleinere Änderungen vorgenommen. PowerPoint Open XML-Dateien weisen in der Regel die folgenden Dateierweiterungen auf:
* .pptx

* .pptm

* .potx

* .potm

* .ppsx

* .ppsm

* .ppam

* .thmx

* .xml


Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können PowerPoint 2007-Benutzer keine Open XML-Dateien öffnen, die in Vorabversionen von PowerPoint 2007 erstellt wurden. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.41. Öffnen von Vorabversionen neuer PowerPoint 2007-Dateiformate blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


ppt12.adm

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


CCE-1688

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung könnte zu unerwarteten Beeinträchtigungen führen, wenn sich Ihr Unternehmen an einer Betabereitstellung der 2007 Microsoft Office-Version beteiligt hat. Wenn Ihr Unternehmen keine Beta- oder Releasekandidatversion von PowerPoint 2007 bereitgestellt hat, sollte diese Einstellung für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Vorabversionen neuer PowerPoint 2007-Dateiformate über das Compatibility Pack für 2007 Office System und den PowerPoint 2007-Konverter blockieren

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Benutzer mit dem Microsoft Office Compatibility Pack für Word-, Excel- und PowerPoint 2007-Dateiformate Office Open XML-Dateien öffnen können, die mit Vorabversionen von PowerPoint 2007 gespeichert wurden.

#### Sicherheitsrisiko

Das Microsoft Office Compatibility Pack für Word-, Excel- und PowerPoint 2007-Dateiformate ermöglicht Benutzern von Microsoft PowerPoint 2000, PowerPoint 2002 und Office PowerPoint 2003 das Öffnen von Dateien, die im Office Open XML-Format von PowerPoint 2007 gespeichert sind. PowerPoint Open XML-Dateien weisen in der Regel die folgenden Dateierweiterungen auf:
* .pptx

* .pptm

* .potx

* .potm

* .ppsx

* .ppsm

* .ppam

* .thmx

* .xml


Standardmäßig werden mit dem Compatibility Pack keine Dateien geöffnet, die in Vorabversionen des neuen Office Open XML-Formats gespeichert wurden. An diesem Format wurden vor der endgültigen Veröffentlichung von PowerPoint 2007 kleinere Änderungen vorgenommen. Wenn diese Konfiguration durch eine Änderung in der Registrierung oder eine andere Methode geändert wird, können Benutzer mit installiertem Compatibility Pack Dateien öffnen, die mit bestimmten Vorabversionen von PowerPoint gespeichert wurden, mit anderen Versionen gespeicherte dagegen nicht. Dies führt zu einer inkonsistenten Dateiöffnungsfunktionalität.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer des Compatibility Pack keine Office Open XML-Dateien öffnen, die in Vorabversionen von PowerPoint 2007 erstellt wurden.

**Tabelle 1.42. Öffnen von Vorabversionen neuer PowerPoint 2007-Dateiformate über das Compatibility Pack für 2007 Office System und den PowerPoint 2007-Konverter blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Office 2007-Konverter

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


Aktiviert

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


CCE-1594

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Vorabversionen neuer Word 2007-Dateiformate blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Word 2007-Benutzer Open XML-Dateien öffnen können, die mit Vorabversionen von Word 2007 gespeichert wurden.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer Dateien öffnen, die mit Vorabversionen des neuen Office Open XML-Formats gespeichert wurden. An diesem Format wurden vor der endgültigen Veröffentlichung von Microsoft Office Word 2007 kleinere Änderungen vorgenommen. Word Open XML-Dateien weisen in der Regel die folgenden Dateierweiterungen auf:
* .docx

* .docm

* .dotx

* .dotm

* .xml


Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Word 2007-Benutzer keine Open XML-Dateien öffnen, die in Vorabversionen von Word 2007 erstellt wurden. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.43. Öffnen von Vorabversionen neuer Word 2007-Dateiformate blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


CCE-1746

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung könnte zu unerwarteten Beeinträchtigungen führen, wenn sich Ihr Unternehmen an einer Betabereitstellung der 2007 Microsoft Office-Version beteiligt hat. Wenn Ihr Unternehmen keine Beta- oder Releasekandidatversion von Word 2007 bereitgestellt hat, sollte diese Einstellung für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Vorabversionen neuer Word 2007-Dateiformate über das Compatibility Pack für 2007 Office System und den Word 97-2003/Open XML-Formatkonverter blockieren

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Benutzer mit dem Microsoft Office Compatibility Pack für Word-, Excel- und PowerPoint 2007-Dateiformate Office Open XML-Dateien speichern können, die mit Vorabversionen von Word 2007 gespeichert wurden.

#### Sicherheitsrisiko

Das Microsoft Office Compatibility Pack für Word-, Excel- und PowerPoint 2007-Dateiformate ermöglicht Benutzern von Microsoft Word 2000, Word 2002 und Office Word 2003 das Öffnen von Dateien, die im Office Open XML-Format von Word 2007 gespeichert sind. Word Open XML-Dateien weisen in der Regel die folgenden Dateierweiterungen auf:
* .docx

* .docm

* .dotx

* .dotm

* .xml


Standardmäßig werden mit dem Compatibility Pack keine Dateien geöffnet, die in Vorabversionen des neuen Office Open XML-Formats gespeichert wurden. An diesem Format wurden vor der endgültigen Veröffentlichung von Word 2007 kleinere Änderungen vorgenommen. Wenn diese Konfiguration durch eine Änderung in der Registrierung oder eine andere Methode geändert wird, können Benutzer mit installiertem Compatibility Pack Dateien öffnen, die von bestimmten Vorabversionen von Word gespeichert wurden, andere dagegen nicht. Dies führt zu einer inkonsistenten Dateiöffnungsfunktionalität.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer des Compatibility Pack keine Office Open XML-Dateien öffnen, die in Vorabversionen von Word 2007 erstellt wurden.

**Tabelle 1.44. Öffnen von Vorabversionen neuer Word 2007-Dateiformate über das Compatibility Pack für 2007 Office System und den Word 97-2003/Open XML-Formatkonverter blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Office 2007-Konverter

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


Aktiviert

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


CCE-1549

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung setzt die Standardkonfiguration durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von RTF-Dateitypen blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Benutzer Dateien im RTF-Format (Rich Text Format) in Word 2007 öffnen können.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer RTF-Dateien öffnen. RTF wurde für eine einfache Übertragung formatierter Dokumente zwischen unterschiedlichen Anwendungen entwickelt. RTF-Dateien weisen in der Regel die Dateierweiterung .rtf auf.

Wenn ein Sicherheitsrisiko entdeckt wird, das RTF-Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen von RTF-Dateien gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer RTF-Dateien in Word 2007 nicht öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.45. Öffnen von RTF-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


CCE-1579

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, RTF-Dateien in Word 2007 anzuzeigen oder zu bearbeiten. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit RTF-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Textdateitypen blockieren

Betrifft: **Excel, Word**

Diese Einstellung steuert, ob Benutzer Textdateien in den angegebenen Anwendungen öffnen können.

#### Sicherheitsrisiko

Standardmäßig können Word 2007- und Excel 2007-Benutzer Textdateien öffnen, die in der Regel die Dateierweiterung .txt aufweisen. Excel-Benutzer können dazu textbasierte, durch Kommas getrennte CSV- und Druckerdateien öffnen, die normalerweise die Dateierweiterungen .csv und .prn aufweisen. Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieser Dateiformate gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer keine Textdateien in den angegebenen Anwendungen öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.46. Öffnen von Textdateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm, word12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-IDs**

</td>

<td>


Excel: CCE-1415

Word: CCE-1072

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, Textdateien in den ausgewählten Anwendungen anzuzeigen oder zu bearbeiten. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit Textdateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von Word 2003-XML-Dateitypen blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Word 2007-Benutzer Dateien öffnen können, die im XML-Format von Word 2003 gespeichert wurden.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer Dateien öffnen, die im mit Microsoft Office Word 2003 eingeführten WordprocessingML-Dateiformat gespeichert wurden. WordprocessingML-Dokumente weisen in der Regel die Dateierweiterung .xml auf.

Wenn ein Sicherheitsrisiko entdeckt wird, das diese Art von Dateien betrifft, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen dieses Dateiformats gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Word 2007-Benutzer keine Word 2003 WordprocessingML-Dateien öffnen. Die Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.47. Öffnen von Word 2003-XML-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


CCE-958

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, WordprocessingML-Dateien in Word 2007 anzuzeigen oder zu bearbeiten. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit WordprocessingML-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von XLL-Dateitypen blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Benutzer XLL-Add-In-Dateien in Excel 2007 öffnen können.

#### Sicherheitsrisiko

Standardmäßig können Benutzer XLL-Add-In-Dateien öffnen und Excel 2007 so um zusätzliche Funktionen erweitern. XLL-Dateien weisen in der Regel die Dateierweiterung .xll auf. XLL-Dateien enthalten Code. Daher könnte eine von einem Angreifer erstellte XLL-Datei den Computer des Benutzers bzw. die darauf enthaltenen Daten gefährden.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer XLL-Dateien in Excel 2007 nicht öffnen.

**Tabelle 1.48. Öffnen von XLL-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


CCE-1437

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, XLL-Add-Ons in Excel 2007 zu laden. Wenn Ihr Unternehmen unternehmenswichtige XLL-Add-Ons verwendet, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die keine XLL-Add-Ons laden, sind von dieser Einstellung nicht betroffen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Öffnen von XML-Dateitypen blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Benutzer XML-Dateien in Excel 2007 öffnen können.

#### Sicherheitsrisiko

Standardmäßig können Benutzer Extensible Markup Language (XML)-Dateien in Excel 2007 öffnen. Diese Dateien weisen normalerweise die Dateierweiterung .xml auf. Wenn ein Sicherheitsrisiko für diese Dateien entdeckt wird, können Sie Ihr Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, da Benutzer vorübergehend so lange am Öffnen von XML-Dateien gehindert werden, bis ein Sicherheitspatch verfügbar ist.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer XML-Dateien in Excel 2007 nicht öffnen. Diese Einstellung kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf spezifische Dateitypen abzielen.

**Tabelle 1.49. Öffnen von XML-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Öffnen

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


CCE-1195

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, XML-Dateien in Excel 2007 anzuzeigen oder zu bearbeiten. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit XML-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von DIF- und SYLK-Dateitypen blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Benutzer die Dateitypen DIF und SYLK in Excel 2007 speichern können.

#### Sicherheitsrisiko

Bei Dateien im Datenaustauschformat (Data Interchange Format, DIF) und im Format für symbolische Verknüpfungen (Symbolic Link Format, SYLK) handelt es sich um Nur-Text-Dateiformate, die zum Austausch von Daten zwischen verschiedenen Anwendungen, z. B. Excel 2007, verwendet werden. Wenn eine DIF- oder SYLK-Datei mit anderen Benutzern gemeinsam verwendet wird, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, kann ein effektiver Informationsaustausch behindert werden.

Standardmäßig können Benutzer Dateien mit den Dateierweiterungen .dif und .sylk in Excel speichern.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer DIF- oder SYLK-Dateien in Excel 2007 nicht speichern.

**Tabelle 1.50. Speichern von DIF- und SYLK-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-IDCCE-ID**

</td>

<td>


CCE-573

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, DIF- und SYLK-Dateien in Excel 2007 zu speichern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit DIF- oder SYLK-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

Berücksichtigen Sie bei der Entscheidung, ob diese Einstellung aktiviert werden soll, die Konfiguration der Einstellung „Öffnen von DIF- und SYLK-Dateitypen blockieren“. Wenn „Öffnen von DIF- und SYLK-Dateitypen blockieren“ aktiviert und diese Einstellung deaktiviert oder nicht konfiguriert ist, können Benutzer Dateien in einem Format speichern, das sie nicht öffnen können. Dadurch kann möglicherweise auf wichtige Daten nicht mehr zugegriffen werden.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Binärdateitypen blockieren

Betrifft: **Excel, PowerPoint, Word**

Diese Einstellung steuert, ob die angegebenen Anwendungen Dokumente speichern können, die Binärdateitypen verwenden, etwa solche, die in Office 2003 und früheren Versionen verwendet werden.

#### Sicherheitsrisiko

Die 2007 Office-Version unterstützt das Office Open XML-Format, mit dem durch schädlichen Code verursachte Probleme umgangen werden können. In manchen Fällen ist die Unterstützung von Binärdateiformaten allerdings erforderlich, um Abwärtskompatibilität mit früheren Versionen bereitzustellen.

Standardmäßig können Benutzer Binärdateiformate mit den folgenden Dateierweiterungen in Excel 2007, Word 2007 und PowerPoint 2007 speichern:
* **Excel**. .xls, .xla, .xlt

* **PowerPoint**. .ppt, .pot, .pps, .ppa

* **Word**. .doc, .dot

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Die in der administrativen Vorlagendatei in Excel 2007 bereitgestellte Beschreibung für diese Einstellung enthält eine fehlerhafte Liste der blockierten Dateitypen. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103933)  .

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer keine Binärdateien in den angegebenen Anwendungen speichern.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Die Aktivierung dieser Einstellung verhindert nicht, dass Benutzer Dateien im XLSB-Format speichern, einem neuen mit Excel 2007 eingeführten Binärdateiformat. Unter der Einstellung „Speichern von Binary12-Dateitypen blockieren“ in diesem Handbuch finden Sie Informationen dazu, wie Benutzer am Speichern dieser Dateien gehindert werden.

**Tabelle 1.51. Speichern von Binärdateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Speichern

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Speichern

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm, ppt12.adm, word12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-IDs**

</td>

<td>


Excel: CCE-562

PowerPoint: CCE-1136

Word: CCE-1684

</td>

</tr>

</table>

#### Auswirkung

Viele Unternehmen verwenden diese Dateien nach wie vor bzw. tauschen Dateien mit anderen Unternehmen aus, in denen sie verwendet werden. Wenn Benutzer mit unternehmenswichtigen Office-Binärdateien arbeiten müssen, führt ein Aktivieren dieser Einstellung zu erheblichen Beeinträchtigungen, es sei denn, Sie können diese Dokumente mithilfe eines anderen Tools in geeignetere Formate umwandeln.

Berücksichtigen Sie bei der Entscheidung, ob diese Einstellung aktiviert werden soll, die Konfiguration der Einstellung „Öffnen von Binärdateitypen blockieren“ für die angegebene Anwendung. Wenn „Öffnen von Binärdateitypen blockieren“ aktiviert und diese Einstellung deaktiviert oder nicht konfiguriert ist, können Benutzer Dateien in einem Format speichern, das sie nicht öffnen können. Dadurch kann möglicherweise auf wichtige Daten nicht mehr zugegriffen werden.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Binary12-Dateitypen blockieren

Betrifft: **Excel**

Diese Einstellung steuert, ob Benutzer Excel-Arbeitsmappen öffnen können, die im Binary 12-Dateiformat gespeichert wurden (und die Dateierweiterung *.xlsb aufweisen).

#### Sicherheitsrisiko

Zusätzlich zu den in der 2007 Microsoft Office-Version veröffentlichten Office Open XML-Dateiformattypen wurde in Excel 2007 ein neues Binärdateiformat mit der Erweiterung XLSB eingeführt. Dieser Dateityp bringt im Vergleich zum XLSX-Dateityp von Office Open XML Leistungsverbesserungen mit sich und eignet sich daher für große, komplexe Arbeitsmappen. Wie bei den Open XML-Formaten in Excel 2007 können im Binärformat gespeicherte Dateien Makros enthalten.

Wenn Dateien dieser Art mit anderen Benutzern gemeinsam verwendet werden, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Excel 2007-Benutzer Dateien mit der Erweiterung .xlsb nicht speichern.

**Tabelle 1.52. Speichern von Binary12-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1098

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, XLSB-Dateien in Excel 2007 zu speichern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit XLSB-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

Berücksichtigen Sie bei der Entscheidung, ob diese Einstellung aktiviert werden soll, die Konfiguration der Einstellung „Öffnen von Binary 12-Dateitypen blockieren“. Wenn „Öffnen von Binary 12-Dateitypen blockieren“ aktiviert und diese Einstellung deaktiviert oder nicht konfiguriert ist, können Benutzer Dateien in einem Format speichern, das sie nicht öffnen können. Dadurch kann möglicherweise auf wichtige Daten nicht mehr zugegriffen werden.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Konvertern blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Benutzer Dokumente in Formaten speichern können, für die externe, in der 2007 Office-Version verfügbare Word-Konverter erforderlich sind.

#### Sicherheitsrisiko

Standardmäßig erlaubt Word 2007 Benutzern das Speichern einer Datei in einem beliebigen Format, für das ein entsprechender Konverter installiert ist.

Wenn eine mit einem Konverter gespeicherte Datei gemeinsam mit anderen Benutzern verwendet wird, die aufgrund technischer oder Richtlinienbeschränkungen diese Datei nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Word 2007-Benutzer keine Dateien in Formaten speichern, für die ein Konverter erforderlich ist.

**Tabelle 1.53. Speichern von Konvertern blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1231

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, Dateien in Formaten zu speichern, für die zum Öffnen in Word 2007 externe Konverter erforderlich sind. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen und diese Einstellung aktiviert ist, müssen sie ein anderes Tool verwenden, um diese Dateien in ein geeigneteres Format umzuwandeln. Benutzer, die nicht mit Dateien arbeiten, für die externe Konverter erforderlich sind, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Grafikfiltern blockieren

Betrifft: **PowerPoint**

Diese Einstellung steuert, ob Benutzer PowerPoint 2007-Präsentationen als Grafikdateien speichern können.

#### Sicherheitsrisiko

Standardmäßig können PowerPoint 2007-Benutzer Präsentationen als Grafikdateien in den folgenden Formaten speichern (die Dateierweiterungen sind in Klammern angegeben):
* JPEG (.jpg)

* PNG (.png)

* TIFF (.tif)

* Bitmap (.bmp)

* Windows Metafile (.wmf)

* Enhanced Metafile (.emf)


Wenn Grafikdateien dieser Art mit anderen Benutzern gemeinsam verwendet werden, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer PowerPoint 2007-Präsentationen nicht als Grafikdateien speichern.

**Tabelle 1.54. Speichern von Grafikfiltern blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


ppt12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1722

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung ergeben sich Beeinträchtigungen für Benutzer, die PowerPoint 2007-Präsentationen als Grafikdateien speichern. Andere Benutzer sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von HTML- und XMLSS-Dateitypen blockieren

Betrifft: **Excel**

Diese Richtlinie steuert, ob Excel 2007-Benutzer Excel-Arbeitsmappen als HTML- oder XMLSS-Dateien speichern können.

#### Sicherheitsrisiko

Standardmäßig ermöglicht Excel Benutzern das Speichern von HTML- und XML Spreadsheet 2003 (XMLSS)-Dateien, die die folgenden Dateierweiterungen aufweisen:
* .mht

* .mhtml

* .htm

* .html

* .xml

* .xmlss


Wenn Dateien dieser Art mit anderen Benutzern gemeinsam verwendet werden, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer Dateien in den Formaten HTML oder XMLSS in Excel 2007 nicht speichern.

**Tabelle 1.55. Speichern von HTML- und XMLSS-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1507

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, HTML- und XMLSS-Dateien in Excel 2007 zu speichern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit HTML- und XMLSS-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von HTML-Dateitypen blockieren

Betrifft: **PowerPoint, Word**

Diese Einstellung steuert, ob Benutzer Dokumente im HTML-Format in den angegebenen Anwendungen speichern können.

#### Sicherheitsrisiko

Standardmäßig ist in PowerPoint 2007 und Word 2007 ein Speichern von Dateien im HTML-Format mit den folgenden Dateierweiterungen möglich:
* .mht

* .mhtml

* .htm

* .html


Wenn Dateien dieser Art mit anderen Benutzern gemeinsam verwendet werden, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer in den angegebenen Anwendungen keine Dateien im HTML-Format speichern.

**Tabelle 1.56. Speichern von HTML-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Speichern

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


ppt12.adm, word12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-IDs**

</td>

<td>


PowerPoint: CCE-1766

Word: CCE-1675

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, HTML-Dateien in Word 2007 und PowerPoint 2007 zu speichern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit HTML-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Open XML-Dateitypen blockieren

Betrifft: **Excel, PowerPoint, Word**

Diese Einstellung steuert, ob Benutzer der angegebenen Anwendungen Dokumente im Office Open XML-Dateiformat speichern können.

#### Sicherheitsrisiko

Die in der 2007 Microsoft Office-Version eingeführten Office Open XML-Dateiformattypen bieten im Vergleich zu den in Office 2003 unterstützten Binärdateitypen eine Reihe von Vorteilen, darunter das Potenzial, die Auswirkungen von schädlichem Code zu verringern. Dateien können als unfähig zur Ausführung von Code identifiziert werden und ignorieren daher eingebetteten Code. Außerdem lassen sich Dateien mit eingebettetem Code leichter identifizieren.

Für Benutzer, die ältere Versionen dieser Anwendungen ausführen, bietet Microsoft das [Microsoft Office Compatibility Pack für Word-, Excel- und PowerPoint 2007-Dateiformate](http://www.microsoft.com/downloads/details.aspx?familyid=941b3470-3ae9-4aee-8f43-c6bb74cd1466&amp;displaylang=en)  , das ein Öffnen und Speichern von Open XML-Dateien ermöglicht. Das Compatibility Pack kann mit den folgenden Microsoft Office-Programmen verwendet werden:
* Word 2000 mit Service Pack 3, Excel 2000 mit Service Pack 3 und PowerPoint 2000 mit Service Pack 3

* Word 2002 mit Service Pack 3, Excel 2002 mit Service Pack 3 und PowerPoint 2002 mit Service Pack 3

* Word 2003 mit mindestens Service Pack 1, Excel 2003 mit mindestens Service Pack 1 und PowerPoint 2003 mit mindestens Service Pack 1

* Microsoft Office Word 2003 Viewer

* Microsoft Office Excel 2003 Viewer

* Microsoft Office PowerPoint Viewer 2003 Viewer


Wenn Benutzer aus bestimmten Gründen Dateien im Office Open XML-Format nicht speichern können, können sie die Sicherheitsvorteile der neuen Dateitypen nicht nutzen.

#### Gegenmaßnahme

Wenn diese Einstellung **deaktiviert** ist, können Benutzer Dateien im Office Open XML-Format in den angegebenen Anwendungen speichern.

**Tabelle 1.57. Speichern von Open XML-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Speichern

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Speichern

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm, ppt12.adm, word12.adm

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (EC)**

</td>

<td>


Deaktiviert

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


**CCE-IDs**

</td>

<td>


Excel: CCE-1446

PowerPoint: CCE-1506

Word: CCE-1019

</td>

</tr>

</table>

#### Auswirkung

Office Open XML ist das Standardformat in der 2007 Microsoft Office-Version. Ein Deaktivieren dieser Einstellung sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Gliederungen blockieren

Betrifft: **PowerPoint**

Diese Einstellung steuert, ob Benutzer PowerPoint 2007-Präsentationen als Gliederungen in Nicht-PowerPoint-Formaten speichern können.

#### Sicherheitsrisiko

Standardmäßig können PowerPoint 2007-Benutzer Präsentationen als Gliederungen speichern, die in anderen Anwendungen geöffnet werden können. PowerPoint kann Gliederungsdateien mit den folgenden Dateierweiterungen speichern:
* .rtf

* .txt

* .doc

* .wpd

* .docx

* .docm

* .wps


Wenn Dateien dieser Art mit anderen Benutzern gemeinsam verwendet werden, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer PowerPoint 2007-Präsentationen nicht als Gliederungsdateien mit den aufgeführten Erweiterungen speichern.

**Tabelle 1.58. Speichern von Gliederungen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


ppt12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1180

</td>

</tr>

</table>

#### Auswirkung

Die Aktivierung dieser Einstellung hat erhebliche Auswirkungen auf Benutzer, die daran gewöhnt sind, PowerPoint 2007-Präsentationen als Gliederungen zu speichern, die in anderen Programmen geöffnet werden können. Diese Benutzer müssen Gliederungen innerhalb des Zielprogramms selbst erstellen. Andere Benutzer sind von dieser Einstellung nicht betroffen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von RTF-Dateitypen blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Benutzer Dateien im RTF-Format in Microsoft Word 2007 speichern können.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer Dateien im Rich Text Format (RTF) speichern. RTF wurde für eine einfache Übertragung formatierter Dokumente zwischen unterschiedlichen Anwendungen entwickelt. RTF-Dateien weisen die Dateierweiterung .rtf auf.

Wenn die Einstellung „Öffnen von RTF-Dateitypen blockieren“ aktiviert ist, Benutzer diese Dateitypen jedoch speichern können, speichern sie u. U. versehentlich Dateien im RTF-Format, die sie dann nicht öffnen können. Dadurch kann möglicherweise auf wichtige Daten nicht mehr zugegriffen werden.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer RTF-Dateien in Word 2007 nicht speichern.

**Tabelle 1.59. Speichern von RTF-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1741

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, RTF-Dateien in Word 2007 zu speichern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit RTF-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Textdateitypen blockieren

Betrifft: **Excel, Word**

Diese Einstellung steuert, ob Dateien als Textdateien in den angegebenen Anwendungen gespeichert werden können.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer Dokumente als Textdateien mit der Erweiterung .txt und Excel 2007-Benutzer Arbeitsmappen als Textdateien mit den Erweiterungen .txt, .csv und .prn speichern.

Wenn Dateien dieser Art mit anderen Benutzern gemeinsam verwendet werden, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Benutzer keine Textdateien in den angegebenen Anwendungen speichern.

**Tabelle 1.60. Speichern von Textdateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Dateiformate blockieren\Speichern

Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


excel12.adm, ppt12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-IDs**

</td>

<td>


Excel: CCE-1336

Word: CCE-1755

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, Textdateien in den angegebenen Anwendungen zu speichern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit Textdateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Speichern von Word 2003-XML-Dateitypen blockieren

Betrifft: **Word**

Diese Einstellung steuert, ob Word 2007-Dokumente im XML-Format von Word 2003 gespeichert werden können.

#### Sicherheitsrisiko

Standardmäßig können Word 2007-Benutzer Dateien im mit Microsoft Office Word 2003 eingeführten WordprocessingML-Dateiformat speichern. WordprocessingML-Dokumente weisen die Dateierweiterung .xml auf.

Wenn Dateien dieser Art mit anderen Benutzern gemeinsam verwendet werden, die aufgrund technischer oder Richtlinienbeschränkungen diese Dateien nicht öffnen können, wirkt sich dies möglicherweise negativ auf die Unternehmensproduktivität aus.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Word 2007-Benutzer keine Dateien im WordprocessingML-Format von Word 2003 speichern.

**Tabelle 1.61. Speichern von Word 2003-XML-Dateitypen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Dateiformate blockieren\Speichern

</td>

</tr>

<tr>

<td>


**ADM-Datei**

</td>

<td>


word12.adm

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1200

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden Benutzer daran gehindert, WordprocessingML-Dateien in Word 2007 zu speichern. Wenn Benutzer mit unternehmenswichtigen Dateien dieser Art arbeiten müssen, führt ein Aktivieren dieser Einstellung möglicherweise zu erheblichen Beeinträchtigungen. Benutzer, die nicht mit WordprocessingML-Dateien arbeiten, sollten von dieser Einstellung nicht betroffen sein.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Unter dem Thema zum [Planen der Blockierung von Dateiformateinstellungen im 2007 Office System](http://go.microsoft.com/fwlink/?linkid=101654)   im 2007 Office Resource Kit (möglicherweise in englischer Sprache) finden Sie weitere Informationen zum Verwenden der Gruppenrichtlinie für das Verwalten und Erzwingen von Dateiformatanforderungen. Im Abschnitt „Dateiblockierungstechnologie“ in Kapitel 4 des 2007 Microsoft Office-Sicherheitshandbuchs finden Sie Informationen über Microsoft Office Isolated Conversion Environment (MOICE), wodurch eine weitere Methode bereitgestellt wird.

### Bestimmte Dateitypen als Anlagen für Formulare blockieren

Betrifft: **InfoPath**

Diese Einstellung ermöglicht Administratoren ein Hinzufügen von Dateitypen (nach Dateierweiterung) zur Standardliste der Dateitypen, die in InfoPath 2007 vom Anhängen an Formulare blockiert sind.

#### Sicherheitsrisiko

An Formulare angehängte Dateien können Viren sowie andere schädliche Dateien verbreiten. Solche Dateien beeinträchtigen möglicherweise die Computer unachtsamer Empfänger.

Standardmäßig kann ein Benutzer alle Dateitypen an Formulare anhängen, außer potenziell unsicheren Dateitypen, die Viren enthalten können, z. B. BAT- oder EXE-Dateien. Eine vollständige Liste der von InfoPath® 2007 standardmäßig nicht zugelassenen Dateitypen finden Sie im Abschnitt über Sicherheitsdetails unter dem Thema zum [Einfügen eines Dateianlagesteuerelements](http://office.microsoft.com/en-us/infopath/hp100809081033.aspx)   (möglicherweise in englischer Sprache) auf der Microsoft Office Online-Website.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren zusätzlich zur Standardliste unzulässiger Dateitypen in InfoPath 2007 weitere zu blockierende Dateityperweiterungen festlegen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Informationen zum Entfernen von Dateitypen aus der Standardliste unzulässiger Dateitypen finden Sie unter der Einstellung „Dateitypen als Anlagen für Formulare zulassen“ in diesem Handbuch.

**Tabelle 1.62. Bestimmte Dateitypen als Anlagen für Formulare blockieren**

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


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**Empfohlene Einstellung (SSLF)**

</td>

<td>


Nicht konfiguriert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1267

</td>

</tr>

</table>

#### Auswirkung

Diese Einstellung wirkt sich auf die Nutzbarkeit aus, wenn Benutzer Dateien an Formulare anhängen. Wenn ein Dateityp blockiert ist, müssen Benutzer Dateien dieses Typs durch andere Methoden austauschen, z. B. durch Hochladen an einen freigegebenen Speicherort.

### Vertrauenswürdige Zonen blockieren

Betrifft: **Outlook**

Diese Einstellung steuert, ob Bilder von Websites in der Sicherheitszone für vertrauenswürdige Sites automatisch in Outlook 2007-E-Mail-Nachrichten und andere Elemente heruntergeladen werden.

#### Sicherheitsrisiko

Böswillige Benutzer können HTML-E-Mail-Nachrichten mit eingebetteten Webbeacons versenden. Dabei handelt es sich um Bilder und andere Inhalte von externen Servern, die verfolgen können, ob bestimmte Empfänger die Nachrichten öffnen. Durch Anzeige einer E-Mail-Nachricht mit einem Webbeacon wird bestätigt, dass die E-Mail-Adresse des Empfängers gültig ist, wodurch der Empfänger anfällig für zusätzliche Spam-Nachrichten und schädliche E-Mails wird.

Um das Risiko durch Webbeacons zu reduzieren, wird in Outlook 2007 externer Inhalt in E-Mail-Nachrichten standardmäßig deaktiviert, es sei denn, der Inhalt wird gemäß der Kontrollkästchen im Bereich **Automatischer Download** des Vertrauensstellungscenters als „sicher“ angesehen. Abhängig von der Konfiguration dieser Optionen kann es sich bei sicherem Inhalt um Folgendes handeln: Inhalte in Nachrichten von Adressen, die in der Liste sicherer Absender bzw. in der Liste sicherer Empfänger definiert sind, die vom Junk-E-Mail-Filter verwendet werden, Inhalte aus SharePoint-Diskussionsrunden sowie Inhalte aus Websites in der Zone **Vertrauenswürdige Sites** in Internet Explorer.

Outlook sieht vertrauenswürdige Sites von Internet Explorer als sicher an und lädt daher stammende Inhalte automatisch herunter. Diese Inhalte könnten möglicherweise Webbeacons enthalten.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, lädt Outlook 2007 nicht automatisch Inhalte von Websites der Zone **Vertrauenswürdige Site** in Internet Explorer herunter. Empfänger können auf der Basis jeder einzelnen Nachricht entscheiden, ob externe Inhalte heruntergeladen werden.

**Tabelle 1.63. Vertrauenswürdige Zonen blockieren**

<table>

<tr>

<td>


**Speicherort in Gruppenrichtlinie**

</td>

<td>


Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Einstellungen für den automatischen Download von Bildern

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


Aktiviert

</td>

</tr>

<tr>

<td>


**CCE-ID**

</td>

<td>


CCE-1475

</td>

</tr>

</table>

#### Auswirkung

Die empfohlene Einstellung für eine SSLF-Umgebung ist **Aktiviert**, was bedeutet, dass Outlook 2007 nicht automatisch externen Inhalt von Websites in der Zone **Vertrauenswürdige Sites** herunterlädt Diese Konfiguration kann zu Beeinträchtigungen für Benutzer führen, die regelmäßig HTML-E-Mail-Nachrichten von Websites in dieser Zone empfangen, die Grafiken oder andere externe Inhalte enthalten, da diese Inhalte für jede Nachricht einzeln heruntergeladen werden müssen.

### Anwendung der Aktualisierungen von der Office Update-Website blockieren

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob Updates von der Office Update-Website angewendet werden.

![](images/Dd443669.important(de-de,TechNet.10).gif) **Wichtig:**

Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103519)  .

#### Sicherheitsrisiko

Der Empfang von Updates von der Office Update-Website ermöglicht es Benutzern, ihre 2007 Microsoft Office-Installation auf dem neuesten Stand zu halten. In vielen Fällen ziehen Administratoren jedoch vor, dass Benutzer Updates zu einem Zeitpunkt ihrer Wahl von einem lokalen Server abrufen. Oft werden Updates durch ein Tool wie SMS bereitgestellt. Dieser Ansatz ermöglicht es Administratoren, durch das Testen von Updates eine erhöhte Verfügbarkeit zu gewährleisten sowie einen Änderungs- und Konfigurationsverwaltungsprozess einzusetzen, damit Updates konsequent innerhalb des gesamten Unternehmens implementiert werden.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, werden die Elemente **Suchen nach Updates** im Menü sowie im Aufgabenbereich deaktiviert, und 2007 Office-Anwendungen können keine Updates von der Office Update-Website abrufen.

**Tabelle 1.64. Anwendung der Aktualisierungen von der Office Update-Website blockieren**

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


Deaktiviert

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


CCE-784

</td>

</tr>

</table>

#### Auswirkung

Durch Aktivieren dieser Einstellung werden die Elemente **Suchen nach Updates** im Menü und im Aufgabenbereich deaktiviert.
 
In diesem Beitrag
* [Überblick](https://technet.microsoft.com/de-de/library/fe58931e-25fa-4a32-8497-416dbe4929c3(v=TechNet.10))
* Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10))
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3](https://technet.microsoft.com/de-de/library/f3af8a5d-5067-4add-917b-f7ab8cdca16c(v=TechNet.10))
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10))
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5](https://technet.microsoft.com/de-de/library/30aec6b9-6584-4724-8f8e-46357eecddd6(v=TechNet.10))
* [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6](https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10))
* [Sicherheitseinstellungen für Computerrichtlinien](https://technet.microsoft.com/de-de/library/e5d2501b-a96b-4c69-b912-59ad22c30503(v=TechNet.10))
 

**Download**  


[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)  

[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)  

**Update-Benachrichtigungen**  


[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)  

**Feedback**  


[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007 microsoft office-sicherheitshandbuch, bedrohungen und gegenmaßnahmen: sicherheitseinstellungen in 2007 office system)  

 

<table>

<tr>

<td>

[Zum Seitenanfang](#mainsection)  
</td>

<td>

[](https://technet.microsoft.com/de-de/library/fe58931e-25fa-4a32-8497-416dbe4929c3(v=TechNet.10)"><img AltText="Vorherige Seite)   2 von 8 [](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10)"><img AltText="Nächste Seite)  
</td>

</tr>

</table>




