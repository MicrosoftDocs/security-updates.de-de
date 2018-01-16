---
TOCTitle: 'RMS-Verschlüsselung und -Schlüssel'
Title: 'RMS-Verschlüsselung und -Schlüssel'
ms:assetid: '6ed69817-dab0-4845-b2a4-74203f95f7cf'
ms:contentKeyID: 18118873
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747615(v=WS.10)'
---

RMS-Verschlüsselung und -Schlüssel
==================================

Geschützte Inhalte sind immer verschlüsselt. Auch die in RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwendeten Zertifikate und Lizenzen können verschlüsselten Inhalt enthalten, der nur von einer berechtigten Entität entschlüsselt werden kann. Eine RMS-fähige Anwendung verwendet einen Inhaltsschlüssel, um Daten zu verschlüsseln. Alle Server, Clientcomputer und Benutzerkonten für RMS SP1 haben ein 1024-Bit-RSA-Schlüsselpaar (Rivest-Shamir-Adleman). Diese Schlüssel dienen RMS zur Verschlüsselung des in Veröffentlichungs- und Nutzungslizenzen enthaltenen Inhaltsschlüssels sowie zum Signieren von RMS-Zertifikaten und -Lizenzen. Auf diese Weise wird sichergestellt, dass der Server nur autorisierten Benutzern und Computern Zugriffsberechtigungen erteilt.

Dieser Abschnitt behandelt die folgenden Themen:

-   [RMS-Schlüsseldefinitionen](https://technet.microsoft.com/b052305c-1db7-434a-bad9-26d704156776)
-   [RMS-Serverschlüssel](https://technet.microsoft.com/5f4100a1-9aa5-42af-85c8-4bc691022f06)
-   [RMS-Computerschlüssel](https://technet.microsoft.com/56e59ec2-f681-4ca2-98c7-72218ab9e9d9)
-   [Client-Lizenzgeberschlüssel](https://technet.microsoft.com/28781125-2692-4ff9-99b1-e09227d72966)
-   [Benutzerschlüssel](https://technet.microsoft.com/12dad6e2-64e7-4bab-bde7-b72f90f5cb05)
-   [RMS-Inhaltsschlüssel](https://technet.microsoft.com/63c814bf-2809-477e-a2db-d90370442075)