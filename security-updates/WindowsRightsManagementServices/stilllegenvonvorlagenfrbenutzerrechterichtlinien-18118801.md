---
TOCTitle: Stilllegen von Vorlagen für Benutzerrechterichtlinien
Title: Stilllegen von Vorlagen für Benutzerrechterichtlinien
ms:assetid: '32bf98c7-edda-4507-a4b8-4c11bddd6e60'
ms:contentKeyID: 18118801
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720239(v=WS.10)'
---

Stilllegen von Vorlagen für Benutzerrechterichtlinien
=====================================================

Wenn Sie eine Vorlage für Benutzerrechterichtlinien stilllegen möchten, müssen Sie diese löschen. Diese Vorgehensweise wird nachstehend unter „[So löschen Sie eine Vorlage für Benutzerrechterichtlinien](https://technet.microsoft.com/9c9a1496-cf55-4c65-a4c6-9fe245edce00)“beschrieben. Im Allgemeinen sollten Sie aber keine Vorlagen für Benutzerrechterichtlinien löschen. Wenn Sie eine Vorlage für Benutzerrechterichtlinien stilllegen möchten, müssen Sie unbedingt auch Kopien dieser Vorlage auf den Benutzercomputern entfernen. Dies ist wichtig, da eine Anforderung beim RMS-Server eingeht, wenn ein Autor Inhalte mithilfe einer Vorlage für Benutzerrechterichtlinien veröffentlicht. RMS verwendet eine Kopie der in der Datenbank gespeicherten Vorlage, um auf die Anforderung zu antworten. Wenn die Vorlage für Benutzerrechterichtlinien nicht vorhanden ist, schlägt die Anforderung fehl.

| ![](images/Cc720239.note(WS.10).gif)Hinweis                                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Eine Möglichkeit, das Stilllegen einer Vorlage für Benutzerrechterichtlinien zu verwalten, ist das Erstellen eines Skripts, das die Vorlage von allen Benutzercomputern entfernt. |
