---
TOCTitle: Verwalten der Protokollgröße
Title: Verwalten der Protokollgröße
ms:assetid: '431b32b3-02f0-4666-b52c-183eb65154fd'
ms:contentKeyID: 18118814
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720271(v=WS.10)'
---

Verwalten der Protokollgröße
============================

Der Protokollierungsdienst sendet große Datenmengen an die SQL Server-Datenbank. Sie sollten die Protokollierungsdatenbank regelmäßig überprüfen, um sicherzustellen, dass die Festplattenkapazität für die Daten ausreicht. Wenn Sie der Meinung sind, dass eine übermäßig große Datenmenge vorhanden ist und einige Informationen für die Berichterstellung überflüssig sind, sollten Sie SQL Server-Filter festlegen. Dadurch werden die Protokolldateien verringert und nur die benötigten Protokolle gespeichert. Anleitungen zum Filtern von Protokollierungsinformationen finden Sie in der Hilfe zu SQL Server Enterprise Manager.

Wenn Sie feststellen, dass die Protokollierungsdatenbank für den verfügbaren Speicherplatz zu groß wird, können Sie sie auf einen anderen Server verschieben, wie nachstehend unter „[Verschieben der Protokollierungsdatenbank](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)“ beschrieben.

> [!IMPORTANT]
> Sie sollten außerdem die Größe der ausgehenden Warteschlange für Protokollierungsnachrichten regelmäßig mithilfe von Systemmonitor überwachen. Wenn die Größe der Warteschlange erheblich anwächst, überprüfen Sie, ob der Protokollierungslistenerdienst einwandfrei ausgeführt wird. Weitere Informationen zum Verwenden von Systemmonitor finden Sie im Windows Server 2003-Hilfe- und Supportcenter. 