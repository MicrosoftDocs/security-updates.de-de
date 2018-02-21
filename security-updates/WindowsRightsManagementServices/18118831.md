---
TOCTitle: 'Funktionsweise der RMS-Sperrung'
Title: 'Funktionsweise der RMS-Sperrung'
ms:assetid: '469e3938-a59b-4c92-9779-ead64e724d00'
ms:contentKeyID: 18118831
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720263(v=WS.10)'
---

Funktionsweise der RMS-Sperrung
===============================

Bei einer Sperrung wird die Bindung (der Prozess, der einem Benutzer das Abrufen von Inhalten ermöglicht) verhindert, wenn eine gesperrte Entität in die Bindungsanforderung einbezogen wird. Die Sperrung wird über Sperrlisten implementiert, die an Clientcomputer verteilt werden. Bei diesen Listen handelt es sich um signierte XrML-Dateien (eXtensible rights Markup Language). Sie geben die Inhalte, Anwendungen, Benutzer oder anderen Prinzipale an, die durch den Prinzipal, der die Liste ausstellt, gesperrt wurden.

Jedes Mal, wenn ein Benutzer versucht, geschützten Inhalt abzurufen, sendet die damit verknüpfte RMS-fähige Anwendung eine Anforderung für das erforderliche Recht als Bindungsanforderung an den RMS-Client. Wenn der Benutzer beispielsweise eine Datei zu öffnen versucht, fordert die Anwendung das Recht Anzeigen an, damit die Datei geöffnet werden kann. Wenn der Benutzer die Datei zu bearbeiten versucht, fordert die Anwendung das Recht Bearbeiten an.

Während die Bindungsanforderung verarbeitet wird, führt der RMS-Client folgende Schritte aus:

1.  Sie wertet die Nutzungslizenz für alle Sperrlistenanforderungen aus.
2.  Wenn die Nutzungslizenz eine Sperrung erfordert, überprüft die Clientkomponente, ob die angegebene Sperrliste vorhanden, registriert und entsprechend dem in der Nutzungslizenz angegebenen Aktualisierungsintervall aktuell ist.
3.  Die Clientkomponente überprüft, ob der die Sperrliste signierende Prinzipal in der Nutzungslizenz als ein Prinzipal angegeben ist, der die Lizenz sperren darf.
4.  Nach dem erfolgreichen Abschluss dieser Prüfungen ermittelt die Clientkomponente, ob Prinzipale gesperrt wurden, die in die ursprüngliche Bindungsanforderung einbezogen sind. Falls dies zutrifft, lehnt sie die Bindungsanforderung ab.

Sperrlisten können vom Administrator an Clientcomputer verteilt werden, oder sie können von einer RMS-fähigen Anwendung auf den Computer gedownloadet werden, falls dies für eine Nutzungslizenz erforderlich ist. Beim Verwenden einer Sperrliste zum Binden bestimmter Inhalte, wird die Sperrliste registriert und kann für Bindungsanforderungen bei anderen Nutzungslizenzen verwendet werden, solange die Anwendung geöffnet bleibt. Nach dem Schließen der Anwendung wird die Registrierung der Sperrliste aufgehoben.

Im folgenden Schema wird der Bindungsprozess und die Funktionsweise der Sperrung dabei angezeigt.

![](images/Cc720263.81aa2d70-d261-49ad-b446-96a2eddba1a5(WS.10).gif)

Die Sperrung ist optional. Der RMS-Administrator kann eine Sperrung erforderlich machen, indem er sie in mindestens einer Vorlage für Benutzerrechterichtlinien der Organisation festlegt. Wenn eine Sperrung erforderlich ist, kann eine Lizenz nur dann eine Bindung vornehmen, wenn die erforderliche Sperrliste vorhanden, auf dem Computer des Benutzers registriert und nicht älter als das in der Nutzungslizenz angegebene Aktualisierungsintervall ist.

Es muss jedoch darauf hingewiesen werden, dass die Sperrung für eine bestimmte Nutzungslizenz sogar dann weiterhin wirksam werden kann, wenn die Nutzungslizenz dies nicht erfordert. Die Sperrung wird immer dann wirksam, wenn ein Aussteller eines in der Vertrauenskette befindlichen und in der Bindungsanforderung einbezogenen Zertifikats, eine auf einem Clientcomputer registrierte Sperrliste ausgestellt hat. In diesem Szenario wird die Sperrliste zum Verarbeiten von Bindungsanforderungen verwendet, selbst wenn die einbezogenen Nutzungslizenzen keine Sperrung erfordern. Dies gilt so lange, bis die RMS-fähige Anwendung geschlossen wird, denn dadurch wird die Registrierung der Sperrliste aufgehoben.

Wenn ein Benutzer beispielsweise versucht, Inhalt abzurufen, dessen von Entität A ausgegebene Nutzungslizenz eine ebenfalls von Entität A ausgegebene Sperrliste erfordert, ruft die RMS-fähige Anwendung die Sperrliste von dem in der Nutzungslizenz angegebenen URL ab und registriert sie anschließend. Während der Verarbeitung der Bindungsanforderung prüft der RMS-Client, ob die Sperrliste eventuell Sperrungen enthält.

Anschließend lässt der Benutzer die RMS-fähige Anwendung geöffnet und versucht, einen zweiten Inhalt abzurufen, dessen Nutzungslizenz ebenfalls von Entität A ausgegeben wurde. Obwohl diese Nutzungslizenz keine Sperrbedingungen enthält, ist die Sperrliste von Entität A aktuell auf dem Computer des Benutzers registriert. In dieser Situation untersucht die Clientkomponente die Sperrliste, bevor die Bindungsanforderung verarbeitet wird.

Anschließend versucht der Benutzer, bestimmte Inhalte abzurufen, deren Nutzungslizenz von Entität C ausgestellt wurden. Die Nutzungslizenz schließt keine Sperrbedingung ein. Weil die einzige auf dem Clientcomputer registrierte Sperrliste die von Entität A ausgestellte Liste ist und Entität A sich nicht in der Vertrauenskette für die Nutzungslizenz befindet, ist keine Sperrung für die Bindung wirksam.

Abschließend schließt der Benutzer die RMS-fähige Anwendung und öffnet später erneut den zweiten Inhalt, der keine Sperrbedingung enthielt. Da die Registrierung der von Entität A ausgegebenen Sperrliste durch das Schließen der Anwendung aufgehoben wurde, wird die Liste vor der Verarbeitung der Bindungsanforderung nicht vom RMS-Client überprüft.