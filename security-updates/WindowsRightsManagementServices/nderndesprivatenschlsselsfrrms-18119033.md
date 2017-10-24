---
TOCTitle: Ändern des privaten Schlüssels für RMS
Title: Ändern des privaten Schlüssels für RMS
ms:assetid: 'da32137e-394a-42b2-9552-ba20f4547c23'
ms:contentKeyID: 18119033
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747765(v=WS.10)'
---

Ändern des privaten Schlüssels für RMS
======================================

Während der Bereitstellung erstellt RMS (Rights Management Services oder Dienste für die Rechteverwaltung) den privaten RMS-Schlüssel für den Server. Der private RMS-Schlüssel wird verschlüsselt und in der Konfigurationsdatenbank gespeichert. Sie sollten unbedingt eine Sicherungskopie des privaten Schlüssels anlegen und diese an einem sicheren Ort speichern. Darüber hinaus empfiehlt es sich, den privaten RMS-Schlüssel mithilfe eines Hardwaresicherheitsmoduls zu schützen, da der Schlüssel für die Verschlüsselungsschemata des gesamten vom Server mit RMS geschützten Inhalts verwendet wird. Wird der private Schlüssel von RMS gefährdet, müssen Sie die Bereitstellung von RMS auf dem Server beenden und es danach erneut bereitstellen, um einen neuen privaten Schlüssel von RMS zu erhalten.

Wurde der Server zum Inhaltsschutz verwendet, müssen alle Inhaltseigentümer benachrichtigt werden. Es empfiehlt sich, alle Inhalte auf dem RMS-Server mit dem neuen privaten Schlüssel erneut zu veröffentlichen. Kopien von Inhalten, die mit dem unsicheren Schlüssel geschützt wurden, sind nicht mehr ausreichend geschützt und sind zu zerstören.

| ![](images/Cc747765.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                                   |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Unabhängig davon, ob der Server beim Microsoft-Registrierungsdienst registriert wurde, muss der Bereitstellungsprozess zum Erhalt eines neuen privaten Schlüssels wiederholt werden. Wenn Sie einfach nur den Server mit RMS neu registrieren, wird der zuvor verwendete private Schlüssel weiterhin verwendet. |