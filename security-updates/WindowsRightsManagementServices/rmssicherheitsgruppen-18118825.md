---
TOCTitle: 'RMS-Sicherheitsgruppen'
Title: 'RMS-Sicherheitsgruppen'
ms:assetid: '25749a83-8c12-48ec-96ad-296d31fd55d4'
ms:contentKeyID: 18118825
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720215(v=WS.10)'
---

RMS-Sicherheitsgruppen
======================

Bei der Einrichtung von RMS werden zwei Gruppen erzeugt: die RMS-Dienstgruppe (= RMS Service Group) und die Administratorengruppe (= Super Users Group).

Die RMS-Dienstgruppe ist eine lokale Sicherheitsgruppe, die über ausreichend Berechtigungen verfügt, um auf alle Ressourcen zugreifen zu können, die für den RMS-Betrieb erforderlich sind. Während der Installation legt der Administrator ein Benutzerkonto fest, das als RMS-Dienstkonto fungiert. Dieses Benutzerkonto wird der RMS Service Group automatisch als Mitglied hinzugefügt. Dadurch erhält es die entsprechenden Berechtigungen. Bei Normalbetrieb wird RMS zumeist unter diesem Benutzerkonto ausgeführt.

Eine weitere wichtige Gruppe ist die Administratorengruppe. Diese Gruppe hat vollständige Kontrolle über alle Inhalte, was bedeutet, dass ein Mitglied dieser Gruppe alle RMS-geschützten Inhaltsdateien verschlüsseln kann, sowie den vollständigen RMS-Schutz für sie widerrufen kann. Die Administratorengruppe hat standardmäßig keine Mitglieder, und auch RMS-Administratoren werden nicht automatisch in sie aufgenommen. Das Verwalten der Zugehörigkeit zu dieser Gruppe ist essenziell für die Sicherheit RMS-geschützter Inhalte. Weiter Informationen finden Sie in dieser Dokumentationssammlung unter „Betreiben eines RMS-Servers“ im Abschnitt „Nutzen der Administratorengruppe“.
