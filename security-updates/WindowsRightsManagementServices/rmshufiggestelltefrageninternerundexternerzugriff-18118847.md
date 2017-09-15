---
TOCTitle: 'RMS – Häufig gestellte Fragen: Interner und externer Zugriff'
Title: 'RMS – Häufig gestellte Fragen: Interner und externer Zugriff'
ms:assetid: '59c2c51f-6c20-450c-a334-0e1486292074'
ms:contentKeyID: 18118847
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747577(v=WS.10)'
---

RMS – Häufig gestellte Fragen: Interner und externer Zugriff
============================================================

Interner und externer RMS-Zugriff – Häufig gestellte Fragen
-----------------------------------------------------------

-   [Welche Änderungen muss ich vornehmen, damit meine Firewall RMS-Clients außerhalb der Firewall Zugriff auf RMS-Server gewährt?](#bkmk_37)
-   [Wie funktioniert das Extranetszenario?](#bkmk_38)
-   [Wenn ein Benutzer durch Rechte geschützte Inhalte erstellt und an einen anderen Benutzer weitergibt, der keinen Zugriff auf die RMS-Installation hat, kann dann dieser Benutzer die Inhalte abrufen?](#bkmk_39)
-   [Wenn ich meinen Kunden mit Outlook 2003 oder Outlook 2007 eine durch Rechte geschützte E-Mail sende, was benötigen die Kunden, um diese E-Mail zu lesen?](#bkmk_40)
-   [Wie können Organisationen, die jeweils eigene RMS-Server haben, durch Rechte geschützte Inhalte austauschen?](#bkmk_41)
-   [Wenn eine mit RMS geschützte E-Mail an eine andere Organisation gesendet wird, die Outlook nicht unterstützt, kann dann der Empfänger auf die E-Mail antworten, wenn sie mit dem Add-On für die Rechteverwaltung für Internet Explorer gelesen wird?](#bkmk_42)

<span id="BKMK_37"></span>
#### Welche Änderungen muss ich vornehmen, damit meine Firewall RMS-Clients außerhalb der Firewall Zugriff auf RMS-Server gewährt?

Die Firewall muss Computern außerhalb der Firewall erlauben, SOAP-Anforderungen (Simple Object Access Protocol) über HTTP (TCP-Port 80) bzw. über HTTPS (TCP-Port 443) an den RMS-Server zu senden.

<span id="BKMK_38"></span>
#### Wie funktioniert das Extranetszenario?

Die an den Inhalt gebundene Veröffentlichungslizenz enthält zwei URLs. Eine davon ist die Intranet-URL, die beim Bereitstellen des RMS-Clusters festgelegt wird. Die andere ist eine Extranet-URL, die vom RMS-Administrator festgelegt werden kann. Diese Extranet-URL ermöglicht dem Client den Erwerb von Nutzungslizenzen außerhalb der Firewall. Die Extranet-URL kann nicht zum Erstellen von durch Rechte geschützten Inhalten verwendet werden. In diesem Fall muss die Registrierung auf dem RMS-Client geändert werden.

<span id="BKMK_39"></span>
#### Wenn ein Benutzer durch Rechte geschützte Inhalte erstellt und an einen anderen Benutzer weitergibt, der keinen Zugriff auf die RMS-Installation hat, kann dann dieser Benutzer die Inhalte abrufen?

Wenn der Benutzer beim ersten Öffnen des geschützten Inhalts keine Verbindung zur RMS-Installation hat, kann er den Inhalt nicht abrufen.

Office 2003 und später erwirbt bei durch Rechte geschützten E-Mails im Zuge der Synchronisierung automatisch die entsprechenden Nutzungslizenzen, sodass diese E-Mails ohne Netzwerkverbindung gelesen werden können. Während Outlook 2003 und später jedoch die Nutzungslizenzen für eine E-Mail automatisch zwischenspeichert, werden den Excel 2007-, Excel 2003-, Word 2007-, Word 2003-, PowerPoint 2007- und PowerPoint 2003-Dokumenten, die der E-Mail eventuell angehängt sind, dieselben Rechte gewährt wie der E-Mail, mit der sie verschickt wurden. Sie werden beim Herunterladen der E-Mail nicht automatisch synchronisiert und müssen einzeln geöffnet werden, wenn der Computer mit dem Netzwerk verbunden ist, um die entsprechenden Nutzungslizenzen zu erwerben.

<span id="BKMK_40"></span>
#### Wenn ich meinen Kunden mit Outlook 2003 oder Outlook 2007 eine durch Rechte geschützte E-Mail sende, was benötigen die Kunden, um diese E-Mail zu lesen?

Der Empfänger muss entweder Outlook 2003, Outlook 2007 oder das Add-On für die Rechteverwaltung für Internet Explorer verwenden. Wenn zwischen Ihrer RMS-Installation und denen der Organisation des Empfängers eine Vertrauensstellung besteht, kann der Empfänger die E-Mail ohne weitere Schritte lesen. Die Vertrauensstellung wird aufgebaut, indem RMS-Server-Lizenzgeberzertifikate ausgetauscht werden, die die entsprechenden öffentlichen Schlüssel enthalten.

Wenn die Organisation des Empfängers keine RMS-Infrastruktur hat oder keine Vertrauensstellung besteht, können Sie Ihren Kunden bitten, eine Windows Live-ID einzurichten, und dann beim Senden der E-Mail an den Empfänger die Rechte angeben, die den Windows Live-ID-Anmeldeinformationen des Kunden zugeordnet sind. Bei diesem Verfahren wird der im Internet verfügbare Microsoft IRM-Dienst (Information Rights Management, Verwaltung von Informationsrechten) verwendet, um eine Nutzungslizenz zu erwerben. Der IRM-Dienst wird kostenlos als Testversion zur Verfügung gestellt und dient lediglich dazu, dass die Benutzer RMS testen können. Wenn Sie diesen Dienst verwenden, um geschützten Inhalt zu erstellen, sollten Sie damit rechnen, dass der Dienst eventuell in Zukunft ohne Vorankündigung eingestellt werden kann.

<span id="BKMK_41"></span>
#### Wie können Organisationen, die jeweils eigene RMS-Server haben, durch Rechte geschützte Inhalte austauschen?

RMS verwendet vertrauenswürdige Benutzerdomänen, d. h., die eine RMS-Installation vertraut den von einer anderen RMS-Installation erstellten Benutzerzertifikaten.

<span id="BKMK_42"></span>
#### Wenn eine mit RMS geschützte E-Mail an eine andere Organisation gesendet wird, die Outlook nicht unterstützt, kann dann der Empfänger auf die E-Mail antworten, wenn sie mit dem Add-On für die Rechteverwaltung für Internet Explorer gelesen wird?

Der E-Mail-Empfänger kann eine durch Rechte geschützte E-Mail genau so wie andere E-Mails beantworten, aber der ursprüngliche Hauptteil der empfangenen E-Mail bleibt für die ursprünglichen Empfänger durch Rechte geschützt. Die Struktur dieses E-Mail-Pakets wird von der Clientanwendung bestimmt. Die ursprüngliche E-Mail kann entweder als verschlüsselte Anlage an die Antwort angehängt oder auch vollständig entfernt werden, wie es beispielsweise in Outlook 2003 oder Outlook 2007 der Fall ist.
