---
TOCTitle: 'Ändern des Kennworts für das RMS-Dienstkonto'
Title: 'Ändern des Kennworts für das RMS-Dienstkonto'
ms:assetid: '435c9cef-b622-48b3-9d4d-4bf5cac7d52d'
ms:contentKeyID: 18118818
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720273(v=WS.10)'
---

Ändern des Kennworts für das RMS-Dienstkonto
============================================

Je nach der für die RMS-Server angegebenen Kennwortrichtlinie kann das Kennwort für das RMS-Dienstkonto regelmäßig ablaufen. Wenn das Kennwort abläuft, ist RMS nicht mehr funktionsfähig. Daher müssen Sie das Kennwort vor dem Ablaufen ändern.

**Verwenden eines einzelnen RMS-Dienstkontos**

Wenn Sie ein einzelnes RMS-Dienstkonto verwenden, kann das Kennwort auf jedem RMS-Server folgendermaßen geändert werden:

1.  Befindet sich der Server in einem Cluster, schließen Sie ihn vom regelmäßigen Wechsel aus.
2.  Melden Sie sich mit den Anmeldeinformationen des RMS-Dienstkontos am Server an.
3.  Ändern Sie das Kennwort für das RMS-Dienstkonto.
    Bei den anderen Servern, die das gleiche RMS-Dienstkonto verwenden, tritt ein Dienstausfall auf, da die von diesen Servern gespeicherten Anmeldeinformationen nach dem Ändern des Kennworts ungültig sind.
4.  Melden Sie sich vom Server ab.
5.  Melden Sie sich mit den Administratoranmeldeinformationen von RMS am Server an.
6.  Zur erneuten Konfiguration der Benutzeridentität auf dem Server klicken Sie auf der Seite **Globale Verwaltung** auf **RMS-Dienstkonto ändern**, und geben Sie dann auf der Seite **RMS-Dienstkonto ändern** die Domäne, den Benutzernamen und das Kennwort an.
7.  Starten Sie IIS erneut.
8.  Beziehen Sie den Server ggf. wieder in den regelmäßigen Wechsel ein.
9.  Wiederholen Sie Schritt 6 bis 8 für alle anderen Server im Cluster.

Dies ist das einfachste Verfahren zum Ändern des Kennwortes für das RMS-Dienstkonto. Es kann jedoch vorkommen, dass RMS einige Zeit nicht verfügbar ist, da Active Directory mit dem neuen Kennwort aktualisiert wird, wenn Sie das Kennwort für das RMS-Dienstkonto auf einem Server ändern. IIS startet regelmäßig die Anwendungspools neu. Die unter den alten Anmeldeinformationen ausgeführten Anwendungspools können jedoch erst neu gestartet werden, wenn Sie das Kennwort des RMS-Dienstkontos ändern und IIS auf diesem Server neu starten. RMS ist erst wieder funktionsfähig, wenn die Anwendungspools wieder ausgeführt werden.

**Verwenden von zwei RMS-Dienstkonten**

Erstellen Sie mit dieser Methode zunächst zwei RMS-Dienstkonten, die unterschiedliche Ablaufrichtlinien oder -daten aufweisen. Bei Standardoperationen wird RMS unter dem ersten Konto ausgeführt. Wenn Sie das Kennwort für das Dienstkonto des ersten Kontos ändern möchten, führen Sie auf jedem RMS-Server die folgenden Schritte aus:

1.  Befindet sich der Server in einem Cluster, schließen Sie ihn vom regelmäßigen Wechsel aus.
2.  Geben Sie das zweite RMS-Dienstkonto als das Konto an, unter dem RMS ausgeführt werden soll. Anweisungen zum Ändern des Kontos finden Sie nachstehend unter „[Ändern des RMS-Dienstkontos](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)“.
3.  Starten Sie IIS erneut.
4.  Beziehen Sie den Server ggf. wieder in den regelmäßigen Wechsel ein.

Wenn alle RMS-Server das zweite RMS-Dienstkonto verwenden, können Sie das Kennwort des ersten RMS-Dienstkontos ändern, ohne dass die Ausführung des RMS-Systems davon beeinträchtigt wird. Sie können auf diese Weise zwischen den beiden Konten wechseln und somit Downtimes bei RMS vermeiden.