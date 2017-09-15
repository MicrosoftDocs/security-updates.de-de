---
TOCTitle: Alternativen zur Außerbetriebsetzung von RMS
Title: Alternativen zur Außerbetriebsetzung von RMS
ms:assetid: '4d32f35e-997d-4d10-ab66-efe217e853f7'
ms:contentKeyID: 18118839
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720268(v=WS.10)'
---

Alternativen zur Außerbetriebsetzung von RMS
============================================

Wenn Sie RMS in Ihrer Organisation weiter einsetzen, jedoch bestimmte RMS-Server aus einem beliebigen Grund nicht mehr benutzen möchten, sollten Sie die folgenden Alternativen zur Außerbetriebsetzung in Betracht ziehen.

**Einrichten einer vertrauenswürdigen Veröffentlichungsdomäne**

Sämtliche RMS-geschützten Informationen werden mit dem privaten Schlüssel des RMS-Servers verschlüsselt. Eine vertrauenswürdige Veröffentlichungsdomäne ermöglicht Ihnen den Import des privaten Schlüssels eines RMS-Servers in einen anderen RMS-Server. Dadurch kann ein RMS-Server Nutzungslizenzen gegen Veröffentlichungslizenzen ausstellen, die von einem anderen RMS-Server erstellt wurden. Nach dem Export des Schlüssels kann der Server aus dem System entfernt und deinstalliert werden.

**Einrichten von Administratorengruppen**

Wenn RMS-geschützte Inhalte nicht geöffnet werden können, weil kein Benutzer entsprechende Rechte besitzt, können Sie Vollzugriff auf die gesamten RMS-geschützten Inhalte gewähren, die von diesem Server für die Administratorengruppe veröffentlicht werden. Den Mitgliedern der Administratorengruppe werden volle Besitzerrechte in allen Nutzungslizenzen erteilt, die vom Server mit RMS oder vom Cluster, auf dem die Administratorengruppe konfiguriert ist, ausgestellt wurden. Dies bedeutet, dass Mitglieder dieser Gruppe beliebige Dateien mit geschützten Inhalten entschlüsseln und ihren Schutz entfernen können. Ein Mitglied dieser Gruppe kann beispielsweise den Schutz von Dateien entfernen, die von einem gekündigten Mitarbeiter veröffentlicht wurden, damit ein neuer Besitzer die Dateien veröffentlichen und verwalten kann.

Die Administratorengruppe schließt nicht automatisch Mitglieder ein. Dies gilt auch für Administratoren. Diese Gruppe muss im Active Directory als Verteilungsgruppe mit einem E-Mail-Adressenattribut vorhanden sein, das denselben Wert wie der Gruppenname im Format „*gruppenname*@*domänenname*.com“ aufweist. Der Gruppenname muss dem E-Mail-Adressenattribut genau entsprechen, und Groß-/Kleinschreibung muss beachtet werden.
