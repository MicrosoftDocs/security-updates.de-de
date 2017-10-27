---
TOCTitle: Verwenden der Administratorengruppe
Title: Verwenden der Administratorengruppe
ms:assetid: '0febcb3e-7124-4e51-971a-1013b928d33b'
ms:contentKeyID: 18118751
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720198(v=WS.10)'
---

Verwenden der Administratorengruppe
===================================

Während der Bereitstellung erstellt RMS (Rights Management Services oder Dienste für die Rechteverwaltung) eine spezielle Administratorengruppe, die über Vollzugriff auf die gesamten geschützten Inhalte verfügt. Den Mitgliedern der Administratorengruppe werden volle Besitzerrechte in allen Nutzungslizenzen erteilt, die vom Server mit RMS oder vom Cluster, auf dem die Administratorengruppe konfiguriert ist, ausgestellt wurden. Dies bedeutet, dass Mitglieder dieser Gruppe beliebige Dateien mit geschützten Inhalten entschlüsseln und ihren Schutz entfernen können. Ein Mitglied dieser Gruppe kann beispielsweise den Schutz von Dateien entfernen, die von einem gekündigten Mitarbeiter veröffentlicht wurden, damit ein neuer Besitzer die Dateien veröffentlichen und verwalten kann.

Die Administratorengruppe hat keine standardmäßigen Mitglieder, nicht einmal Administratoren gehören ihr automatisch an. Auf der Verwaltungswebsite können Sie eine Active Directory-Sicherheitsgruppe angeben, die als Administratorengruppe für RMS verwendet werden soll. Sie können entweder eine vorhandene Active Directory-Gruppe verwenden oder eine neue Gruppe erstellen. Die Gruppe muss zu derselben Active Directory-Gesamtstruktur gehören wie die RMS-Installation. Allen Benutzerkonten, die Mitglied der als RMS-Administratorengruppe angegebenen Gruppe sind, werden automatisch die Berechtigungen der Administratorengruppe erteilt.

Weitere Informationen zum Angeben einer Administratorengruppe für RMS finden Sie nachstehend unter „[So richten Sie eine Administratorengruppe ein](https://technet.microsoft.com/f2ef847e-2824-471f-9079-5c343094aba8)“.

| ![](images/Cc720198.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Die Gruppe, die Sie als Administratorengruppe für RMS angeben, muss zuvor bereits in derselben Active Directory-Gesamtstruktur wie die RMS-Installation vorhanden sein. Die Eigenschaften dieser Gruppe müssen eine E-Mail-Adresse umfassen, die einen voll gekennzeichneten Domänennamen (Fully Qualified Domain Name oder FQDN) einschließt. Dieser muss mit dem Kontonamen übereinstimmen. Die E-Mail-Adresse muss folgendes Format aufweisen: *Gruppenname*@*Domänenname*. |