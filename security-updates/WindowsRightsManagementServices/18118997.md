---
TOCTitle: Vertrauenswürdige Veröffentlichungsdomänen
Title: Vertrauenswürdige Veröffentlichungsdomänen
ms:assetid: 'bca1c33a-d3ef-42b5-adbe-6e104979a71f'
ms:contentKeyID: 18118997
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747738(v=WS.10)'
---

Vertrauenswürdige Veröffentlichungsdomänen
==========================================

Standardmäßig stellen RMS-Server keine Nutzungslizenzen für Veröffentlichungslizenzen aus, die von einem RMS-Server in einem anderen Cluster ausgestellt wurden. Es gibt jedoch Situationen, in denen derselbe Server oder Cluster keine Veröffentlichungs- und Nutzungslizenzen zusammen für bestimmte geschützte Inhalte ausstellen kann. Dies ist beispielsweise der Fall, wenn ein bestimmter RMS-Cluster stillgelegt wird und ein anderer seine Stelle einnimmt, z. B. wenn zwei Unternehmen fusionieren. In dieser Situation muss ein RMS-Cluster die Möglichkeit haben, Nutzungslizenzen für Veröffentlichungslizenzen auszustellen, die von einem anderen RMS-Cluster erstellt wurden.

Sie können einen RMS-Cluster so konfigurieren, dass er den Veröffentlichungslizenzen, die von einem anderen RMS-Cluster ausgestellt wurden, vertraut und Nutzungslizenzen dafür ausstellt, indem Sie eine vertrauenswürdige Veröffentlichungsdomäne implementieren. Zu diesem Zweck importieren Sie das Server-Lizenzgeberzertifikat und den privaten Schlüssel von dem anderen Server und fügen ihn zur Liste der vertrauenswürdigen Veröffentlichungsdomänen hinzu. Die importierten privaten Schlüssel werden nur zum Entschlüsseln signierter Veröffentlichungslizenzen und nicht zum Signieren neuer Lizenzen verwendet.

Weitere Informationen zu vertrauenswürdigen Benutzerdomänen sowie schrittweise Anleitungen finden Sie unter „Hinzufügen und Entfernen von vertrauenswürdigen Veröffentlichungsdomänen“ und „Einrichten von Vertrauensrichtlinien“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.