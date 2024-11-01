---
audience: end-user
title: Transaktionsmeddelanden
description: Transactional messaging with Adobe Campaign Web
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Om transaktionsmeddelanden {#transactional-messaging}

>[!CONTEXTUALHELP]
>id="acw_transacmessages"
>title="Transaktionsmeddelanden"
>abstract="Transactional messaging är en specialiserad modul i Adobe Campaign som hanterar utlösta meddelanden."

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Transaktionsmeddelanden"
>abstract="Transactional messaging är en specialiserad modul i Adobe Campaign som hanterar utlösta meddelanden. Dessa meddelanden genereras automatiskt som svar på händelser som kommer från informationssystem."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Se versionsinformation"

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
