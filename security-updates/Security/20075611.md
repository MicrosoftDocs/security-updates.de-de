---
Title: Windows Vista-Sicherheitshandbuch – Kapitel 4 (Anwendungskompatibilität)
TOCTitle: Windows Vista-Sicherheitshandbuch – Kapitel 4 (Anwendungskompatibilität)
ms:assetid: 557de5af-482d-45d9-a1f1-6999c4b521ed
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443668(v=TechNet.10)
ms:contentKeyID: 20075611
---


# Windows Vista-Sicherheitshandbuch



### Kapitel 4: Anwendungskompatibilität
Veröffentlicht: 08. Nov 2006
 

Die Anwendungskompatibilität stellt immer eine zentrale Herausforderung dar, der sich Unternehmen beim Bereitstellen eines neuen Betriebssystems stellen müssen. Ein Großteil der Entwicklungsarbeit bei Windows Vista™ wurde aufgewendet, um sicherzustellen, dass die neuen Funktionen und Dienste im Betriebssystem mit älteren Programmen weitgehend kompatibel sind und deren Funktionalität gewährleisten. Während der gesamten Entwicklung testete das Microsoft Application Experience Team eine Vielzahl von Anwendungen von vielen verschiedenen Drittanbietern.

Die Sicherheitseinstellungen, die in diesem Handbuch zum Absichern von Windows Vista beschrieben werden, wurden umfassenden Tests unterzogen. Auf diese Weise konnte sowohl die Kompatibilität mit dem Betriebssystemkern als auch mit der Anwendungssuite Microsoft® Office gewährleistet werden. Anwendungen, die unter Windows Vista ausgeführt werden, sollten weiterhin problemlos auf den Clientcomputern funktionieren, nachdem die in diesem Handbuch empfohlenen Einstellungen vorgenommen wurden.

Allerdings besteht die Möglichkeit, dass ältere Anwendungen möglicherweise mit einigen der neuen Sicherheitstechnologien von Windows Vista nicht richtig zusammenarbeiten. Technologien wie die Benutzerkontensteuerung (UAC) und der Windows-Ressourcenschutz können die Funktionalität älterer Anwendungen beeinträchtigen.

