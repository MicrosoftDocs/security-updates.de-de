---
TOCTitle: Aktivieren des Außerbetriebsetzungsdienstes
Title: Aktivieren des Außerbetriebsetzungsdienstes
ms:assetid: '45226e85-b50d-41cc-aca7-0f603f8509d5'
ms:contentKeyID: 18118886
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720261(v=WS.10)'
---

Aktivieren des Außerbetriebsetzungsdienstes
===========================================

Zur Außerbetriebsetzung des RMS-Systems ist der private Schlüssel erforderlich, mit dem alle veröffentlichten Informationen geschützt sind. Dieser private Schlüssel ist in der Konfigurationsdatenbank gespeichert. Er ist durch die Datenschutz-API (DPAPI) verschlüsselt und beruht auf dem Kennwort, das bei der Bereitstellung eingegeben wurde. Wenn der private RMS-Schlüssel auf einem Hardwaresicherheitsmodul (HSM) gespeichert ist, ist er nicht gleichzeitig in der Konfigurationsdatenbank gespeichert.

| ![](images/Cc720261.Caution(WS.10).gif)Vorsicht                                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie das RMS-System außer Betrieb setzen, müssen Sie deshalb sicherstellen, dass Sie Ihr Kennwort für den privaten Schlüssel kennen. Wenn Sie das Kennwort nicht wissen, sollten Sie es zurücksetzen, bevor Sie den RMS-Server außer Betrieb setzen. |

Der erste Schritt zum Außerbetriebsetzen des RMS-Systems ist das Außerbetriebsetzen der Server im Cluster. Da es sich bei der Außerbetriebsetzung um eine Lizenzfunktion handelt, kann ein Server in einem unterregistriertem RMS-Lizenzierungscluster außer Betrieb gesetzt werden, ohne dass der RMS-Stammcluster oder andere unterregistrierten RMS-Lizenzierungscluster beeinträchtigt werden. Aus diesem Grund müssen Sie den RMS-Stammcluster und alle Lizenzierungscluster separat außer Betrieb setzen, da jeder Lizenzierungscluster über einen eigenen privaten Schlüssel zum Erstellen von Veröffentlichungslizenzen verfügt.

Aktivieren Sie den Außerbetriebsetzungsdienst wie folgt:

1.  Öffnen Sie die Windows RMS-Verwaltungswebsite.
2.  Klicken Sie auf **RMS verwalten**, und klicken Sie auf **Sicherheitseinstellungen**.
3.  Aktivieren Sie das Kontrollkästchen **Außerbetriebsetzung der RMS-Installation aktivieren**.
4.  Ein Dialogfeld wird geöffnet, in dem Sie aufgefordert werden, die Außerbetriebsetzung zu bestätigen. Klicken Sie hier auf **OK**.

Wenn Sie einen Server außer Betrieb setzen, kann dieser nicht mehr in einer RMS-Standardkonfiguration wiederhergestellt werden. Dieser Vorgang kann nicht rückgängig gemacht werden.

Nachdem RMS außer Betrieb gesetzt wurde, muss RMS in der Systemsteuerung über die Funktion **Software** vollständig entfernt werden, bevor Sie eine andere Instanz von RMS installieren können.
