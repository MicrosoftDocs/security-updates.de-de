---
TOCTitle: 'Bewährte Methoden bei der RMS-Verwaltung'
Title: 'Bewährte Methoden bei der RMS-Verwaltung'
ms:assetid: '385f8112-da00-417f-a2b8-42dc1e06b717'
ms:contentKeyID: 18118808
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720245(v=WS.10)'
---

Bewährte Methoden bei der RMS-Verwaltung
========================================

Beachten Sie die folgenden bewährten Methoden für die Verwaltung von RMS.

-   **Stellen Sie keine zusätzlichen Dienste auf RMS-Servern bereit.**

    Wenn Sie außer den RMS-Diensten noch andere Dienste auf Ihren Servern ausführen, treten möglicherweise Konflikte auf, die zu Sicherheitsproblemen führen können. Überwachen Sie anhand von Leistungsindikatoren, ob die Leistung des Dienstes nachlässt oder ein Konflikt besteht.

-   **Führen Sie regelmäßige Sicherungen der Konfigurationsdatenbanken durch.**

    In den Konfigurationsdatenbanken werden Informationen gespeichert, die für die Funktionstüchtigkeit von RMS von essenzieller Bedeutung sind. In der Konfigurationsdatenbank des Stammzertifizierungsclusters sind außerdem die Schlüsselpaare für die gesamte Installation gespeichert. Wenn Sie regelmäßige Sicherungen durchführen, können Sie im Falle eines Datenbankserverversagens eine rasche Wiederherstellung von RMS gewährleisten. Neben den regelmäßigen Sicherungen sollten Sie auch regelmäßig die Gültigkeit dieser Sicherungen überprüfen, indem Sie in einer separaten Testumgebung Testwiederherstellungen durchführen. Weitere Informationen dazu finden Sie unter „Sichern und Wiederherstellen des RMS-Systems“ im Abschnitt „Planen einer RMS-Bereitstellung“ in dieser Dokumentationssammlung.
    
-   **Regulieren Sie regelmäßig die Größe der Protokollierungsdatenbank.**

-   **Verwenden Sie Microsoft Operations Manager (MOM) zur Überwachung des RMS-Servers.**

    Verwenden Sie MOM und RMS MOM Pack, um kritische Ereignisse zu erfassen oder Leistungsverschlechterungen zu entdecken und Benachrichtigungen von besagten Ereignissen zu versenden.