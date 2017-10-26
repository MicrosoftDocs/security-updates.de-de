---
TOCTitle: Ausschließen von Anwendungen
Title: Ausschließen von Anwendungen
ms:assetid: 'b68ae4b2-b9ba-44ae-90cb-c88df600ec86'
ms:contentKeyID: 18118979
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747644(v=WS.10)'
---

Ausschließen von Anwendungen
============================

Sie können die Version einer RMS-fähigen Anwendung (Rights Management Services oder Dienste für die Rechteverwaltung) angeben, mit der alle Lizenzierungsanforderungen verglichen werden. Der Anwendungsausschluss stempelt auf jede Nutzungslizenz eine Bedingung. Diese besagt, dass die Lizenz nur die RMS-geschützten Inhalte anbinden kann, für die sie ausgestellt wurde, sofern die Anwendung, die die Lizenz anfordert, nicht in der Ausschlussliste enthalten ist.

Dies ist z. B. dann hilfreich, wenn ein Unternehmen ein Sicherheitsupdate für eine Anwendung bereitstellt. Systemadministratoren können die üblichen Mechanismen zum Installieren des Updates auf Clientcomputern verwenden. Sie können Anwendungsausschlussrichtlinien festlegen, die mithilfe der Versionsinformationen der Anwendung definiert werden, welche die Verwaltungswebsite verwendet. Aufgrund dieser Ausschlussrichtlinie kann RMS keine Lizenzen für Clients ausstellen, die frühere Versionen der Software verwenden.

RMS-fähige Anwendungen werden mithilfe des Dateinamens und der Versionsnummer ausgeschlossen. Dies ist möglicherweise sinnvoll, wenn Sie sicherstellen möchten, dass Benutzer eine neuere, sicherere Version einer Anwendung installieren, sobald diese verfügbar ist. Sie verwenden z. B. Version 1.0.4.2315 einer RMS-fähigen Anwendung, die in Ihrer Organisation bereitgestellt wird. Der Anwendungsentwickler hat aber ein Sicherheitsproblem gefunden, das durch Ausstellen von Version 1.0.4.4200 behoben wird. Zusätzlich zur Einführung der neuen Anwendungsversion können Sie eine Ausschlussrichtlinie erstellen, die das Abrufen geschützter Inhalte durch Benutzer mithilfe der früheren Version verhindert.

Wie auch bei anderen Ausschlusstypen müssen Sie den Anwendungsausschluss auf jedem Cluster, für den er gelten soll, konfigurieren.

Wenn Sie diese Ausschlussrichtlinie auf dem Server anwenden, können Clients neue Nutzungslizenzen für RMS-geschützte Inhalte nicht mehr mit der ausgeschlossenen Anwendung anfordern und verbinden. Sie können die ausgeschlossene Anwendung aber weiterhin zum Abrufen von zuvor lizenzierten Dateien verwenden.

| ![](images/Cc747644.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                   |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS erfordert, dass die Anwendungsversion durch vier jeweils durch Punkte getrennte Ziffern (\#.\#.\#.\# ) angegeben wird. Bei manchen Anwendungen ist die Anwendungsversion allerdings in zwei bzw. drei durch Punkte getrennten Ziffern angegeben. Ist dies der Fall, sollte „.0“ angefügt werden, um die Versionsnummer an das für RMS erforderliche Format anzupassen. |