---
TOCTitle: So importieren und verwenden Sie das RMS Management Pack
Title: So importieren und verwenden Sie das RMS Management Pack
ms:assetid: 'd9a73ef0-2f81-48c2-97cc-deb7bf477389'
ms:contentKeyID: 18119042
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747688(v=WS.10)'
---

So importieren und verwenden Sie das RMS Management Pack
========================================================

Importieren und Verwenden des RMS Management Pack
-------------------------------------------------

#### So importieren und verwenden Sie das RMS Management Pack

1.  Kopieren Sie das RMS Management Pack (RMS\_MOMPack.akm) aus dem Ordner %Programme%\\Windows Rights Management Services\\Tools auf den Server mit Microsoft Operations Manager (MOM).

2.  Öffnen Sie die MOM-Verwaltungskonsole, und importieren Sie das RMS Management Pack, indem Sie die folgenden Schritte ausführen:

    1.  Erweitern Sie in der Konsolenstruktur der MOM-Verwaltungskonsole das Element **Rules**, und klicken Sie dann mit der rechten Maustaste auf das Element **Processing Rule Group**.
    2.  Klicken Sie im Verknüpfungsmenü auf **Import Management Pack**. Das Dialogfeld **Import Management Pack** wird angezeigt.
    3.  Klicken Sie auf **Browse**, und wählen Sie dann die Datei RMS\_MOMPack.akm aus.

3.  Geben Sie die Zusammenführungs- oder Ersetzungsoptionen an. Weitere Optionen zum Zusammenführen und Ersetzen finden Sie unter „Exporting and Importing Management Packs“ auf der Microsoft-Website (http://www.microsoft.com/) (nur auf Englisch verfügbar).

    Klicken Sie auf **Replace**. Bei Verwendung der Ersetzungsoption überschreibt das importierte Management Pack die bestehenden Verarbeitungsregelgruppen. Es bleiben keine Benutzerkommentare erhalten. Wenn Sie dieses Management Pack und ein bestehendes Management Pack zusammenführen möchten, sollten Sie dies zunächst in einer Testumgebung ausführen. Verwenden Sie dann die Option **Replace**, wenn Sie das Management Pack in der Produktionsumgebung bereitstellen.

4.  Klicken Sie auf **Import**, um das Management Pack zu importieren.

5.  Klicken Sie in der **MOM-Verwaltungskonsole** auf das Element **Configuration**, und klicken Sie dann auf den Ordner **Agent Managers**.

6.  Klicken Sie mit der rechten Maustaste auf den Namen des Servers, auf dem Sie das RMS Management Pack importiert haben, und klicken Sie dann auf **Scan Managed Computers Now**.
