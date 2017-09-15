---
TOCTitle: Überwachen mithilfe von Microsoft Operations Manager
Title: Überwachen mithilfe von Microsoft Operations Manager
ms:assetid: 'ce372598-7421-4f1f-b8eb-f62da26e85d1'
ms:contentKeyID: 18119015
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747758(v=WS.10)'
---

Überwachen mithilfe von Microsoft Operations Manager
====================================================

RMS enthält ein Management Pack, das zusammen mit Microsoft® Operations Manager (MOM) verwendet werden kann. Mithilfe von MOM können Sie die Servervorgänge in Ihrer Organisation folgendermaßen verwalten:

-   Überwachen von Ereignissen, die von RMS im Ereignisprotokoll der Anwendung aufgezeichnet werden.
-   Hervorheben von Ereignissen, die auf mögliche Dienstausfälle oder Konfigurationsprobleme hinweisen. Auf diese Weise können Sie korrigierende oder vorbeugende Maßnahmen schnell ergreifen.
-   Anzeigen von Warnmeldungen und Fehlern, wie z. B. dem Ablauf des Server-Lizenzgeberzertifikats oder dem Ausfall eines Webdienstes.

Das RMS Management Pack (RMS\_MOMPack.akm) wird zusammen mit RMS im Ordner %Programme%\\Windows Rights Management Services\\Tools installiert.

Dieses Management Pack enthält die folgenden Gruppen von Regeln, die der RMS-Administrator zur Verwaltung der RMS-Serverbereitstellung verwenden kann.

**RMS MOM Management Pack-Regeln**

1.  PMC Measure - Activation Proxy Total Failures
2.  PMC Measure - Activation Proxy Total Time
3.  PMC Measure - Activation Total Processing Time
4.  PMC Measure - Activation Total Reqs
5.  PMC Measure - ActivationProxy Total Reqs
6.  PMC Measure - AD Cache (DB Cache) Hits
7.  PMC Measure - AD Cache (DB Cache) Misses
8.  PMC Measure - Average License Processing Time
9.  Event - Configuration Info Corruption
10. PMC Measure - Dead GC Connections
11. PMC Measure - Enroll Failures
12. Event - General Error
13. Event - Init Failure
14. Event - Licensor Cert has expired
15. Event - Licensor Cert Request Failure
16. Event - Logging Service Failure
17. PMC Measure - Max GC connections available
18. Event - Missing License Acq Point Generation Plugin
19. PMC Measure - MSMQ Queue length on all RM servers
20. Event - No GCs available
21. Event - Plugin Init Failure
22. Event - PrivateKey protection password changed
23. Event - RM Server Shut Down
24. Event - RM Server ShutDown Failure
25. Event - Server Startup Failure
26. PMC Measure - SubEnroll Failures
27. Event - SuperUser privileged override power was invoked
28. PMC Threshold - Too Many GetLicensorCert Failures
29. Event - Upcoming Licensor Cert Expiry - 1 Month
30. Event - Upcoming Licensor Cert expiry - 1 Week

Weitere Informationen zum Bereitstellen von MOM Management Packs in einem Unternehmen finden Sie auf der [Microsoft-Website](http://www.microsoft.com/)(http://www.microsoft.com/).