Der Microsoft Solution Accelerator for Business Desktop Deployment (BDD) 2007 enthält einen umfassenden Leitfaden zur Anwendungskompatibilität, damit IT-Experten die Kompatibilität von Anwendungen mit Windows Vista prüfen und Kompatibilitätsprobleme mindern können, die möglicherweise während des Verfahrens entdeckt wurden. Weitere Informationen finden Sie im [*Application Compatibility Feature Team Guide*](http://go.microsoft.com/fwlink/?linkid=74194) (engl.).

Dieses Kapitel enthält einfache Vorgehensweisen, mit denen Sie den Grad der Kompatibilität Ihrer Anwendungen mit Windows Vista überprüfen können. Zudem werden einige der häufigsten Gründe von Problemen mit der Anwendungskompatibilität besprochen. Außerdem enthält das Kapitel Verweise auf verfügbare Ressourcen, die beim Lösen der Probleme hilfreich sind.

Auf dieser Seite

[Kompatibilitätsprüfung in 30 Minuten](#edaa)  
[Bekannte Probleme mit der Anwendungskompatibilität](#ecaa)  
[Tools und Ressourcen](#ebaa)  
[Weitere Informationen](#eaaa)  



### Kompatibilitätsprüfung in 30 Minuten

Dieser Abschnitt enthält Anleitungen zum Prüfen und Bewerten der Anwendungskompatibilität mit Windows Vista. Er umfasst zwei Szenarien, die Sie zum Prüfen der Anwendungskompatibilität mit dem Betriebssystem verwenden können. Diese Szenarien unterstützen Sie bei Folgendem:
* Testen einer Anwendung mit einer vollständig neuen Installation von Windows Vista

* Testen einer Anwendung mit einem Upgrade auf Windows Vista von Microsoft Windows® XP mit Service Pack 2 (SP2)

 

**So testen Sie eine Anwendung mit einer vollständig neuen Installation von Windows Vista**
1. Installieren Sie Windows Vista auf einem Testcomputer.

2. Melden Sie sich als Administrator auf dem Testcomputer an, auf dem Windows Vista ausgeführt wird.

3. Installieren Sie die Anwendung, die Sie unter Windows Vista testen möchten. Wenn Sie in einem Dialogfeld gefragt werden, ob die Anwendung installiert werden darf, klicken Sie auf **Zulassen**, um mit der Installation fortzufahren. Wenn die Installation erfolgreich war, fahren Sie mit Schritt 6 fort.

4. Wenn die Installation der Anwendung nicht erfolgreich war und kein Dialogfeld angezeigt wurde, in dem Sie um Erlaubnis zur Installation gefragt wurden, klicken Sie mit der rechten Maustaste auf die Installationsdatei, klicken Sie auf die Option **Als Administrator ausführen**, und installieren Sie die Anwendung erneut. Wenn die Installation erfolgreich war, fahren Sie mit Schritt 7 fort.

    **Hinweis**:   Dieser Schritt ist nicht notwendig, wenn Sie eine MSI-Datei (Microsoft Installer) zum Installieren der Anwendung verwenden.

5. Wenn Fehler zu Betriebssystemversion, Anwendungsregistrierung oder Dateikopie angezeigt werden, klicken Sie mit der rechten Maustaste auf die Installationsdatei, klicken Sie auf **Kompatibilität**, und wählen Sie dann den Windows XP SP2-Kompatibilitätsmodus aus.

6. Wiederholen Sie Schritt 2. Wenn Sie die Anwendung immer noch nicht installieren können, gehen Sie zu Schritt 8.

7. Melden Sie sich als Benutzer ohne Administratorechte an dem Testcomputer an, auf dem Windows Vista ausgeführt wird.

8. Starten Sie die Anwendung. Wenn die Anwendung nicht ordnungsgemäß startet oder Fehlermeldungen angezeigt werden, aktivieren Sie den Windows XP SP2-Kompatibilitätsmodus für die Anwendungsprogrammdatei, und versuchen Sie dann erneut, die Datei unter dem Betriebssystem zu installieren.

9. Wenn die Anwendung erfolgreich startet, führen Sie die vollständige Reihe von Tests aus, die Sie typischerweise auf einem Computer verwenden würden, auf dem Windows XP ausgeführt wird. Überprüfen Sie die Funktionalität Ihrer Anwendung, um zu bestätigen, dass sie ordnungsgemäß ausgeführt wird. Wenn die Anwendung alle wichtigen Funktionalitätstests besteht, kann sie problemlos mit Windows Vista verwendet werden.

10. Wenn die Anwendung nicht erfolgreich installiert und gestartet werden kann, nicht mehr reagiert, Fehler verursacht oder einen der wichtigsten Funktionalitätstests nicht besteht, gehört sie möglicherweise zu der kleinen Anzahl von Anwendungen, bei denen Kompatibilitätsprobleme mit Windows Vista auftreten. Ziehen Sie die anderen Ressourcen in den Referenzen dieses Kapitels heran, um Ihre Anwendung weiter zu untersuchen und zu testen.

 

**So testen Sie eine Anwendung mit einem Upgrade auf Windows Vista von Windows XP SP2**
1. Installieren Sie Windows XP mit SP2 auf einem Testcomputer, und installieren Sie dann die Anwendung, die Sie testen möchten. Überprüfen Sie die gesamte Funktionalität der Anwendung, bevor Sie fortfahren.

2. Aktualisieren Sie den Testcomputer auf Windows Vista. Befolgen Sie die Anweisungen zu Installation und Upgrade für Windows Vista. Nachdem das Upgrade abgeschlossen ist, melden Sie sich am Testcomputer in gleicher Weise an wie unter Windows XP.

3. Starten Sie die Anwendung. Wenn die Anwendung nicht ordnungsgemäß startet oder wenn Fehlermeldungen angezeigt werden, aktivieren Sie den Windows XP SP2-Kompatibilitätsmodus für die Anwendungsprogrammdatei, und versuchen Sie dann erneut, die Datei zu installieren.

4. Wenn die Anwendung erfolgreich startet, führen Sie die vollständige Reihe von Tests aus, die Sie typischerweise auf einem Computer verwenden würden, auf dem Windows XP ausgeführt wird. Überprüfen Sie die Funktionalität Ihrer Anwendung, um zu bestätigen, dass sie ordnungsgemäß ausgeführt wird. Wenn die Anwendung alle wichtigen Funktionalitätstests besteht, kann sie problemlos mit Windows Vista verwendet werden.

5. Wenn die Anwendung nicht erfolgreich installiert und gestartet werden kann, nicht mehr reagiert, Fehler verursacht oder einen der wichtigsten Funktionalitätstests nicht besteht, gehört sie möglicherweise zu der kleinen Anzahl von Anwendungen mit Kompatibilitätsproblemen, die durch die Änderungen in Windows Vista verursacht wurden. Ziehen Sie die anderen Ressourcen in den Referenzen dieses Kapitels heran, um Ihre Anwendung weiter zu untersuchen und zu testen.

 

Wenn Sie beide Szenarien abschließen und bestimmen, dass die Anwendung ordnungsgemäß funktioniert, können Sie von einer Kompatibilität mit Windows Vista ausgehen.
[Zum Seitenanfanq](#mainsection)  



### Bekannte Probleme mit der Anwendungskompatibilität

In diesem Abschnitt einiger der geläufigsten neuen Technologien, Verbesserungen und Änderungen in Windows Vista beschrieben, die Probleme mit der Anwendungskompatibilität verursachen. Soweit möglich, enthält dieser Abschnitt zudem Methoden zum potenziellen Abmildern der Probleme.

**Wichtig**:   Testen Sie alle Anwendungen von Drittanbietern, die Sie in Ihrer Umgebung mit Windows Vista verwenden möchten. Auf diese Weise können Sie sicherstellen, dass die Anwendungen problemlos mit dem Betriebssystem verwendet werden können.


#### Sicherheitsverbesserungen

Die folgenden neuen Sicherheitsfunktionen in Windows Vista können Kompatibilitätsprobleme mit Anwendungen von Drittanbietern verursachen:
* **Benutzerkontensteuerung:** Diese neue Funktion stellt eine Methode bereit, um die Aufgaben, die von Standardbenutzern ausgeführt werden können, von den Aufgaben zu trennen, die Administratorzugriff erfordern. Die Benutzerkontensteuerung (UAC) erhöht die Sicherheit, indem sie die Computerbenutzung für Benutzer verbessert, die mit Standardbenutzerkonten arbeiten. Benutzer können jetzt mehr Aufgaben ausführen und eine höhere Anwendungskompatibilität nutzen, ohne sich an ihren Clientcomputern mit Administratorrechten anmelden zu müssen. Dies trägt dazu bei, die Auswirkungen von Malware, unautorisierter Softwareinstallation und ungenehmigten Systemänderungen zu verringern.

    UAC kann Probleme bei Anwendungen verursachen, die mit dieser technologischen Erweiterung nicht kompatibel sind. Aus diesem Grund ist es wichtig, Anwendungen vor deren Bereitstellung mit aktivierter Benutzerkontensteuerung zu testen. Weitere Informationen zum Testen der Anwendungskompatibilität finden Sie im [*Application Compatibility Feature Team Guide*](http://go.microsoft.com/fwlink/?linkid=74194) (engl.), der Bestandteil des Solution Accelerator für BDD ist.

* **Windows-Ressourcenschutz:** Diese neue Funktion in Windows Vista trägt zum Sichern von Systemdateien und geschützten Registrierungseinträgen bei und verbessert dadurch die gesamte Sicherheit und Stabilität des Betriebssystems. Die meisten Anwendungen, die zuvor auf diese Dateien oder Einträge zugegriffen oder Änderungen vorgenommen haben, werden jetzt automatisch auf temporäre Speicherorte umgeleitet. Auf diese Weise können die Anwendungen problemlos weiter verwendet werden.

    Falls Anwendungen jedoch Vollzugriff auf diese geschützten Bereiche benötigen und den automatischen Umleitungsvorgang nicht unterstützen, können diese Anwendungen mit Windows Vista nicht richtig genutzt werden. In diesen Fällen müssen Sie die Anwendungen so ändern, dass sie wie vorgesehen funktionieren. Weitere Informationen zu diesem neuen Feature und dessen Auswirkungen auf die Anwendungskompatibilität finden Sie in der MSDN Library unter [About Windows Resource Protection](http://msdn2.microsoft.com/en-us/library/aa382503.aspx) (engl.).

* **Geschützter Modus:** Diese neue Funktion von Microsoft Internet Explorer® 7 trägt dazu bei, Computer mit dem Betriebssystem Windows Vista vor der Installation von Malware und anderer schädlicher Software zu schützen. Hierzu wird das Betriebssystem mit geringeren Rechten ausgeführt, die ein höheres Maß an Sicherheit gewährleisten. Wenn Internet Explorer im geschützten Modus ausgeführt wird, kann der Browser nur mit bestimmten Bereichen des Dateisystems und der Registrierung interagieren.

    Obwohl der geschützte Modus hilft, die Integrität von Clientcomputern unter Windows Vista zu gewährleisten, kann er die Ausführung von älteren Webanwendungen in Internet und Intranet beeinträchtigen. Möglicherweise müssen Sie solche Webanwendungen ändern, damit sie in einer restriktiveren Umgebung ausgeführt werden können.

 


#### Änderungen am Betriebssystem und Innovationen

Die folgenden Neuerungen am Betriebssystem und Innovationen in Windows Vista können möglicherweise Kompatibilitätsprobleme mit Anwendungen von Drittanbietern verursachen:
* **Neue System-APIs:** Anwendungsprogrammierschnittstellen (APIs) stellen den Zugriff auf die verschiedenen Schichten des Betriebssystems Windows Vista auf andere Weise als bei früheren Versionen von Windows bereit. Antiviren- und Firewallsoftware sind Beispiele für Anwendungen, die diese neuen APIs benötigen, um Windows Vista richtig überwachen und schützen zu können. Sie müssen Anwendungen, die diese Funktionen ausführen, auf Versionen aktualisieren, die mit Windows Vista kompatibel sind.

* **Windows Vista 64-Bit:** 16-Bit-Anwendungen und 32-Bit-Treiber werden in der 64-Bit-Umgebung von Windows Vista nicht unterstützt. Die automatische Umleitung für die Registrierung und Systemdateien steht in der 64-Bit-Umgebung nicht zur Verfügung. Aus diesen Gründen müssen neue 64-Bit-Anwendungen vollständig mit den Anwendungsstandards von Windows Vista übereinstimmen.

* **Betriebssystemversionen:** Viele ältere Anwendungen überprüfen auf bestimmte Versionen von Windows. Wenn Anwendungen von Drittanbietern eine bestimmte Betriebssystemversion nicht erkennen können, reagieren viele dieser Anwendungen nicht mehr.

    Den meisten Kompatibilitätsproblemen, die durch Anforderungen an die Betriebssystemversion verursacht werden, wurde durch neue Funktionen in Windows Vista Rechnung getragen. Features wie der Programmkompatibilitäts-Assistent können diese Arten von Problemen in der Regel automatisch lösen. Weitere Informationen über den Programmkompatibilitäts-Assistenten und andere Tools und Ressourcen finden Sie im nächsten Abschnitt dieses Kapitels.

 

Der MSDN-Artikel [The Windows Vista Developer Story: Application Compatibility Cookbook](http://msdn2.microsoft.com/en-us/library/aa480152.aspx) (engl.) stellt zusätzliche Informationen zu diesen Sicherheitsverbesserungen sowie Änderungen am Betriebssystem und Innovationen in Windows Vista zur Verfügung. Dieses Buch mit Anleitungen enthält zudem Testverfahren und mögliche Lösungen für die meisten dieser Kompatibilitätsprobleme.
[Zum Seitenanfanq](#mainsection)  



### Tools und Ressourcen

Dieser Abschnitt enthält kurze Themenüberblicke und Verweise auf Funktionen und Technologien, die für Windows Vista verfügbar sind und Ihnen helfen sollen, Probleme mit der Anwendungskompatibilität zu beheben.


#### Programmkompatibilitäts-Assistent

Diese Funktion legt automatisch einen geeigneten „Kompatibilitätsmodus“ für Anwendungen fest, die für frühere Versionen von Windows entwickelt wurden. Wenn Windows Vista Anwendungen erkennt, die im Kompatibilitätsmodus für Windows XP, Windows 2000 oder spätere Versionen von Windows ausgeführt werden müssen, leitet das Betriebssystem die automatische Aktualisierung dieser Anwendungen ein, damit sie unter Windows Vista ausgeführt werden können. Ein weiterer Eingriff des Benutzers ist hierbei nicht erforderlich.

Weitere Informationen finden Sie unter [Program Compatibility Assistant: Frequently Asked Questions](http://windowshelp.microsoft.com/windows/en-us/help/82c0440d-553e-47e9-b4bd-6c2d10df4de71033.mspx) (engl.).


#### Programmkompatibilitäts-Assistent

Der Programmkompatibilitäts-Assistent in Windows Vista soll Ihnen behilflich sein, wenn ein Programm nicht ordnungsgemäß ausgeführt wird, das für eine frühere Version von Windows geschrieben wurde. Der Assistent unterstützt Sie beim Festlegen von Kompatibilitätseinstellungen für das Programm, um Probleme mit der Anwendungskompatibilität bei vielen älteren Programmen zu lösen.

Zum Zugriff auf den Programmkompatibilitäts-Assistenten doppelklicken Sie auf dem Desktop auf das Symbol **Programmkompatibilitäts-Assistent.**  

Weitere Informationen finden Sie unter [Make Older Programs Run in this Version of Windows](http://windowshelp.microsoft.com/windows/en-us/help/bf416877-c83f-4476-a3da-8ec98dcf5f101033.mspx) (engl.).

![](images/dd443668.warning(de-de,technet.10).gif)**Achtung:**

Führen Sie den Programmkompatibilitäts-Assistenten nicht für ältere Antivirenprogramme, Datenträgerdienstprogramme oder andere Systemprogramme aus, da dies zu Datenverlusten oder Sicherheitsrisiken führen könnte. Verwenden Sie stattdessen nur Versionen dieser Programme und Dienstprogramme, die speziell für die Nutzung mit Windows Vista entwickelt wurden.


#### Microsoft Standard User Analyzer

Dieses Tool zur Prüfung der Anwendungskompatibilität unterstützt Entwickler und IT-Experten beim Diagnostizieren von Problemen, die das ordnungsgemäße Ausführen eines Programms ohne Administratorrechte verhindern. Wenn Sie mit dem Standard User Analyzer Ihre Anwendung testen, können Sie Probleme mit Dateizugriff, Registrierungszugriff, Tokens und anderen geschützten Bereichen des Betriebssystems identifizieren.

Unter Windows Vista können standardmäßig sogar Administratoren die meisten Programme mit Standardbenutzerrechten ausführen. Mit diesem Tool können Sie sicherstellen, dass Ihre Anwendung keinen Administratorzugriff benötigt, um verwendet werden zu können. Die Ergebnisse werden in einer übersichtlichen grafischen Benutzeroberfläche dargestellt.

Sie können dieses Tool unter [Microsoft Standard User Analyzer](http://www.microsoft.com/downloads/details.aspx?familyid=df59b474-c0b7-4422-8c70-b0d9d3d2f575&amp;displaylang=en) (engl.) im Microsoft Download Center herunterladen.


#### Anwendungskompatibilitäts-Toolkit

Microsoft hat eine Reihe von Tools und Dokumentationen bereitgestellt, die Sie beim Identifizieren und Verwalten des Anwendungsportfolios Ihres Unternehmens unterstützen sollen. Das Windows Anwendungskompatibilitäts-Toolkit (ACT) wurde entwickelt, um Kosten und Zeitaufwand für die Behebung von Problemen mit der Anwendungskompatibilität zu verringern und Windows Vista so schneller bereitstellen zu können.

ACT unterstützt Sie bei den Vorbereitungen für den Einsatz von Windows Vista. Hierzu erstellt ACT ein Inventar Ihrer vorhandenen Anwendungen, verwaltet wichtige Anwendungen und bestimmt, in welchem Umfang Ihre Anwendungsumgebung möglicherweise speziell für Windows Vista vorbereitet werden muss.

Zurzeit ist ACT 4.1 verfügbar und wurde ausgeliefert, um Kunden bei der Bereitstellung von Windows XP SP2 zu unterstützen. ACT 4.1 untersucht DCOM-Schnittstellen, Firewalleinstellungen und Probleme mit Internet Explorer. ACT wurde entwickelt um zu ermitteln, welche Anwendungen weitere Tests erfordern, welche Anwendungen veraltet und welche bereits mit SP2 kompatibel sind, so dass Sie Prioritäten für Ihre Arbeit setzen können.

ACT 5.0 wurde speziell im Hinblick auf die Sicherheitsfeatures von Windows Vista aktualisiert.

Zu den Verbesserungen in diesem Toolkit zählen unter anderem:
* Neue spezifische Kompatibilitätsauswertungen für Windows Vista

* Aktualisierte Benutzeroberfläche für die zentrale Verwaltung der Auswertungseinstellungen

* Neue Funktionen zum Organisieren von Daten, mit denen Sie Kategorien und Prioritäten für Ihre Anwendungen erstellen können

* Funktionen zur Datenanalyse, mit denen Sie umfassende Kompatibilitätsberichte anzeigen können

* Eine Anwendercommunity im Internet, die es Kunden und unabhängigen Softwareanbietern (ISVs) ermöglicht, Informationen zu ihren eigenen Ergebnissen bei Tests der Anwendungskompatibilität auszutauschen

 

Weitere Informationen zum Toolkit finden Sie auf der Seite [Windows Vista – Anwendungskompatibilität](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/appcompat/default.mspx) (engl.).

**Vorübergehende Lösungen**

Neben spezifischen Tools und Ressourcen für die Anwendungskompatibilität gibt es weitere Microsoft-Technologien, die Sie bei Problemen mit der Anwendungskompatibilität einsetzen können, deren vollständige Lösung möglicherweise längere Zeit erfordert. Diese Technologien sollen Sie bei der Migration zu Windows Vista unterstützen und es Ihnen ermöglichen, weiterhin unternehmenskritische Anwendungen auszuführen, die nicht mit Windows Vista kompatibel sind. Zu diesen Technologien zählen unter anderem:
* **Virtual PC:** Mit Virtual PC können Sie Anwendungen unter Windows Vista ausführen, die nur mit älteren Versionen von Windows ordnungsgemäß funktionieren. Virtual PC ermöglicht es Benutzern, eine frühere Version von Windows verfügbar zu halten, um nicht kompatible Anwendungen innerhalb ihrer Windows Vista-Umgebung auszuführen. Auf diese Weise kann die Zeit überbrückt werden, bis aktualisierte Versionen nicht kompatibler Anwendungen entwickelt werden. Weitere Informationen finden Sie auf der Website zu [Microsoft Virtual PC](http://www.microsoft.com/germany/windows/virtualpc/default.mspx).

* **Terminaldienste für Anwendungshosting:** Das Hosten älterer Anwendungen auf Terminaldiensten ermöglicht es Ihnen, Windows-basierte Anwendungen oder den Windows-Desktop selbst auf praktisch jedem Computer in Ihrem Netzwerk bereitzustellen. Windows Vista-Clients können über Remotedesktop eine Verbindung mit diesen Anwendungshosting-Umgebungen herstellen, um auf ältere Anwendungen zuzugreifen. Weitere Informationen finden Sie unter [Technical Overview of Windows Server 2003 Terminal Services](http://www.microsoft.com/windowsserver2003/techinfo/overview/termserv.mspx) (engl.).

* **Virtual Server für Anwendungshosting:** In einer Virtual Server-Umgebung können Sie ältere Anwendungen hosten und Remoteverbindungen von Endbenutzern zulassen, die Zugriff auf diese Anwendungen benötigen. In Verbindung mit Windows Server 2003 stellt Virtual Server 2005 R2 eine Virtualisierungsplattform zur Verfügung, unter der die meisten *x*86-Betriebssysteme in einer Gastumgebung ausgeführt werden können. Sie wird von Microsoft als Host für Windows Server-Betriebssysteme und Microsoft Windows Server System™-Anwendungen unterstützt. Weitere Informationen finden Sie auf der [Virtual Server 2005 R2-Produkthomepage](http://www.microsoft.com/germany/virtualserver/default.mspx) (engl.).

 
 
[Zum Seitenanfanq](#mainsection)  



### Weitere Informationen

Die folgenden Links stellen zusätzliche Informationen zur Anwendungskompatibilität mit Windows Vista bereit:
* [About Windows Resource Protection](http://msdn2.microsoft.com/en-us/library/aa382503.aspx) (engl.)

* [*Anwendungskompatibilität – Handbuch für das Feature-Team*](https://technet.microsoft.com/de-de/library/b1e6fe2b-2d1b-4a72-9017-b5d32627b0b7(v=TechNet.10))


* [Introduction to the Protected Mode API](http://msdn.microsoft.com/library/default.asp?url=/workshop/security/protmode/overviews/pmie_intro.asp) (engl.)

* [Windows Vista Help: Make older programs run in this version of Windows](http://windowshelp.microsoft.com/windows/en-us/help/bf416877-c83f-4476-a3da-8ec98dcf5f101033.mspx) (engl.)

* [Microsoft Application Compatibility Toolkit 5.0](http://technet.microsoft.com/en-us/windowsvista/aa905072.aspx) (engl.)

* [Microsoft Standard User Analyzer](http://www.microsoft.com/downloads/details.aspx?familyid=df59b474-c0b7-4422-8c70-b0d9d3d2f575&amp;displaylang=en) (engl.)

* [Microsoft Virtualization Solutions](http://www.microsoft.com/windowsserversystem/virtualization/default.mspx) (engl.)

* [Windows Vista Help: Program Compatibility Assistant – Frequently Asked Questions](http://windowshelp.microsoft.com/windows/en-us/help/82c0440d-553e-47e9-b4bd-6c2d10df4de71033.mspx) (engl.)

* [Technical Overview of Windows Server 2003 Terminal Services](http://www.microsoft.com/windowsserver2003/techinfo/overview/termserv.mspx) (engl.)

* [The Windows Vista Developer Story: Application Compatibility Cookbook](http://msdn2.microsoft.com/en-us/library/aa480152.aspx) (engl.)

* [Windows Vista - Anwendungskompatibilität](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/appcompat/default.mspx) (engl.)

 
 
[Zum Seitenanfanq](#mainsection)
 


### In diesem Beitrag
* [ Übersicht](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/default.mspx)
* [ Kapitel 1: Implementieren der Sicherheitsbasis](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx)
* [Kapitel 2: Schutz vor Malware](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx)
* [ Kapitel 3: Schutz von vertraulichen Daten](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)
*  Kapitel 4: Anwendungskompatibilität   

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

[![](https://technet.microsoft.com/de-de/Dd443668.pageLeft(de-de,TechNet.10).gif "Dd443668.pageLeft(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)
5 von 7[![](https://technet.microsoft.com/de-de/Dd443668.pageRight(de-de,TechNet.10).gif "Dd443668.pageRight(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/specialized_security.mspx)

</td>

</tr>

</table>





