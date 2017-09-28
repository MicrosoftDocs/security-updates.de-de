---
TOCTitle: 'Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen'
Title: 'Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen'
ms:assetid: '3a17dffb-0395-4656-ada8-28e3954307f5'
ms:contentKeyID: 20075663
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443720(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen

Aktualisiert: 27.12.2005

In der in diesem Handbuch enthaltenen Microsoft® Excel®-Arbeitsmappe „Windows* *Server* *2003 Security Guide Settings.xls“ (in englischer Sprache) werden die Richtlinien- und Diensteinstellungen für sämtliche in diesem Handbuch enthaltenen Rollen und Umgebungen erläutert. Die Arbeitsmappe enthält zehn Arbeitsblätter, und zwar eines für jede Rolle im Handbuch:

-   Das Arbeitsblatt **Domain** (Domäne) enthält die Gruppenrichtlinieneinstellungen, mit denen die Richtlinienobjekte auf Domänenebene konfiguriert werden (siehe dazu Kapitel 6, „Die Domänenrichtlinie“).

-   Das Arbeitsblatt **Member Server Baseline** (Mitgliedserver-Baseline) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die MSBP konfiguriert wird (siehe dazu Kapitel 6, „Die Richtlinie für die Mitgliedsserver-Baseline“).

-   Das Arbeitsblatt **Domain Controller** (Domänencontroller) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die DCBP konfiguriert wird (siehe dazu Kapitel 6, „Die Richtlinie für die Domänencontroller-Baseline“).

-   Das Arbeitsblatt **Infrastructure Server** (Infrastrukturserver) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die Richtlinien für den Infrastrukturserver konfiguriert werden (siehe dazu Kapitel 6, „Die Infrastrukturserverrolle“).

-   Das Arbeitsblatt **File Server** (Dateiserver) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die Dateiserverrichtlinien konfiguriert werden (siehe dazu Kapitel 7, „Die Dateiserverrolle“).

-   Das Arbeitsblatt **Print Server** (Druckserver) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die Druckserverrichtlinien konfiguriert werden (siehe dazu Kapitel 8, „Die Druckserverrolle“).

-   Das Arbeitsblatt **Web Server** (Webserver) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die Richtlinien für den IIS-Webserver konfiguriert werden (siehe dazu Kapitel 9, „Die Webserverrolle“).

-   Das Arbeitsblatt **IAS Server** (IAS-Server) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die Richtlinien für den IAS-Server konfiguriert werden (siehe dazu Kapitel 10, „Die IAS-Serverrolle“).

-   Das Arbeitsblatt **CA Server** (Zertifizierungsstellenserver) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die Richtlinien für den Zertifikatdienstserver konfiguriert werden (siehe dazu Kapitel 11, „Die Zertifikatdienstserverrolle“).

-   Das Arbeitsblatt **Bastion Host** (Bastion-Host) enthält die Gruppenrichtlinien und SCW-Diensteinstellungen, mit denen die Richtlinien für den Bastion-Host konfiguriert werden (siehe dazu Kapitel 12, „Die Bastion-Hostrolle“).

Jedes Arbeitsblatt enthält die folgenden Spalten:

-   Spalte H, **Policy Setting Name in User Interface** (Name der Richtlinieneinstellung in der Benutzeroberfläche), enthält den Namen der Einstellung, wie er im Snap-In „Gruppenrichtlinien-Editor“ von Windows* *Server* *2003 angezeigt wird.

-   Spalte J, **Legacy Client** (Älterer Client), ist der empfohlene Wert für diese Einstellung in einer Umgebung mit älteren Clients.

-   Spalte K, **Enterprise Client** (Unternehmensclient), ist der empfohlene Wert für diese Einstellung in der Unternehmensclient-Umgebung.

-   Spalte L, **SSLF** (Hochsicher), ist der empfohlene Wert für diese Einstellung in der Hochsicherheitsumgebung.

Um die Lesbarkeit der Tabelle zu erhöhen, wurden zusätzliche Spalten verwendet, damit die Objekthierarchie innerhalb des Gruppenrichtlinien-Editors veranschaulicht wird. Die Spalten A bis G stellen dabei jeweils eine Ebene der Hierarchie dar. **Computer Configuration** (Computerkonfiguration) wird z. B. in Spalte A und **Security Settings** (Sicherheitseinstellungen) in Spalte C angezeigt. Spalte I wurde ebenfalls eingefügt, um die Lesbarkeit zu erhöhen.

[](#mainsection)[Zum Seitenanfang](#mainsection)

##### In diesem Beitrag

-   [Überblick](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/sgch00.mspx)
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch01.mspx)
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch02.mspx)
-   [Kapitel 3: Die Domänenrichtlinie](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch03.mspx)
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch04.mspx)
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch05.mspx)
-   [Kapitel 6: Die Infrastrukturserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch06.mspx)
-   [Kapitel 7: Die Dateiserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch07.mspx)
-   [Kapitel 8: Die Druckserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch08.mspx)
-   [Kapitel 9: Die Webserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch09.mspx)
-   [Kapitel 10: Die IAS-Serverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch10.mspx)
-   [Kapitel 11: Die Zertifikatdienstserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch11.mspx)
-   [Kapitel 12: Die Bastion-Hostrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch12.mspx)
-   [Kapitel 13: Zusammenfassung](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch13.mspx)
-   [Anhang A: Sicherheitstools und Formate](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxa.mspx)
-   [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxb.mspx)
-   Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen
-   [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxd.mspx)
-   [Danksagungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgack.mspx)

[](#mainsection)[Zum Seitenanfang](#mainsection)

**Download**

[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409)

**Benachrichtigung über Neuerungen**

[Melden Sie sich an, um sich über Updates und neue Versionen zu informieren](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx)

**Feedback**

[Senden Sie uns Ihre Kommentare oder Vorschläge](mailto:secwish@microsoft.com?subject=windows%20server%202003%20security%20guide)

 
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
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxb.mspx"><img src="images/Dd443720.pageLeft(de-de,TechNet.10).gif" /></a> 17 von 19 <a href="http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxd.mspx"><img src="images/Dd443720.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
