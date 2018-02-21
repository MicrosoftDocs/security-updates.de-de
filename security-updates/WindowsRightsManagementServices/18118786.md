---
TOCTitle: Rechtekontozertifikate
Title: Rechtekontozertifikate
ms:assetid: '2ff315cc-211d-4e6e-85e8-56867c2abd94'
ms:contentKeyID: 18118786
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720230(v=WS.10)'
---

Rechtekontozertifikate
======================

Organisationen müssen die Benutzer identifizieren, die innerhalb des RMS-Systems als vertrauenswürdige Entitäten gelten sollen. Zu diesem Zweck stellt RMS Rechtekontozertifikate aus, die Benutzerkonten mit spezifischen Computern verknüpfen. Die Rechtekontozertifikate der Benutzer müssen in Anforderungen von Client-Lizenzgeberzertifikaten und -Nutzungslizenzen enthalten sein. Ein Client-Lizenzgeberzertifikat ermöglicht es einem Autor, RMS-geschützte Inhalte wie Dateien und E-Mail-Nachrichten auch offline zu veröffentlichen. Eine Nutzungslizenz ermöglicht es einem Benutzer, RMS-geschützte Inhalte einzusehen. Jedes Rechtekontozertifikat enthält den öffentlichen Schlüssel des Benutzers, mit dem Daten verschlüsselt werden, die für diesen Benutzer bestimmt sind.

Es gibt zwei Arten von Rechtekontozertifikaten: Standardzertifikate und temporäre Zertifikate. Sie können die Gültigkeitsdauer für beide Typen angeben. Die Dauer für Standardzertifikate wird in Tagen angegeben (standardmäßig 365 Tage). Die Dauer für temporäre Kontozertifikate wird in Minuten angegeben (standardmäßig 15 Minuten). Temporäre Kontozertifikate ermöglichen Benutzern das temporäre Abrufen von Inhalten, z. B. an einem Kiosk, wenn sie auf den von ihnen normalerweise verwendeten Computer nicht zugreifen können. Damit wird verhindert, dass ein anderer Benutzer die Inhalte von diesem Computer aus zu einem späteren Zeitpunkt abruft.