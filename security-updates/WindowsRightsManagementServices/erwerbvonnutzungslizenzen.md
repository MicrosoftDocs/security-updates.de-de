---
TOCTitle: Erwerb von Nutzungslizenzen
Title: Erwerb von Nutzungslizenzen
ms:assetid: '0b6cde34-418a-4dee-9d27-b65b93b535ac'
ms:contentKeyID: 18118747
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720194(v=WS.10)'
---

Erwerb von Nutzungslizenzen
===========================

Wenn ein Benutzer RMS-geschützte Inhalte einsehen möchte, muss er eine Nutzungslizenz über den RMS-Lizenzierungsdienst anfordern. In der folgenden Abbildung wird der Prozess dargestellt, mit dem eine Nutzungslizenz angefordert und empfangen wird.

![](images/Cc720194.37b8d28c-9749-4e81-bc6a-22692fefb8b6(WS.10).gif)

Der Erwerb einer Nutzungslizenz verläuft in den folgenden Schritten:

1.  Der Benutzer erhält eine geschützte Datei auf einem der typischen Verteilungswege und öffnet sie mit einer RMS-fähigen Anwendung. Falls der Benutzer auf dem verwendeten Computer bzw. Gerät nicht über ein Rechtekontozertifikat verfügt, muss er ein solches erwerben.
2.  Die RMS-fähige Anwendung fordert eine Nutzungslizenz von dem Server an, der auch die Veröffentlichungslizenz für den betreffenden geschützten Inhalt ausgestellt hat. Die Anforderung umfasst das Rechtekontozertifikat des Benutzers einschließlich des öffentlichen Schlüssels, sowie die Veröffentlichungslizenz, die den symmetrischen Schlüssel des Inhalts enthält.
    Eine von einem Client-Lizenzgeberzertifikat ausgestellte Veröffentlichungslizenz schließt den URL des Servers ein, der das Zertifikat ausgestellt hat. In diesem Beispiel wird die Anforderung für eine Nutzungslizenz an den Server gesendet, der das Client-Lizenzgeberzertifikat ausgestellt hat, und nicht an den Computer, der die Veröffentlichungslizenz ausgestellt hat.
3.  Der Lizenzierungsserver überprüft, ob der Benutzer autorisiert und sein Name in der Veröffentlichungslizenz angegeben ist, und erstellt dann eine Nutzungslizenz. Der Server überprüft das Kontozertifikat des Benutzers und ermittelt anschließend, welche Berechtigungen dem Benutzer erteilt wurden ? entweder direkt oder als Mitglied einer Gruppe, der Berechtigungen erteilt wurden.
    Der Server entschlüsselt den symmetrischen Inhaltsschlüssel mit dem privaten Serverschlüssel, verschlüsselt ihn erneut mit dem öffentlichen Schlüssel des Empfängers und fügt ihn zu der Nutzungslizenz hinzu. Mit diesem Schritt wird sichergestellt, dass nur der vorgesehene Benutzer den Inhaltsschlüssel und die geschützten Inhalte entschlüsseln kann.
    Der Server fügt zu der Nutzungslizenz alle relevanten Bedingungen, wie z. B. einen Anwendungs- oder Windows-Versionsausschluss, hinzu. Diese Bedingungen werden vom Client erzwungen, sobald die Nutzungslizenz mit den RMS-geschützten Inhalten verbunden ist.
4.  Nach Abschluss der Überprüfung gibt der Lizenzierungsserver die Nutzungslizenz an den Clientcomputer des Benutzers zurück.