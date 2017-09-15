---
TOCTitle: So aktivieren Sie die Remoteverwaltung von RMS
Title: So aktivieren Sie die Remoteverwaltung von RMS
ms:assetid: '00f17054-5f5d-47e2-89c1-7a593b930bb3'
ms:contentKeyID: 18118738
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720181(v=WS.10)'
---

So aktivieren Sie die Remoteverwaltung von RMS
==============================================

Auf dem Computer, der für die Remoteverwaltung von RMS verwendet wird, muss Internet Explorer 6.0 oder höher installiert sein.

Aktivieren der Remoteverwaltung von RMS
---------------------------------------

#### So aktivieren Sie die Remoteverwaltung von RMS

1.  Melden Sie sich an dem Server an, für den Sie eine Remoteverwaltung durchführen möchten.

2.  Öffnen Sie unter **Verwaltung** das Snap-In für den **Internetinformationsdienste-Manager (IIS-Manager)**.

3.  Erweitern Sie das Objekt, das die Website repräsentiert, auf der Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) bereitgestellt haben.

4.  Klicken Sie mit der rechten Maustaste auf den Ordner **\_wmcs**, und klicken Sie auf **Eigenschaften**. Klicken Sie auf der Registerkarte **Verzeichnissicherheit** unter **Sichere Kommunikation** auf **Bearbeiten**, klicken Sie auf **Sicheren Kanal verlangen (SSL)**, und klicken Sie dann auf **OK**. Dadurch wird SSL-Schutz (Secure Sockets Layer) für die RMS-Webdienste zugewiesen. Weitere Informationen zum Verwalten von Websites mithilfe von IIS finden Sie in der Hilfe zu IIS.

    | ![](images/Cc720181.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                                 |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Sie können RMS-Webdienste mit SSL (Secure Sockets Layer) verwenden, um zusätzliche Sicherheit zu erzielen und HTTP-Remotezugriff auf die RMS-Verwaltungswebseiten zu ermöglichen. Wenn Sie SSL für die RMS-Webdienste aktivieren möchten, beziehen und installieren Sie ein gültiges SSL-Webserverzertifikat. |

5.  Klicken Sie mit der rechten Maustaste auf den Ordner **Admin**, und klicken Sie dann auf **Eigenschaften**. Klicken Sie auf der Registerkarte **Verzeichnissicherheit** unter **Beschränkungen für IP-Adressen und Domänennamen** auf **Bearbeiten**, und klicken Sie dann unter **Zugriffsbeschränkungen für IP-Adressen** auf **Zugriff gewährt**, um allen Computern das Anfordern einer Verbindung mit dieser Website zu ermöglichen.
