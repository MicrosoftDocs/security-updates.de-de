---
Title: Kapitel 7 - Zusammenfassung
TOCTitle: Kapitel 7 - Zusammenfassung
ms:assetid: 8001f9fb-f330-4ab4-a134-ff756091ea0d
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Cc163082(v=TechNet.10)
ms:contentKeyID: 20072367
---


# Windows XP-Sicherheitshandbuch



### Kapitel 7: Zusammenfassung
Aktualisiert: 20. Okt 2005
 

Herzlichen Glückwunsch! Nach dem Lesen dieses Handbuchs sollten Sie nun ein klares Verständnis davon haben, wie Sie die Risiken einschätzen können, die in Ihrer Organisation die Sicherheit von Computer beeinträchtigen, auf denen das Betriebssystem Microsoft® Windows® XP Professional mit Service Pack 2 (SP2) ausgeführt wird. Sie haben Kenntnisse über die Planung und Entwicklung von Sicherheitsmaßnahmen für die Clientcomputer in Ihrer Infrastruktur gewonnen, wo solche Maßnahmen durchführbar sind.

Dieses Handbuch enthält Material von Beratern und Systemtechnikern, die Lösungen für Windows XP, Microsoft Windows Server™ 2003 und Windows 2000 in einer Vielzahl von Umgebungen implementiert haben. Es soll Ihnen einen aktuellen Satz an empfohlenen Vorgehensweisen für die Arbeit mit Windows XP an die Hand geben. Die ausführlichen Informationen in diesem Handbuch können auf jede Organisation angewendet werden.

Sicherheit ist ein wichtiges Thema, ungeachtet der Umgebung Ihrer Organisation. Viele Organisationen legen jedoch keinen großen Wert auf Sicherheit, da sie sie fälschlicherweise als etwas ansehen, das ihre Beweglichkeit und Flexibilität einschränkt. Wenn gut durchdachte Sicherheit zu einer Hauptgeschäftsanforderung wird und von Anfang an für jedes IT-Projekt geplant wird, kann eine korrekt implementierte Sicherheitsstrategie die Verfügbarkeit und Leistungsfähigkeit Ihrer Computersysteme verbessern. Umgekehrt kann eine Sicherheitsstrategie, die nachträglich zu einem Projekt hinzugefügt wird, die Benutzerfreundlichkeit, Stabilität und Verwaltungsflexibilität beeinträchtigen. Aus diesen Gründen wird vorgeschlagen, der Sicherheit in jeder Organisation höchste Priorität einzuräumen.

#### Auf dieser Seite

