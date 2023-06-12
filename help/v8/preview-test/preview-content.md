---
audience: end-user
title: Förhandsgranska e-postinnehåll
description: Lär dig hur du förhandsgranskar ditt e-postinnehåll med webbgränssnittet för Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha" type="Positive"
source-git-commit: 6671d4c18da5655d67b9fd30c05fd2e9052d000b
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 1%

---


# Förhandsgranska e-postinnehåll {#preview-content}

Använd [!DNL Campaign] funktioner för simulering av innehåll för att förhandsgranska innehållet i ditt e-postmeddelande innan det skickas. På så sätt kan du styra personaliseringen och kontrollera hur den visas för mottagarna.

Om du vill förhandsgranska innehållet i ditt e-postmeddelande följer du stegen nedan.

1. Bläddra till e-postmeddelandet [Redigera innehåll](../content/edit-content.md) eller till [E-postdesigner](../content/get-started-email-designer.md).

1. Klicka på knappen **[!UICONTROL Simulate content]**.

   ![](assets/simulate-button.png)

1. Använd **[!UICONTROL Add test profile(s)]** för att välja de profiler som ska användas för att förhandsgranska ditt personaliserade innehåll.

1. Du kan kombinera testprofiler och profiler för att förhandsgranska e-postmeddelandet.

   * The **[!UICONTROL Test profiles]** På -fliken visas alla dirigerade adresser, som är ytterligare och fiktiva mottagare i databasen.

     >[!NOTE]
     >
     >Testprofiler kan skapas i [!DNL Campaign] konsolen i **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** mapp. Läs mer i [Kampanjdokumentation v8 (konsol)](https://experienceleague.corp.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * The **[!UICONTROL Profiles]** På -fliken visas alla mottagare som lagras i **[!UICONTROL Profiles and Targets]** mapp från [!DNL Campaign] konsol. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

   ![](assets/simulate-select-profiles.png)

1. Klicka **[!UICONTROL Select]** för att bekräfta ditt val på båda flikarna.

   En förhandsgranskning av e-postmeddelandet visas i den högra rutan i dialogrutan **[!UICONTROL Simulate]** skärm. Personaliserade element ersätts med data från den profil som valts i den vänstra rutan.

   ![](assets/simulate-preview.png)

1. Om du har lagt till flera profiler kan du växla mellan dem i listan för att förhandsgranska motsvarande e-postinnehåll. Du kan också lägga till fler testprofiler och ta bort markeringen med motsvarande knappar i den vänstra rutan.

1. Du kan justera **[!UICONTROL Zoom level]** och förhandsgranska innehållet på datorn eller en mobil enhet med den dedikerade ikonen i det övre högra hörnet.

1. Från **[!UICONTROL Simulate]** kan du också:
   * Kontrollera e-poståtergivningen i vanliga e-postklienter - [Läs mer](email-rendering.md)
   * Skicka testmeddelanden till specifika mottagare för validering - [Läs mer](proofs.md)



