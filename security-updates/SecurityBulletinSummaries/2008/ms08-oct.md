---
TOCTitle: 'MS08-OCT'
Title: Microsoft Security Bulletin Summary für Oktober 2008
ms:assetid: 'ms08-oct'
ms:contentKeyID: 61225065
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms08-oct(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Oktober 2008
====================================================

Veröffentlicht: Dienstag, 14. Oktober 2008 | Aktualisiert: Donnerstag, 23. Oktober 2008

**Version:** 3.0

In diesem Bulletin Summary sind die im Oktober 2008 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Oktober 2008 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 9. Oktober 2008 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am 15. Oktober 2008 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im Oktober.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374639) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

Für das außerplanmäßige Security Bulletin, das in Version 3.0 dieser Bulletin Summary hinzugefügt wurde, stellt Microsoft am 23. Oktober 2008 um 11:00 Uhr pazifischer Zeit (USA & Kanada) einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Webcast zum außerplanmäßigen Bulletin.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032393978&eventcategory=4&culture=en-us&countrycode=us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

Die Security Bulletins für diesen Monat, nach Schweregrad geordnet:

Kritisch (5)
------------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-067                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit im Serverdienst kann Remotecodeausführung ermöglichen (958644)**](http://go.microsoft.com/fwlink/?linkid=130719)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Serverdienst. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein betroffenes System eine speziell gestaltete RPC-Anforderung erhält. Auf Systemen mit Microsoft Windows 2000, Windows XP und Windows Server 2003 kann ein Angreifer diese Sicherheitsanfälligkeit ohne Authentifizierung ausnutzen, um beliebigen Code auszuführen. Diese Sicherheitsanfälligkeit kann bei der Gestaltung einer als Computerwurm verwendbaren Ausnutzung verwendet werden. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerkressourcen vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-060                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Active Directory kann Remotecodeausführung ermöglichen (957280)**](http://go.microsoft.com/fwlink/?linkid=128125)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Implementierungen von Active Directory unter Microsoft Windows 2000 Server. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer Zugang zu einem betroffenen Netzwerk erlangt. Diese Sicherheitsanfälligkeit betrifft nur Microsoft Windows 2000-Server, die konfiguriert wurden, um als Domänencontroller zu fungieren. Wenn ein Microsoft Windows 2000-Server nicht zu einem Domänencontroller heraufgestuft wurde, ist er nicht bereit, LDAP-Abfragen (Lightweight Directory Access-Protokoll) oder LDAPS-Abfragen (LDAP über SSL) zu empfangen, und ist nicht von dieser Sicherheitsanfälligkeit betroffen. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-058                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Kumulatives Sicherheitsupdate für Internet Explorer (956390)**](http://go.microsoft.com/fwlink/?linkid=128060)                                                                                                                                                                                                                                                                                                                                                                                   |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete und eine öffentlich gemeldete Sicherheitsanfälligkeit. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, können die Sicherheitsanfälligkeiten Offenlegung von Informationen bzw. Remotecodeausführung ermöglichen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                                                  |
| **Betroffene Software:**                    | **Microsoft Windows, Internet Explorer.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                 |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-059                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit im RPC-Dienst des Host Integration Servers kann Remotecodeausführung ermöglichen (956695)**](http://go.microsoft.com/fwlink/?linkid=125712)                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Host Integration Server. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete RPC-Anforderung (Remote Procedure Call, Remoteprozeduraufruf) an ein betroffenes System sendet. Benutzer, die die empfohlenen Vorgehensweisen befolgen und das SNA RPC-Dienstkonto mit weniger Benutzerrechten auf dem System konfigurieren, sind u. U. weniger stark betroffen als Benutzer, die das SNA RPC-Dienstkonto mit administrativen Benutzerrechten konfigurieren. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Betroffene Software:**                    | **Microsoft Host Integration Server.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-057                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (956416)**](http://go.microsoft.com/fwlink/?linkid=124653)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office Excel, die eine Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist kein Neustart des Computers erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Betroffene Software:**                    | **Microsoft Office.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

Hoch (6)
--------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-066                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit im Microsoft-Treiber für zusätzliche Funktionen kann Erhöhung von Berechtigungen ermöglichen (956803)**](http://go.microsoft.com/fwlink/?linkid=125709)                                                                                                                                                                                                                                                                                      |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft-Treiber für zusätzliche Funktionen (Ancillary Function Driver, AFD). Nutzt ein lokaler Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                         |
| **Auswirkung der Sicherheitsanfälligkeit:** | Erhöhung von Berechtigungen                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                      |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                        |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-061                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (954211)**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx)                                                                                                                                                                                                              |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine öffentlich gemeldete und zwei vertraulich gemeldete Sicherheitsanfälligkeiten im Windows-Kernel. Nutzt ein lokaler Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                     |
| **Auswirkung der Sicherheitsanfälligkeit:** | Erhöhung von Berechtigungen                                                                                                                                                                                                                                                                                                                                                                         |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                  |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                    |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-062                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit im Windows-Internetdruckdienst kann Remotecodeausführung ermöglichen (953155)**](http://go.microsoft.com/fwlink/?linkid=120829)                                                                                                                                                                                                                                                                                   |
| **Kurzzusammenfassung**                     | Dieses Update behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Windows-Internetdruckdienst, die Remotecodeausführung ermöglichen kann. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Berechtigungen erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                              |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                           |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                             |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-063                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in SMB kann Remotecodeausführung ermöglichen (957095)**](http://go.microsoft.com/fwlink/?linkid=127994)                                                                                                                                                                                                                                                                                                                                                |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft SMB-Protokoll (Server Message Block). Die Sicherheitsanfälligkeit kann Remotecodeausführung auf einem Server ermöglichen, auf dem Dateien oder Ordner freigegeben werden. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit vollständigen Benutzerrechten erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                                |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                  |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-064                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit bei Virtual Address Descriptor-Änderung kann Erhöhung von Berechtigungen ermöglichen (956841)**](http://go.microsoft.com/fwlink/?linkid=128103)                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Virtual Address Descriptor. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer eine speziell gestaltete Anwendung ausführt. Ein authentifizierter Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann auf einem betroffenen System eine Erhöhung von Berechtigungen erreichen. Ein Angreifer kann dann Programme installieren; Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Auswirkung der Sicherheitsanfälligkeit:** | Erhöhung von Berechtigungen                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-065                                                                                                                                                                                                                                                        |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Message Queuing kann Remotecodeausführung ermöglichen (951071)**](http://go.microsoft.com/fwlink/?linkid=128102)                                                                                                                                              |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Message Queuing-Dienst (MSMQ) auf Microsoft Windows 2000-Systemen. Die Sicherheitsanfälligkeit kann Remotecodeausführung auf Microsoft Windows 2000-Systemen mit aktiviertem MSMQ-Dienst ermöglichen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                             |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                        |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                          |
| **Betroffene Software:**                    | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                            |

Mittel (1)
----------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-056                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Microsoft Office kann Offenlegung von Informationen ermöglichen (957699)**](http://go.microsoft.com/fwlink/?linkid=128145)                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer auf eine speziell gestaltete CDO-URL klickt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann in den Browser des Benutzers ein clientseitiges Skript injizieren, das Inhalte vortäuschen, Informationen offenlegen oder Aktionen ausführen kann, zu denen ein Benutzer auf der betroffenen Website berechtigt ist. |
| **Bewertung des maximalen Schweregrads:**   | [Mittel](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Auswirkung der Sicherheitsanfälligkeit:** | Offenlegung von Informationen                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist kein Neustart des Computers erforderlich.                                                                                                                                                                                                                                                                                                                                                                                        |
| **Betroffene Software:**                    | **Microsoft Office.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                          |

Ausnutzbarkeitsindex
--------------------

**Wie verwende ich diese Tabelle?**  

Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzungsindex](http://technet.microsoft.com/en-us/security/cc998259.aspx).

| Kennung des Bulletins                                                                   | Titel des Bulletins                                                                                                                                                                | CVE-ID        | Ausnutzbarkeitsindex – Bewertung                                                                                 | Wichtige Hinweise                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|-----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [MS08-056](http://go.microsoft.com/fwlink/?linkid=128145)                               | [Sicherheitsanfälligkeit in Microsoft Office kann Offenlegung von Informationen ermöglichen (957699)](http://go.microsoft.com/fwlink/?linkid=128145)                               | CVE-2008-4020 | [2 – Inkonsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)     | Es könnte funktionierender Angreifercode erstellt werden. Die Auswirkungen auf den Schweregrad sind jedoch begrenzt, da die Sicherheitsanfälligkeit nur in bestimmten Webanwendungsszenarien Spoofing in einem Dialogfeld ermöglicht. Deshalb wird dieses Problem von Angreifern möglicherweise weitgehend ignoriert.                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653)                               | [Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                                     | CVE-2008-4019 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653)                               | [Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                                     | CVE-2008-3471 | [2 – Inkonsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653)                               | [Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                                     | CVE-2008-3477 | [2 – Inkonsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060)                               | [Kumulatives Sicherheitsupdate für Internet Explorer (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                                      | CVE-2008-2947 | (Öffentlich bei Veröffentlichung des Bulletins)                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060)                               | [Kumulatives Sicherheitsupdate für Internet Explorer (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                                      | CVE-2008-3472 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060)                               | [Kumulatives Sicherheitsupdate für Internet Explorer (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                                      | CVE-2008-3473 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060)                               | [Kumulatives Sicherheitsupdate für Internet Explorer (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                                      | CVE-2008-3475 | [2 – Inkonsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060)                               | [Kumulatives Sicherheitsupdate für Internet Explorer (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                                      | CVE-2008-3474 | [3 – Funktionierender Angreifercode unwahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060)                               | [Kumulatives Sicherheitsupdate für Internet Explorer (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                                      | CVE-2008-3476 | [3 – Funktionierender Angreifercode unwahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-059](http://go.microsoft.com/fwlink/?linkid=125712)                               | [Sicherheitsanfälligkeit im RPC-Dienst des Host Integration Servers kann Remotecodeausführung ermöglichen (956695)](http://go.microsoft.com/fwlink/?linkid=125712)                 | CVE-2008-3466 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | Obwohl wahrscheinlich nur bestimmte Arten von Unternehmenskunden Host Integration Server installieren würden, ist es wahrscheinlich, dass funktionierender Angreifercode erstellt wird.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [MS08-060](http://go.microsoft.com/fwlink/?linkid=128125)                               | [Sicherheitsanfälligkeit in Active Directory kann Remotecodeausführung ermöglichen (957280)](http://go.microsoft.com/fwlink/?linkid=128125)                                        | CVE-2008-4023 | [2 – Inkonsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)     | Es ist wahrscheinlich, dass die Sicherheitsanfälligkeit ausgelöst wird, um eine Denial-of-Service-Bedingung zu verursachen. Die Erstellung funktionierenden Angreifercodes zum Erreichen einer Remotecodeausführung ist jedoch schwierig, da es nicht möglich ist, eine benötigte Schreibadresse zu kontrollieren.                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| [MS08-061](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx) | [Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (954211)](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx) | CVE-2008-2250 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-061](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx) | [Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (954211)](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx) | CVE-2008-2252 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | Funktionierender Angreifercode wird höchstwahrscheinlich für Mehrprozessorsysteme erstellt werden.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| [MS08-061](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx) | [Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (954211)](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx) | CVE-2008-2251 | [3 – Funktionierender Angreifercode unwahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Ein Auslösen der Sicherheitsanfälligkeit ist möglich. Das Erstellen eines erfolgreichen, funktionierenden Angreifercodes ist aber sehr schwierig.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [MS08-062](http://go.microsoft.com/fwlink/?linkid=120829)                               | [Sicherheitsanfälligkeit im Windows-Internetdruckdienst kann Remotecodeausführung ermöglichen (953155)](http://go.microsoft.com/fwlink/?linkid=120829)                             | CVE-2008-1446 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | Konsistenter Angreifercode wurde in begrenzten, gezielten Angriffen entdeckt. Obwohl der IPP-Dienst (Internet Printing-Protokoll) standardmäßig aktiviert ist, erfordert der Zugriff auf diesen Dienst mittels IIS auf allen Plattformen standardmäßig auch eine Authentifizierung.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-063](http://go.microsoft.com/fwlink/?linkid=127994)                               | [Sicherheitsanfälligkeit in SMB kann Remotecodeausführung ermöglichen (957095)](http://go.microsoft.com/fwlink/?linkid=127994)                                                     | CVE-2008-4038 | [2 – Inkonsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-064](http://go.microsoft.com/fwlink/?linkid=128103)                               | [Sicherheitsanfälligkeit bei Virtual Address Descriptor-Änderung kann Erhöhung von Berechtigungen ermöglichen (956841)](http://go.microsoft.com/fwlink/?linkid=128103)             | CVE-2008-4036 | [2 – Inkonsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-065](http://go.microsoft.com/fwlink/?linkid=128102)                               | [Sicherheitsanfälligkeit in Message Queuing kann Remotecodeausführung ermöglichen (951071)](http://go.microsoft.com/fwlink/?linkid=128102)                                         | CVE-2008-3479 | [3 – Funktionierender Angreifercode unwahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Obwohl eine Offenlegung von Information möglich sein kann, ist es nicht immer möglich, nützlichen Inhalt aus dem Speicher abzurufen. Das Problem der Speicherbeschädigung kann ausgelöst werden, aber eine Remotecodeausführung ist schwierig.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| [MS08-066](http://go.microsoft.com/fwlink/?linkid=125709)                               | [Sicherheitsanfälligkeit im Microsoft-Treiber für zusätzliche Funktionen kann Erhöhung von Berechtigungen ermöglichen (956803)](http://go.microsoft.com/fwlink/?linkid=125709)     | CVE-2008-3464 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [MS08-067](http://go.microsoft.com/fwlink/?linkid=130719)                               | [Sicherheitsanfälligkeit im Serverdienst kann Remotecodeausführung ermöglichen (958644)](http://go.microsoft.com/fwlink/?linkid=130719)                                            | CVE-2008-4250 | [1 – Konsistenter Angreifercode wahrscheinlich](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | Konsistenter Angreifercode wurde in begrenzten, gezielten Angriffen entdeckt, die Windows XP und Windows Server 2003 betreffen. Dieser Dienst ist standardmäßig auf allen betroffenen Plattformen aktiviert, doch die Ausnutzung ist unter Microsoft Windows 2000, Windows XP und Windows Server 2003 am Wahrscheinlichsten. Standardmäßige Installationen von Windows Vista und Windows Server 2008 erfordern Authentifizierung aufgrund von Schutzmechanismen, die als Teil der Benutzerkontensteuerung eingeführt wurden und die zusätzliche Integritätsebenen durchsetzen. Dieser Schutz besteht auch, wenn die UAC-Eingabeaufforderung deaktiviert ist. Selbst nach der Authentifizierung erschweren Verbesserungen von ASLR und DEP die Ausnutzung. |

Betroffene Software und Downloadadressen
----------------------------------------

**Wie verwende ich diese Tabelle?**  

In dieser Tabelle finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Sie sollten jedes aufgeführte Softwareprogramm und jede Komponente überprüfen, um zu sehen, ob Sicherheitsupdates erforderlich sind. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.

**Hinweis**: Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Prüfen Sie für jede aufgeführte Kennung der Bulletins die gesamte Spalte, um basierend auf den in Ihrem System installierten Programmen und Komponenten alle Updates zu finden, die Sie installieren müssen.

#### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=e22eb3ae-1295-4fe2-9775-6f43c5c2aed3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Active Directory unter Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8ed7bb9a-4b26-49d7-8c14-60226d2bc20d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=257c0478-56dd-42eb-a90e-607d01613db7)  
(Kritisch)  
[Microsoft Internet Explorer 6 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=02390258-08e9-4b75-960d-be081b749558)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=3a6165a6-d7e7-4526-9291-290caf0639b4)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8163d1f6-feb5-4f39-8134-3ed42326b822)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9ed29c3a-0682-4586-bbc2-a73deaa18e4c)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=899e2728-2433-4ccb-a195-05b5d65e5469)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=0d5f9b6e-9265-44b9-a376-2067b73d6a03)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a7f0f47b-b1ee-4516-9fbf-bf8e579963d0)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4e73de2b-05e6-4901-9bac-46d8f469e635)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=b16d9dac-c430-4dd8-a1e5-9a614801f1d9)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=7718bf14-c26c-43f3-be67-4c79ab5b2607)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e7ef571f-c9e8-4e14-95a3-3eeaec55b784)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2f7e5981-6eef-4f08-86c0-c6a7607ea5d0)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=25997b73-a640-49c1-b19e-768a18bbe22c)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4c16a372-7bf8-4571-b982-dac6b2992b25)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=234c05fb-988b-4e02-aab6-bb23e447df3d)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ccf7a3e3-ec30-4b95-9a86-00032301513c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5b607efc-c6fb-4079-8478-e4f3262386d3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b06d3a02-b6e4-4d40-913a-3759a31f20f3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3ae4b913-bff0-4974-b198-828ca10d2a87)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4e1675eb-6b06-48e9-9765-23a2c7737bdc)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=50fae854-0bde-46f8-9444-b9e0d9bfecad)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f26d395d-2459-4e40-8c92-3de1c52c390d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ae8d22d5-20aa-471d-a423-f54c9d75febe)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=feaf2adf-7892-4dbf-a147-db4d5dbe52f3)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ee88ff2d-1b12-4f4c-a081-9f27a6fba074)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6e696762-d652-4a8f-ab8f-622f9746c320)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=437a9b68-6a0c-48c8-9348-0d6fda48aa21)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=dbbebb3f-f1c7-402c-bd16-6f88da0d042c)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e8ef3d5f-dd8e-4945-92cd-9d3e30b16667)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c04d2afb-f9d0-4e42-9e1f-4b944a2de400)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=07fc88c4-2571-4a4d-b573-ae576798ab4c)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=319dba34-07ca-47f9-a1e9-20df2df7966b)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ab4d94d3-458c-4946-ab7f-03a279629d25)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=57ca28ea-e5e1-4191-a3d6-84aa90a3d668)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d3df6508-a568-449d-ac97-fbf3f97b98ef)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=989ac6f1-515c-467d-a200-2aabe66d9319)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c2e754f9-086a-494c-bc19-5feed7df8b65)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ab590756-f11f-43c9-9dcc-a85a43077acf)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b68937af-f04a-4d1e-9d7f-ec92af5194de)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=47381d91-4a14-4a09-96b3-3345155df52d)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=63234f85-6e5d-4ef6-b7cf-d1d2c78a5517)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=1e6c3f81-85bb-48e6-a5af-635a7e540c93)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=748f54f1-40b9-407c-9819-909061b53743)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=91589cfb-15ba-4dd2-9e3b-107899fbcba6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5a3832ec-3f8f-42c1-a603-b1330d527547)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista und Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=18fdff67-c723-42bd-ac5c-cac7d8713b21)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4756e04b-6e1c-4d78-a3c0-17f6b4b97975)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3483b400-cedc-441f-ba8e-594e3df89190)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=9b5995df-a3b8-4e81-b118-9bb057e19884)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=72dd6015-25d1-45f4-a769-88ac43074b44)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b4212db5-093e-497d-b999-2e3780f9f7c2)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=a976999d-264f-4e6a-9bd6-3ad9d214a4bd)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bd19c72b-4f83-47ab-93be-d2c286e732c4)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=905ab030-14a5-4a3d-aa11-e8f957f6a1ea)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=4a0fcf4b-eb8e-456a-b934-400ae18248ee)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f793af16-5464-4db1-a42b-1c5f17c538ed)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c20808cb-c30a-4b53-91e5-810eb6b4b2e3)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-061.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=25c17b07-1efe-43d7-9b01-3dfdf1ce0bd7)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ec73f416-2204-42d6-8932-c96578ac819f)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8b97114a-71aa-47a2-b9e7-f4e158c18c80)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3d6290d8-1745-4bc0-9ca9-eeb1ad0be4a5)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=cf6744e6-b54c-40f6-a78d-7ba9453133c0)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ec9eeb82-0497-4c55-94bb-9a47cb3521b4)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=7b12018e-0cc1-4136-a68c-be4e1633c8df)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=defamilyid=baacd1c2-9764-4fea-bd4d-c49791974fef)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6e641db2-90c8-458f-9795-3e46b70a5203)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a33c833c-d5c5-4e37-8f89-7b9079f92e59)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=223236e8-7b19-4b47-8a90-bfc35eb9318a)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0bc178b8-f8ae-4f41-8f88-fb6a75be1bca)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=2bcf89ef-6446-406c-9c53-222e0f0baf7a)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=250a45dd-7eae-4440-bd10-02a703940976)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b6546e1c-bf7b-4354-8574-6c16fa707de0)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=31783e88-76e2-4bc6-b4ae-308443c6d223)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=077b697c-04a0-45bd-b08c-331d5c30cb47)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0af72663-4945-4916-8c55-090ba4d82793)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**\*Die Server Core-Installation von Windows Server 2008 ist betroffen.** Für unterstützte Editionen von Windows Server 2008 gilt dieses Update mit der gleichen Bewertung des Schweregrads. Dabei spielt es keine Rolle, ob Windows Server 2008 mit der Server Core-Installationsoption installiert wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**\*\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch diese Updates behobenen Sicherheitsanfälligkeiten betreffen keine unterstützten Editionen von Windows Server 2008, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office Suites, Systeme und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2000 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1b2740e0-ecdd-48ca-84e0-eb187c31eb16)  
(KB955461)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=27cedef1-c47c-472c-a343-cd9b4ebc2bba)  
(KB955464)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b1aee2d5-bfa0-40e3-91b6-98bf65524e8c)  
(KB956464)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 und Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Hoch)  
[Excel 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office System 2007 und Microsoft Office System 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Excel 2007](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Hoch)  
[Excel 2007 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ba4fa21a-7e01-4ef8-9b9f-9d51d00ef094)  
(KB958312)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?displaylang=defamilyid=e70c5ae0-2858-46de-81f8-dcd1786656b7)  
(KB958267)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Open XML-Dateiformatkonverter für Mac
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2a8d9a3b-b8a4-43b6-82a6-a2e7d16ae11d)  
(KB958304)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Hoch)  
[Microsoft Office Excel Viewer 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Hoch)  
[Microsoft Office Excel Viewer](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=83c88444-75b8-44d1-b280-3671394ade45)  
(KB955935)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Hoch)  
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Hoch)  
[Microsoft Office SharePoint Server 2007 Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Hoch)  
[Microsoft Office SharePoint Server 2007 x64 Edition](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Hoch)  
[Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
\*Dieses Update gilt für Server, auf denen Excel Services installiert sind, z. B. die Standardkonfiguration von Microsoft Office SharePoint Server 2007 Enterprise und Microsoft Office SharePoint Server 2007 für Websites. Microsoft Office SharePoint Server 2007 Standard enthält Excel Services nicht.

#### Microsoft Server Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Host Integration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-059**](http://go.microsoft.com/fwlink/?linkid=125712)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2000
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2000 Service Pack 2 (Server)](https://www.microsoft.com/download/details.aspx?familyid=11cca58b-59a4-4e93-9eb1-19b07c290a10)  
(Kritisch)  
[Microsoft Host Integration Server 2000 Administrator Client](https://www.microsoft.com/download/details.aspx?familyid=41b49291-1231-4e23-aef7-818207453d56)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2004 (Server)](https://www.microsoft.com/download/details.aspx?familyid=9ca255ed-9334-4848-af94-49ef3078cdc0)  
(Kritisch)  
[Microsoft Host Integration Server 2004 Service Pack 1 (Server)](https://www.microsoft.com/download/details.aspx?familyid=eca756a1-ca56-4481-b23c-53c159a4e08c)  
(Kritisch)  
[Microsoft Host Integration Server 2004 (Client)](https://www.microsoft.com/download/details.aspx?familyid=92cb54e7-f4ff-40a4-99cb-6257c4d8d4cd)  
(Kritisch)  
[Microsoft Host Integration Server 2004 Service Pack 1 (Client)](https://www.microsoft.com/download/details.aspx?familyid=d776515c-09aa-4a04-876d-606bfc26a006)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2006 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=1ae79da3-ec17-4d4b-8011-d777a237ac93)  
(Kritisch)  
[Microsoft Host Integration Server 2006 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=05da4540-4976-458a-a612-7385d78695a2)  
(Kritisch)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Security Center](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch über [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](http://office.microsoft.com/de-de/downloads/default.aspx) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) und das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](http://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection-Tool für eine breite Unterstützung bei der Erkennung und dem Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), die im [Anwendungskompatibilitäts-Toolkit 5.0](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Anwendungskompatibilitäts-Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services für 2008. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214,aspx).

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   [NetAgent Co., Ltd.](http://www.netagent.co.jp/) für den Hinweis auf ein in MS08-056 beschriebenes Problem.
-   Joshua J. Drake von [iDefense](http://labs.idefense.com/) für den Hinweis auf ein in MS08-057 beschriebenes Problem.
-   Wushi in Zusammenarbeit mit [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS08-057 beschriebenes Problem.
-   Lionel d'Hauenens von [Labo Skopia](http://www.laboskopia.com/), der mit dem [iDefense VCP](http://labs.idefense.com/) zusammenarbeitet, für den Hinweis auf ein in MS08-057 beschriebenes Problem.
-   David Bloom für den Hinweis auf ein in MS08-058 beschriebenes Problem.
-   Gregory Rubin für den Hinweis auf ein in MS08-058 beschriebenes Problem.
-   [Ivan Fratric](http://ifsec.blogspot.com/), der mit [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in MS08-058 beschriebenes Problem.
-   Thierry Zoller von [n.runs](http://www.nruns.com/) für den Hinweis auf ein in MS08-058 beschriebenes Problem.
-   Lee Dagon von [Composica](http://www.composica.com/) für den Hinweis auf ein in MS08-058 beschriebenes Problem.
-   Stephen Fewer von [Harmony Security](http://www.harmonysecurity.com/), der mit [iDefense VCP](http://labs.idefense.com/) zusammenarbeitet, für den Hinweis auf ein in MS08-059 beschriebenes Problem.
-   Paul Miseiko von [nCircle](http://www.ncircle.com/) für den Hinweis auf ein in MS08-060 beschriebenes Problem.
-   Paul Caton von [iShadow](http://www.ishadow.com/) für den Hinweis auf ein in MS08-061 beschriebenes Problem.
-   Thomas Garnier von [SkyRecon](http://www.skyrecon.com/) für den Hinweis auf ein in MS08-061 beschriebenes Problem.
-   [CERT/CC](http://www.cert.org/) für den Hinweis auf ein in MS08-062 beschriebenes Problem.
-   Joshua Morin von [Codenomicon](http://www.codenomicon.com/) für den Hinweis auf ein in MS08-063 beschriebenes Problem.
-   Alex Ionescu (<http://www.alex-ionescu.com/>) für den Hinweis auf ein in MS08-064 beschriebenes Problem.
-   Cody Pierce und Aaron Portnoy von [TippingPoint DVLabs](http://dvlabs.tippingpoint.com) für den Hinweis auf ein in MS08-065 beschriebenes Problem.
-   Fabien Le Mentec von [SkyRecon](http://www.skyrecon.com/) für den Hinweis auf ein in MS08-066 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (14. Oktober 2008): Bulletin Summary veröffentlicht.
-   V2.0 (15. Oktober 2008): Die Bewertung des Schweregrads für Windows Server 2008 für Itanium-basierte Systeme (MS08-062) wurde entfernt.
-   V2.1 (16. Oktober 2008): Aktualisierung der Kurzzusammenfassung für das Microsoft Security Bulletin MS08-062.
-   V3.0 (23. Oktober 2008): Microsoft Security Bulletin MS08-067, Sicherheitsanfälligkeit im Serverdienst kann Remotecodeausführung ermöglichen (958644) wurde hinzugefügt. Der Verweis auf den Bulletin Webcast für dieses außerplanmäßige Bulletin wurde ebenfalls hinzugefügt.

*Built at 2014-04-18T01:50:00Z-07:00*
