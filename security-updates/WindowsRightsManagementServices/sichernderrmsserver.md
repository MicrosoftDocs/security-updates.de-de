---
TOCTitle: 'Sichern der RMS-Server'
Title: 'Sichern der RMS-Server'
ms:assetid: '7e6c4d3a-6cfb-4e96-9dda-ead83f961a6e'
ms:contentKeyID: 18118914
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747574(v=WS.10)'
---

Sichern der RMS-Server
======================

Mithilfe der folgenden Empfehlungen können Sie die Benutzerkonten und Sicherheitseinstellungen auf den RMS-Servern verwalten:

-   Die virtuellen Verzeichnisse der zum Verwalten von RMS verwendeten Website verfügen über freigegebene Zugriffssteuerungslisten (DACLs oder Discretionary Access Control Lists), die den Zugriff auf lokale Administratoren beschränken. Ein lokaler Administrator kann eine zusätzliche Sicherheitsgruppe erstellen, um den Zugriff durch Hinzufügen und Entfernen von Mitgliedern und durch Festlegen weiterer Einträge für die Zugriffssteuerung (ACEs oder Access Control Entries) auf den Verwaltungswebseiten noch stärker zu steuern.
-   Für höhere Sicherheit sollten die DACL-Einstellungen für die Webseite „Sicherheitseinstellungen“ (SecurityPolicy.aspx) geändert werden. Zum Zulassen einer Bereitstellung gewährt der Standard-ACE demjenigen Konto Vollzugriff, das RMS bereitstellt. Nach der Bereitstellung sollten Sie den ACE entweder für eine Einzelperson oder eine eingeschränkte Sicherheitsgruppe ändern.
-   Abgesehen von den Berechtigungen und Rechten für jeden RMS-Server sollten darüber hinaus besonders die Anforderungen zum Sichern der Konfigurationsdatenbank beachtet werden, die für das Sichern der gesamten Bereitstellung wichtig sind. Weitere Informationen finden Sie nachstehend unter [Sichern der Konfigurationsdatenbank](https://technet.microsoft.com/e023b96f-81d0-45fb-8cc5-becaf6d47ae1).

Weitere Informationen zum Sichern von Microsoft SQL Server™ finden Sie auf der Seite **SQL Server Security** auf der [Microsoft-Website](http://www.microsoft.com/)(http://www.microsoft.com/) (nur auf Englisch verfügbar).

Weitere Informationen zum Sichern von Computern, auf denen ein Betriebssystem der Microsoft Windows Server 2003-Produktfamilie ausgeführt wird, finden Sie im „Windows Server 2003 Security Guide“ im Microsoft Download Center auf der [Microsoft-Website](http://www.microsoft.com/)(http://www.microsoft.com/) (nur auf Englisch verfügbar).