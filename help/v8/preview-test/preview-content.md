---
audience: end-user
title: Förhandsgranska leveransinnehåll
description: Lär dig hur du förhandsgranskar ditt leveransinnehåll med Campaign Web UI
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Begränsad tillgänglighet"
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 2%

---


# Förhandsgranska meddelandeinnehållet {#preview-content}

Använd [!DNL Campaign] innehållssimulering för att förhandsgranska innehållet i meddelandet innan det skickas. På så sätt kan du styra personaliseringen och kontrollera hur den visas för mottagarna.

Följ stegen nedan om du vill förhandsgranska innehållet i leveransen.

1. Bläddra till skärmen Redigera innehåll för leveransen eller till [E-postdesigner](../email/get-started-email-designer.md).

1. Klicka på knappen **[!UICONTROL Simulate content]**.

   ![](assets/simulate-button.png)

1. Om du vill välja de profiler som ska användas för att förhandsgranska ditt personaliserade innehåll använder du:

   * **[!UICONTROL Add test profile(s)]** för förhandsgranskning av e-post- och SMS-leveranser

   * **[!UICONTROL Add subscriber(s)]** för förhandsgranskning av push-meddelanden

1. Du kan kombinera testprofiler och profiler för att förhandsgranska ditt e-postmeddelande eller SMS.

   * The **[!UICONTROL Test profiles]** På -fliken visas alla dirigerade adresser, som är ytterligare och fiktiva mottagare i databasen.

     ![](assets/simulate-select-profiles.png)

     >[!NOTE]
     >
     >Testprofiler kan skapas från **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** -menyn. [Läs mer](../audience/test-profiles.md#create-test-profiles)

   * The **[!UICONTROL Profiles]** På -fliken visas alla mottagare som är lagrade i **[!UICONTROL Profiles and Targets]** mapp från [!DNL Campaign] konsol. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}.

     >[!NOTE]
     >
     >Du kan också visa och hantera profiler från motsvarande flik i webbgränssnittet för Campaign. [Läs mer](../audience/about-recipients.md)

1. Klicka **[!UICONTROL Select]** för att bekräfta ditt val.

   En förhandsgranskning av leveransinnehållet visas i den högra rutan i dialogrutan **[!UICONTROL Simulate]** skärm. Personaliserade element ersätts med data från den profil som valts i den vänstra rutan.

   ![](assets/simulate-preview.png)

1. Om du har lagt till flera profiler kan du växla mellan dem i listan för att förhandsgranska motsvarande leveransinnehåll. Du kan också lägga till fler testprofiler och ta bort markeringen med motsvarande knappar i den vänstra rutan.

1. För e-postleveranser kan du justera **[!UICONTROL Zoom level]** och förhandsgranska innehållet på datorn eller en mobil enhet med den dedikerade ikonen i det övre högra hörnet.

1. Från **[!UICONTROL Simulate]** kan du också:
   * Skicka testleveranser till specifika mottagare för validering - [Läs mer](test-deliveries.md)
   * Få åtkomst till loggarna för skickade testleveranser - [Läs mer](test-deliveries.md#access-test-deliveries)
   * Kontrollera innehållsåtergivningen i vanliga e-postklienter endast för e-post - [Läs mer](email-rendering.md)



