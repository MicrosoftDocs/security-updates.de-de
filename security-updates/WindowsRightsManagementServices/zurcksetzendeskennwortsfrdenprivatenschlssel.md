---
TOCTitle: Zurücksetzen des Kennworts für den privaten Schlüssel
Title: Zurücksetzen des Kennworts für den privaten Schlüssel
ms:assetid: 'ceba927e-a7fd-4b06-bb70-5e5d9d6d099c'
ms:contentKeyID: 18119032
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747675(v=WS.10)'
---

Zurücksetzen des Kennworts für den privaten Schlüssel
=====================================================

Wählen Sie beim Bereitstellen eines Servers eine Methode zum Schützen des privaten Schlüssels von RMS (Rights Management Services oder Dienste für die Rechteverwaltung) aus. Bei Auswahl der Standardoption, einen softwarebasierten Schutz für den privaten Schlüssel zu verwenden, haben Sie ein sicheres Kennwort angegeben, mit dem der private Schlüssel des Servers in der Konfigurationsdatenbank verschlüsselt wurde. Wenn das Kennwort verloren oder vergessen wurde, kann es von einem Mitglied der Administratorengruppe zurückgesetzt werden. Dies ist unten unter [So setzen Sie das Kennwort für den privaten Schlüssel zurück](https://technet.microsoft.com/f71df255-fe19-4e07-810e-87309a5e8e88) beschrieben.

Wird RMS in einer Clusterumgebung ausgeführt, müssen Sie den privaten Schlüssel auf jedem Frontendserver mit RMS in Ihrer Installation zurücksetzen. Unterlassen Sie dies, arbeiten diese Server nicht ordnungsgemäß und können den Serverschlüssel in der Konfigurationsdatenbank nicht entschlüsseln.

Weitere Informationen zum Verwenden von sicheren Kennwörtern finden Sie im Windows Server 2003 Hilfe- und Supportcenter.