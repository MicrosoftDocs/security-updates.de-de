---
TOCTitle: 'Schritt 4: Synchronisieren des Servers'
Title: 'Schritt 4: Synchronisieren des Servers'
ms:assetid: 'a5514e46-a50b-46a6-9e5b-33c87c5b7cef'
ms:contentKeyID: 18127559
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708523(v=WS.10)'
---

Schritt 4: Synchronisieren des Servers
======================================

Nach dem Konfigurieren der Netzwerkverbindung können Sie Updates erhalten. Standardmäßig ist WSUS so konfiguriert, dass wichtige Updates und Sicherheitsupdates für alle Microsoft-Produkte gedownloadet werden. Um Updates zu erhalten, müssen Sie den WSUS-Server *synchronisieren*.

Beim Synchronisieren kontaktiert der WSUS-Server Microsoft Update. Wenn der Kontakt hergestellt ist, ermittelt WSUS, ob seit der letzten Synchronisierung neue Updates zur Verfügung gestellt wurden. Da es sich hier um die erste Synchronisierung des WSUS-Servers handelt, sind alle Updates verfügbar und können von Ihnen für die Installation genehmigt werden.

| ![](images/Cc708523.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| In diesem Dokument ist das Synchronisieren der Standardeinstellungen beschrieben. WSUS beinhaltet jedoch auch Optionen, mit denen Sie den Bandbreitenverbrauch während der Synchronisierung minimieren können. Weitere Informationen finden Sie im Whitepaper "Bereitstellen von Microsoft Server Windows Update Services" (möglicherweise in englischer Sprache). |

**So synchronisieren Sie den WSUS-Server**
1.  Klicken Sie auf der Symbolleiste der WSUS-Konsole auf **Optionen** und dann auf **Synchronisierungsoptionen**.

2.  Klicken Sie unter **Aufgaben** auf **Jetzt synchronisieren**.

Klicken Sie nach Abschluss der Synchronisierung auf der Symbolleiste der WSUS-Konsole auf **Updates**, um die Liste der Updates anzuzeigen.
