---
audience: end-user
title: Förhandsgranska leveransinnehåll
description: Lär dig hur du förhandsgranskar ditt leveransinnehåll med Campaign Web-gränssnittet
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Förhandsgranska meddelandeinnehållet {#preview-content}

Använd innehållssimuleringsfunktionen [!DNL Campaign] för att förhandsgranska innehållet i meddelandet innan du skickar det. På så sätt kan du styra personaliseringen och kontrollera hur den visas för mottagarna.

Följ stegen nedan om du vill förhandsgranska innehållet i leveransen.

1. Bläddra till skärmen Redigera innehåll för leveransen eller till [e-postmeddelandet för Designer](../email/get-started-email-designer.md).

1. Klicka på knappen **[!UICONTROL Simulate content]**.

   ![](assets/simulate-button.png){zoomable="yes"}

1. Välj de profiler som ska användas för att förhandsgranska innehållet. Det gör du genom att klicka på knappen **[!UICONTROL Add test profile(s)]** (för e-post och SMS) eller på knappen **[!UICONTROL Add subscriber(s)]** (för push-meddelanden).

1. Du kan kombinera profiler och testprofiler för att förhandsgranska ditt e-postmeddelande eller SMS.

   * Fliken **[!UICONTROL Test profiles]** visar alla testprofiler, som är ytterligare och fiktiva mottagare i databasen. [Lär dig arbeta med testprofiler](../audience/test-profiles.md)

   * På fliken **[!UICONTROL Profiles]** visas alla profiler som lagras i databasen. [Lär dig arbeta med profiler](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable="yes"}

1. När du bläddrar i testprofilen eller profillistorna kan du använda filter för att förfina sökningen. Du kan till exempel definiera en regel för att hitta alla testprofiler med statusen **[!UICONTROL Prospect]**. [Lär dig hur du lägger till regler med frågemodelleraren](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** för att bekräfta ditt val.

   En förhandsgranskning av leveransinnehållet visas i den högra rutan på skärmen **[!UICONTROL Simulate]**. Personaliserade element ersätts med data från den profil som valts i den vänstra rutan.

   ![](assets/simulate-preview.png){zoomable="yes"}

1. Om du har lagt till flera profiler kan du växla mellan dem i listan för att förhandsgranska motsvarande leveransinnehåll. Du kan också lägga till fler testprofiler och ta bort markeringen med motsvarande knappar i den vänstra rutan.

1. För e-postleveranser kan du justera **[!UICONTROL Zoom level]** och förhandsgranska ditt innehåll på en dator eller mobil enhet med hjälp av den dedikerade ikonen i det övre högra hörnet.

1. Från skärmen **[!UICONTROL Simulate]** kan du även:
   * Skicka korrektur till specifika mottagare för validering - [Läs mer](test-deliveries.md)
   * Få åtkomst till loggarna för skickade korrektur - [Läs mer](test-deliveries.md#access-test-deliveries)
   * Kontrollera innehållsåtergivningen i vanliga e-postklienter för endast e-post - [Läs mer](email-rendering.md)



