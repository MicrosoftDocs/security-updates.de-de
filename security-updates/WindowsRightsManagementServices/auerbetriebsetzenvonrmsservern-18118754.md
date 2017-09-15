---
TOCTitle: 'Außerbetriebsetzen von RMS-Servern'
Title: 'Außerbetriebsetzen von RMS-Servern'
ms:assetid: '11badb02-62c1-455c-96b7-935bbcb496bc'
ms:contentKeyID: 18118754
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720200(v=WS.10)'
---

Außerbetriebsetzen von RMS-Servern
==================================

Wenn Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) außer Betrieb setzen, ändert sich das Verhalten des Servers mit RMS so, dass er einen Schlüssel bereitstellen kann, der die zuvor veröffentlichten RMS-geschützten Inhalte entschlüsselt. Damit wird das Speichern der Inhalte ohne RMS-Schutz ermöglicht. Dies ist hilfreich, wenn Sie den RMS-Schutz künftig nicht mehr in Ihrer Organisation verwenden möchten.

Sie sollten den Server lange genug im außer Betrieb gesetzten Zustand ausführen, damit Benutzer Gelegenheit haben, die Inhalte ohne RMS-Schutz zu speichern, und Netzwerk- und Systemadministratoren die Verwendung des Dienstes durch RMS-fähige Clients deaktivieren können.

Sie können die Außerbetriebsetzung auf der Webseite **Sicherheitseinstellungen** der Verwaltungswebsite aktivieren. Wenn Sie die Außerbetriebsetzung aktiviert haben, können Sie für den Server keine RMS- Standardserverkonfiguration wiederherstellen. Wenn die Installation vertrauenswürdige veröffentlichte Domänen beinhaltet hat, werden diese ebenfalls außer Betrieb gesetzt.

Wenn Sie die Außerbetriebsetzung aktiviert haben, enthält die Verwaltungswebsite lediglich die **Seite mit Informationen des außer Betrieb gesetzten Servers**. Es werden also keine weiteren Verwaltungsaufgaben unterstützt. Sie müssen die folgenden Schritte ausführen, um die Außerbetriebsetzung des Servers abzuschließen:

1.  Weisen Sie der **RMS Service Group** (RMS-Dienstgruppe) die Berechtigungen zum Lesen und Ausführen zu.
2.  Fügen Sie die Gruppe **Jeder** mit Leseberechtigung zur DACL (Discretionary Access Control List oder Zugriffssteuerungsliste) der Datei „Decommissioning.asmx“ hinzu.
3.  Informieren Sie die Benutzer, dass die RMS-Installation außer Betrieb gesetzt wird, und raten Sie ihnen, eine Verbindung zum Server herzustellen, um die Inhalte ohne RMS-Schutz zu speichern.
4.  Konfigurieren Sie alle RMS-Anwendungen im Unternehmen für die Verbindung mit der Seite Decommissioning.asmx. Je nach RMS-fähiger Anwendung kann dies über einen Registrierungsschlüssel oder die Einstellung Gruppenrichtlinie gesteuert werden.
5.  Wenn eine Organisation RMS-fähige Anwendungen verwendet, die die Installation automatisch zum Veröffentlichen verwenden, sollten Sie mithilfe der Gruppenrichtlinie auf diesen Computern einen Registrierungseintrag festlegen, damit diese Anwendungen den Außerbetriebsetzungsdienst verwenden.
6.  Wenn Sie davon überzeugt sind, dass alle Inhalte ungeschützt vorliegen, sollten Sie eine Sicherungskopie des privaten Schlüssels des Servers anlegen und RMS vom Server deinstallieren.