[Sichern des Clients](#ecaa)  
[Richtlinie für Softwareeinschränkungen](#ebaa)  
[Zusammenfassung](#eaaa)  



### Sichern des Clients

Windows XP Professional bietet einen vollständigen Satz an Sicherheitslösungen, mit denen Sie Desktop- und Laptopcomputer vor Bedrohungen schützen können. Benutzer, deren Computer keiner Domäne angehören, haben zwar weniger Sicherheitsoptionen, dennoch profitieren sowohl Benutzer innerhalb einer Domäne als auch eigenständige Benutzer von sicherem Zugriff auf ihre Computer.


#### Unternehmensclients

Wenn ein Clientcomputer Bestandteil eines Unternehmensnetzwerks ist, konfiguriert der Netzwerkadministrator den Computer möglicherweise durch die Sicherheitsfunktionen der Gruppenrichtlinie im Active Directory®-Verzeichnisdienst, der in diesem Handbuch ausführlich beschrieben wird. Alle von einem Netzwerkadministrator angewendeten Gruppenrichtlinieneinstellungen haben Vorrang vor den lokalen Einstellungen, die Benutzer auf ihren Computern festlegen. Mit Gruppenrichtlinien können Administratoren Umgebungen verwalten, die viele verschiedene Arten von Clientcomputern enthalten.


#### Clients in Hochsicherheitsumgebungen

In der Hochsicherheitsumgebung, die in diesem Handbuch beschrieben wird, stehen Fragen des Zugriffs, Dienste und die Infrastruktur der Umgebung im Vordergrund. Zusätzlich zu der verbesserten Sicherheitskontrolle und Benutzerauthentifizierung haben Administratoren eine größere Kontrolle über den Zugriff auf Ressourcen und Objekte im Netzwerk und auf den Clientarbeitsstationen. Diese Kontrolle wird von Administratoren benötigt, die für die Sicherheit von Daten und Ressourcen sorgen müssen. Dadurch wird unvermeidlich eingeschränkt, welche Aufgaben auf einem Clientcomputern in Hochsicherheitsumgebungen ausgeführt werden können. Aufgrund der erhöhten Sicherheitsanforderungen in dieser Art von Umgebung sind diese Einschränkungen jedoch notwendig.


#### Eigenständige Clients

Obwohl für eigenständige Clientcomputer weniger Einstellungen für Sicherheitsrichtlinien zur Verfügung stehen als für jene, die einer Active Directory-Domäne angehören, stehen für solche Computer wichtige Sicherheitsfunktionen zur Verfügung. Durch die korrekte Konfiguration dieser Richtlinieneinstellungen auf eigenständigen Computern wird das Risiko der Ausnutzung von Sicherheitsanfälligkeiten minimiert. Die Umgebung mit eigenständigen Clients bringt einen höheren administrativen Aufwand mit sich, da diese Computer nicht mithilfe von domänenbasierten Gruppenrichtlinien verwaltet werden können. Die Verwendung der in diesem Handbuch beschriebenen Programme trägt jedoch dazu bei, den administrativen Aufwand zu verringern.  

[Zum Seitenanfang](#mainsection)  

### Richtlinie für Softwareeinschränkungen

Richtlinien für Softwareeinschränkungen stellen Administratoren eine Möglichkeit zur Identifizierung von Software zur Verfügung, die auf Clientcomputern in einer Domäne oder in einer Umgebung mit eigenständigen Clients ausgeführt werden. Außerdem wird damit gesteuert, ob Software ausgeführt werden kann. Damit können schädliche Skripts oder Codes blockiert und die Ausführung unerwünschter Anwendungen verhindert werden. Richtlinien für Softwareeinschränkungen können für eigenständige Systeme konfiguriert oder über domänenbasierte Gruppenrichtlinien verwaltet werden, um die Systemintegrität und Verwaltbarkeit zu verbessern.  

[Zum Seitenanfang](#mainsection)  

### Zusammenfassung

In diesem Handbuch wurde erklärt, wie Sicherheitsrisiken in drei unterschiedlichen Umgebungen für Computer mit Windows XP mit SP2 effektiv beurteilt, priorisiert und vermindert werden können. Es wurden dokumentierte Methoden zum Planen und Entwerfen von Sicherheitsmaßnahmen für die Netzwerkinfrastruktur einer Organisation bereitgestellt, außerdem eine ausführliche Anleitung für die Beurteilung und Verminderung bestimmter Sicherheitsanfälligkeiten auf Computern in den Arten von Umgebungen, die im Handbuch beschrieben sind.

Die Gründe für die getroffenen Entscheidungen werden im Hinblick auf die Kompromisse erklärt, die einzugehen sind, wenn eine Organisation die verschiedenen Richtlinieneinstellungen für die drei Umgebungen implementiert. Es werden ausführliche Informationen dazu zur Verfügung gestellt, welche Auswirkungen bestimmte Richtlinieneinstellungen auf Funktionalität, Verwaltbarkeit, Leistung und Zuverlässigkeit haben können. Dadurch können Sie fundierte Entscheidungen darüber treffen, welche Einstellungen in Ihrer eigenen Umgebung implementiert werden sollten.

Sie sollten sich unbedingt dessen bewusst sein, dass die Absicherung von Clientcomputern in Ihrem Netzwerk kein einmaliges Projekt, sondern ein fortlaufender Prozess ist. Organisationen sollten sicherheitsbezogene Aufgaben und Planungen in ihre Budgets und Zeitpläne aufnehmen. Die Implementierung jeder Richtlinieneinstellung, die in diesem Handbuch erörtert wird, verbessert die Sicherheit in den meisten Organisationen, in denen Windows XP Professional verwendet wird. Wenn jedoch eine neue schwerwiegende Sicherheitsanfälligkeit entdeckt wird, können diese Umgebungen erneut angreifbar sein. Aus diesem Grund ist es äußerst wichtig, verschiedene Ressourcen zu überwachen, sodass Sie über Sicherheitsrisiken auf dem Laufenden bleiben, die mit den Betriebssystemen, Anwendungen und Geräten in Ihrer Umgebung in Zusammenhang stehen.

Alle Teammitglieder, die bei der Erstellung dieses Handbuchs mitgewirkt haben, hoffen, dass das darin enthaltene Material für Sie nützlich, informativ und leicht verständlich ist.


#### Weitere Informationen

Die folgenden Links bieten weitere Informationen zu sicherheitsbezogenen Themen hinsichtlich Windows XP Professional.
* Links zu häufigen Fragen und Antworten, Anleitungen, den neuesten Downloads und mehr finden Sie im [Windows XP-Supportcenter](http://support.microsoft.com/winxp) unter http://support.microsoft.com/winxp.

* Informationen zur Aufrechterhaltung der Sicherheit unter Windows XP finden Sie auf der Website [Vertrauenswürdiges Programmieren: Sicherheit](http://www.microsoft.com/germany/sicherheit/default.mspx) (in englischer Sprache) unter www.microsoft.com/germany/sicherheit/default.mspx.

* Informationen zur [Sicherheit](http://www.microsoft.com/technet/security/default.mspx) in TechNet finden Sie (in englischer Sprache) unter www.microsoft.com/technet/security/default.mspx.

* Informationen zur Planung für Windows XP Professional finden Sie auf der Seite [Windows XP Professional – Plan](http://www.microsoft.com/germany/technet/prodtechnol/winxppro/plan/default.mspx) auf der Technet-Website unter www.microsoft.com/germany/technet/prodtechnol/winxppro/plan/default.mspx.

* Ausführliche Anleitungen zu Sicherheitsfragen unter Windows XP Professional finden Sie auf der Webseite [Ressourcen für Sicherheitsanleitungen](http://www.microsoft.com/technet/itsolutions/howto/sechow.mspx) (in englischer Sprache) unter www.microsoft.com/technet/itsolutions/howto/sechow.mspx.

* Anleitungen zum [Ver- und Entschlüsseln von Daten](http://www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/sag_seconceptsunencrypt.mspx) mit dem verschlüsselnden Dateisystem (Encrypting File System, EFS) finden Sie (in englischer Sprache) unter www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/sag_seconceptsunencrypt.mspx.

[Zum Seitenanfang](#mainsection)
 

In diesem Beitrag
* [Überblick](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/default.mspx)
* [Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch01.mspx)
* [Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch02.mspx)
* [Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch03.mspx)
* [Kapitel 4: Administrative Vorlagen für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch04.mspx)
* [Kapitel 5: Schützen eigenständiger Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch05.mspx)
* [Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch06.mspx)
* Kapitel 7: Zusammenfassung
* [Anhang A: Weitere Anleitungen für Windows XP Service Pack 2](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapa.mspx)
* [Anhang A: Zu berücksichtigende Schlüsseleinstellungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxa.mspx)
* [Anhang B: Testen des Sicherheitshandbuchs für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxb.mspx)
* [Danksagungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgack.mspx)
 

Download

![](images/cc163082.icon_exe(de-de,technet.10).gif)[Windows XP-Sicherheitshandbuch herunterladen (engl.)](http://go.microsoft.com/fwlink/?linkid=14840&amp;clcid=0x409"><img AltText="Cc163082.icon_exe(de-de,TechNet.10).gif)  

[Zum Seitenanfang](#mainsection)