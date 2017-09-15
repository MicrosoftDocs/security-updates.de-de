---
TOCTitle: Der Außerbetriebsetzungsvorgang
Title: Der Außerbetriebsetzungsvorgang
ms:assetid: '57bd9949-9433-437b-93ed-ffb2dff9992e'
ms:contentKeyID: 18118850
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720276(v=WS.10)'
---

Der Außerbetriebsetzungsvorgang
===============================

Über die Internetinformationsdienste (Internet Information Services oder IIS) von RMS können verschiedene angebotene Dienste eingesehen werden. So werden durch den Zertifizierungsdienst Benutzer und deren Computer registriert und durch den Lizenzierungsdienst Inhalte veröffentlicht und Zugriff auf RMS-geschützte Informationen gewährt. Ein zusätzlicher Dienst, der Außerbetriebsetzungsdienst, muss auf dem RMS-Server aktiviert werden, um den Vorgang der Außerbetriebssetzung zu initiieren. Ist der Außerbetriebsetzungsdienst aktiviert, sind sämtliche anderen RMS-Dienste, die vom Server bereitgestellt werden, deaktiviert.

Nachdem der RMS-Server zur Außerbetriebsetzung aktiviert wurde, können Anwendungen einen Inhaltsschlüssel vom Außerbetriebsetzungsdienst erhalten, mit dem sie RMS-geschützte Inhalte permanent entschlüsseln können.

Wenn der RMS-Server im Außerbetriebsetzungsmodus ausgeführt wird, kann jeder beliebige Benutzer, unabhängig davon, ob er Rechte auf den ursprünglichen RMS-geschützten Inhalt besitzt oder nicht, einen Inhaltsschlüssel und somit Vollzugriff auf den Inhalt erhalten.

Nach der Verschlüsselung des Inhalts empfiehlt es sich, den Inhalt ohne RMS-Schutz zu speichern. Bedenken Sie, dass für die Verwendung des Außerbetriebsetzungsdienstes eine Registrierung des Benutzers in der RMS-Infrastruktur erforderlich ist. Ein Benutzer ohne aktivierten RMS-Client kann den Außerbetriebsetzungsdienst nicht für den Zugriff auf RMS-geschützte Inhalte in Anspruch nehmen.
