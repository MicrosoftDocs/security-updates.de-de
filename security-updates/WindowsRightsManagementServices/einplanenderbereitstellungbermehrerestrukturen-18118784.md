---
TOCTitle: Einplanen der Bereitstellung über mehrere Strukturen
Title: Einplanen der Bereitstellung über mehrere Strukturen
ms:assetid: '2dfb40b7-95b1-4362-b32e-72867544b705'
ms:contentKeyID: 18118784
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720233(v=WS.10)'
---

Einplanen der Bereitstellung über mehrere Strukturen
====================================================

Wenn Sie RMS in einer Umgebung bereitstellen möchten, die mehrere Strukturen umfasst, müssen Sie zunächst ermitteln, welche Form der Unterstützung für die einzelnen Benutzer oder Gruppen erforderlich ist, die sich außerhalb der Struktur befinden, in der RMS bereitgestellt wird. Das Problem liegt in einem solchen Fall bei der Tatsache, dass für Benutzer- bzw. Gruppenobjekte aus anderen Strukturen normalerweise keine repräsentativen Entsprechungen in der Struktur vorliegen, die auch RMS umfasst. Wenn Sie beabsichtigen, mithilfe von RMS die Berechtigungen von Benutzern oder Gruppen aus anderen Strukturen einzuschränken, müssen Sie zunächst die RMS-Struktur so konfigurieren, dass Gruppenerweiterungen über die verschiedenen Strukturen hinweg möglich sind.

Es gibt zwei Möglichkeiten, um die Unterstützung von Gruppenerweiterungen bei RMS über mehrere Strukturen von hinweg umzusetzen:

-   Sie können RMS in der Struktur bereitstellen, in der Gruppen definiert werden. Hier kann RMS zum Erweitern der Gruppenmitgliedschaften eingesetzt werden.
-   Sie können auch Gruppendefinitionen zwischen Strukturen synchronisieren. Dies ermöglicht es der lokalen RMS-Installation, die vollständigen Gruppenmitgliedschaften aller Benutzer zu ermitteln. Wenn der Benutzer, der eine Lizenz anfordert, über ein Windows-Konto in einer anderen Struktur verfügt, muss auch in der lokalen Struktur ein Kontaktobjekt vorliegen, das die Gruppenzugehörigkeit dieses Benutzers repräsentiert. Mithilfe von Metaverzeichnissen wie Microsoft® Identity Integration Server (MIIS) 2003 oder dem Identity Integration Feature Pack (IIFP) können Sie eine vollständige Synchronisation von Gruppenobjekten über mehrere Strukturen erreichen.

Wenn Sie RMS nur für eine Struktur verwenden möchten, können Sie den Ausstellungsvorgang für Benutzerlizenzen optimieren, indem Sie in der RMS-Konfigurationsdatenbank die Clusterrichtlinie **MaxCrossForestCalls** anpassen. Diese Richtlinie gibt an, über wie viele Strukturgrenzen sich die Zugehörigkeit zu einer Gruppe maximal erstrecken kann. Der Standardwert ist 10. Wenn Sie diesen Wert beispielsweise in 0 ändern möchten, verwenden Sie dafür den folgenden SQL-Befehl:

`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'`
