---
TOCTitle: Vorlagen für Benutzerrechterichtlinien
Title: Vorlagen für Benutzerrechterichtlinien
ms:assetid: 'eee931c8-7c98-48e9-9e2c-d0b7bd4f2b96'
ms:contentKeyID: 18119079
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747732(v=WS.10)'
---

Vorlagen für Benutzerrechterichtlinien
======================================

Vorlagen für Benutzerrechterichtlinien beschreiben eine Standardgruppe von Benutzern, Rechten und Bedingungen, die auf RMS-geschützten Inhalt angewendet werden können. Wenn ein Benutzer eine Vorlage für Benutzerrechterichtlinien auf bestimmte Inhalte anwendet, werden die Rechte der Vorlage zu einem Teil der Veröffentlichungslizenz.

Auf der RMS-Verwaltungswebsite können Sie Vorlagen für Benutzerrechterichtlinien erstellen oder vorhandene Vorlagen ändern oder löschen. Vorlagen für Benutzerrechterichtlinien können verschiedene Bedingungen enthalten, wie z. B. bestimmte Empfänger oder Active Directory-Gruppen, eine begrenzte Gültigkeitsdauer der Nutzungslizenz für den Inhalt, eine begrenzte Abrufdauer für den Inhalt nach seiner Veröffentlichung und sogar benutzerdefinierte Werte, die nur für eine bestimmte RMS-fähige Anwendung relevant sind. Eine Vorlage kann eine Sperrliste erfordern. Sie gibt den URL (Uniform Resource Locator) zur Listendatei sowie die Anzahl von Tagen für die Gültigkeit der Liste an. Wenn ein Empfänger eine auf einer Vorlage basierende Nutzungslizenz anfordert, überprüft das System die Sperrliste, bevor der Benutzer den RMS-geschützten Inhalt abrufen kann. Weitere Informationen hierzu finden Sie unter „[RMS-Sperrung](https://technet.microsoft.com/72689f90-f3c5-4b61-94ea-d825f3199b3b)“ weiter unten in diesem Thema.

Im Folgenden werden einige Beispiele für Rechte, die in die Vorlage für Benutzerrechterichtlinien eingeschlossen werden könnten, aufgeführt:

-   Jeder kann die Inhalte anzeigen, doch nur der Autor kann sie ändern.
-   Jeder im Unternehmen kann die Inhalte anzeigen, doch nur während eines Monats nach der Veröffentlichung.
-   Jeder im Unternehmen kann die Inhalte anzeigen. Dies gilt nicht für externe Partner oder Kunden.
-   Nur angegebene Empfänger können die Inhalte anzeigen.
-   Nur ein angegebener Empfänger kann die Inhalte anzeigen oder ändern.

Vorlagen können verschiedene Bedingungen einschließen, z. B.:

-   Bestimmte Empfänger oder Active Directory-Gruppen, die über Rechte für die Inhalte verfügen.
-   Die Gültigkeitsdauer einer Nutzungslizenz für die Inhalte.
-   Die Abrufdauer der Inhalte nach deren Veröffentlichung.
-   Die Erfordernis einer Sperrliste und das Aktualisierungsintervall für die Liste.
-   Benutzerdefinierte Werte, die nur für eine bestimmte RMS-fähige Anwendung relevant sind.

Vorlagen für Benutzerrechterichtlinien werden sowohl in der Konfigurationsdatenbank als auch in einem freigegebenen Ordner gespeichert. Der RMS-Administrator ist für die Verteilung der Vorlagen für Benutzerrechterichtlinien aus dem freigegebenen Ordner an die Clientcomputer verantwortlich, damit sie von den Autoren verwendet werden können. Weitere Informationen hierzu finden Sie unter „Verteilen von Vorlagen für Benutzerrechterichtlinien“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.

In einer RMS-fähigen Anwendung können Autoren die Vorlage für Benutzerrechterichtlinien, die angewendet werden soll, auswählen. In der Vorlage ist normalerweise eine Gruppe angegeben, deren Mitglieder den Inhalt abrufen dürfen. Wenn ein Empfänger eine Nutzungslizenz anfordert, wendet der Server die Vorlage für Benutzerrechterichtlinien aus der Datenbank an. Damit wird sichergestellt, dass die Bestimmungen einer Nutzungslizenz immer die aktuellste Version der Vorlage wiedergeben.
