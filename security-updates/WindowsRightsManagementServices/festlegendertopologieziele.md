---
TOCTitle: Festlegen der Topologieziele
Title: Festlegen der Topologieziele
ms:assetid: '8275a04d-3e5b-40b0-be9d-2f31b7aeca6b'
ms:contentKeyID: 18118907
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747652(v=WS.10)'
---

Festlegen der Topologieziele
============================

Einer der wichtigsten Schritte im Topologieentwurf ist das Festlegen der jeweiligen Ziele. Einige der wichtigsten Bereiche, mit denen Sie sich beim Entwurf der RMS-Topologie befassen sollten, sind die folgenden:

-   **Verwaltungskosten**. Die Websitetopologie soll die Verwaltungskosten auf ein Minimum reduzieren. Dies bedingt nach Möglichkeit auch eine Zentralisierung der Serververwaltung und das Absenken der Serveranzahl auf das absolut erforderliche Minimum.
-   **Netzwerkwartezeiten**. Die Netzwerkwartezeiten zwischen Client und Server werden für Benutzer als zusätzliche Verzögerung beim Öffnen von E-Mail-Nachrichten oder Dokumenten bemerkbar sein. Im Allgemeinen sollte sichergestellt sein, dass die Wartezeiten in jede Richtung in 90 % der Fälle zwei Sekunden nicht überschreiten.
-   **Zuverlässigkeit**. Das Netzwerk zwischen Client und Server sollte zuverlässig genug sein, um zu gewährleisten, dass für HTTP-Anforderungen oder -Antworten eine Fehlerquote, d. h. fehlerhafte oder wegfallende Übertragungen, von unter 5 % eingehalten wird.

Dies sind nur allgemeine Richtlinien; die Ziele können je nach Anforderungen und Ressourcen der betreffenden Organisation variieren. Die Zielsetzungen sind Voraussetzung, um zu ermitteln, ob die Topologie die jeweiligen Ansprüche erfüllt. Viele Faktoren wirken sich auf die Erfüllung der Ziele aus. Dies schließt unter anderem Benutzer-, Lizenzanforderungs-, Abfragen- und Nachrichtenanzahl sowie sonstige RMS-bezogene Verkehrsfaktoren mit ein. Darüber hinaus kann das Vorgehen bei der Bereitstellung, insbesondere auch die Entscheidung, in welchen Domänen und Strukturen RMS bereitgestellt werden soll, einen großen Einfluss darauf haben, ob die Topologieziele erreicht werden können. Beim Entwurf der Topologie sollten diese Ziele nicht aus den Augen verloren werden, insbesondere auch in Bezug darauf, wie sich die einzelnen Schritte des Entwurfsvorgangs auf das Erreichen dieser Ziele auswirken.