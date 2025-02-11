---
audience: end-user
title: Transaktionsmeddelanden
description: Transactional messaging with Adobe Campaign Web
exl-id: 90830dca-acff-4aa3-a88b-1005e349cf52
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Om transaktionsmeddelanden {#transactional-messaging}

>[!CONTEXTUALHELP]
>id="acw_transacmessages"
>title="Transaktionsmeddelanden"
>abstract="Transactional messaging är en specialiserad modul i Adobe Campaign som hanterar utlösta meddelanden."

<!-- >>[!CONTEXTUALHELP]
>id="acw_transacmessages_exclusionlogs"
>title="Transactional messaging exclusion logs"
>abstract="Transactional messaging exclusion logs" -->

Transactional messaging är en specialiserad modul i Adobe Campaign som hanterar utlösta meddelanden. Dessa meddelanden genereras automatiskt som svar på händelser som kommer från informationssystem. Vanliga exempel på sådana händelser är att klicka på knappar eller länkar, överge varukorgar, begära varningar om produkttillgänglighet, skapa eller ändra konto osv.

Transaktionsmeddelanden används för att skicka:

* Viktiga meddelanden, som orderbekräftelser eller lösenordsåterställningar,
* Realtidssvar på kundåtgärder (t.ex. skapande av konto, slutförande av köp),
* Icke-marknadsföringsmaterial som är viktigt för kundinteraktioner.

Transactional Messaging-modulen integreras smidigt med era informationssystem. Evenemangen, till exempel kundåtgärder, skickas till Adobe Campaign som skickar motsvarande personaliserade meddelande. Dessa meddelanden kan skickas individuellt eller gruppvis via olika kanaler som e-post, SMS eller push-meddelanden.

Du hittar modulen **[!UICONTROL Transactional message]** i avsnittet **[!UICONTROL Triggered messages]**.

![](assets/transactional.png){zoomable="yes"}

Du har tre flikar på sidan **[!UICONTROL Transactional message]**:

* **[!UICONTROL Browse]** där du har en lista över transaktionsmeddelanden med status,
* **[!UICONTROL Templates]** där du hittar och skapar mallar för transaktionsmeddelanden,
* **[!UICONTROL History]** där du har information om alla transaktionsmeddelanden som har körts.

Läs mer i den här dokumentationen om hur du:

* [Skapa transaktionsmeddelanden](create-transactional.md) med hjälp av en mall och lär dig de inställningar som behövs,
* [Verifiera innehållet i dina transaktionsmeddelanden](validate-transactional.md) och simulera en personalisering,
* [Övervaka dina transaktionsmeddelanden](monitor-transactional.md).
