---
TOCTitle: 'RMS-Serverschlüssel'
Title: 'RMS-Serverschlüssel'
ms:assetid: '5f4100a1-9aa5-42af-85c8-4bc691022f06'
ms:contentKeyID: 18118862
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720280(v=WS.10)'
---

RMS-Serverschlüssel
===================

Ein RMS-Server verfügt über ein 1024-Bit-RSA-Schlüsselpaar (Rivest-Shamir-Adleman).

Der öffentliche Serverschlüssel dient zur Verschlüsselung des Inhaltsschlüssels, der sich in einer Veröffentlichungslizenz befindet, sodass nur der RMS-Server den Inhaltsschlüssel abrufen und Nutzungslizenzen für diese Veröffentlichungslizenz ausgeben kann. Das Server-Lizenzgeberzertifikat enthält den öffentlichen Serverschlüssel.

Der private Serverschlüssel wird zum Signieren aller vom Server ausgestellten Zertifikate und Lizenzen verwendet.

Schutz des privaten Serverschlüssels
------------------------------------

Standardmäßig wird der private Serverschlüssel während der Bereitstellung erstellt und in verschlüsselter Form in der RMS-Datenbank gespeichert. Alternativ können Sie während dieses Prozesses einen Kryptographiedienstanbieter (Cryptographic Service Provider oder CSP) angeben, der auf dem Server bereits installiert ist.

Sie können einen Kryptographiedienstanbieter auf zwei verschiedene Arten verwenden:

-   Wählen Sie zwischen Implementierungen des Kryptographiedienstanbieters aus, die vom Server standardmäßig installiert werden.
    – Oder –
-   Verwenden Sie die Software eines nicht von Microsoft stammenden Kryptographiedienstanbieters, die auf dem Server installiert ist.

> [!NOTE]
> Wenn Sie ein Hardwaresicherheitsmodul verwenden möchten, wählen Sie unbedingt einen Kryptographiedienstanbieter aus, der Hardwaresicherheitsmodule unterstützt. 

Wenn Sie sich dafür entscheiden, den privaten Serverschlüssel durch Verwendung eines Kryptographiedienstanbieters zu schützen, speichert RMS den Namen des Anbieters und den Namen des Schlüsselcontainers in der Konfigurationsdatenbank.