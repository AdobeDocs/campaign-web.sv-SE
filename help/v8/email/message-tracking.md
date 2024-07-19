---
audience: end-user
title: Spåra meddelanden
description: Lär dig hur du lägger till länkar och spårar skickade meddelanden
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 2%

---

# Lägga till länkar och spåra meddelanden {#tracking}

Använd e-postdesignern för att lägga till länkar till ditt innehåll och spåra meddelanden som skickas för att övervaka mottagarnas beteende.

## Infoga länkar {#insert-links}

När du utformar ett meddelande kan du lägga till länkar till innehållet.

>[!NOTE]
>
>När spårning är aktiverat spåras alla länkar i meddelandeinnehållet.

Följ stegen nedan om du vill infoga länkar i ditt e-postinnehåll:

1. Markera ett element och klicka på **[!UICONTROL Insert link]** i det sammanhangsberoende verktygsfältet.

1. Välj den typ av länk som du vill skapa:

   ![](assets/message-tracking-insert-link.png){zoomable="yes"}

   * **[!UICONTROL External link]**: Infoga en länk till en extern URL.

     >[!AVAILABILITY]
     >
     >Följande funktioner (länk till **[!UICONTROL Landing page]**, **[!UICONTROL Subscription link]** och **[!UICONTROL Unsubscription link]**) har begränsad tillgänglighet (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

   * **[!UICONTROL Landing page]**: Infoga en länk till en landningssida. Om du väljer en dynamisk landningssida (med alternativet **[!UICONTROL Service from URL]** markerat) kan du välja vilken tjänst som helst i listan. [Läs mer](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable="yes"}

   * **[!UICONTROL Subscription link]**: Infoga en länk till en prenumerationstjänst. När användarna klickar på länken dirigeras de till den prenumerationsstartsida som refereras till i den valda tjänsten. [Läs mer](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable="yes"}

   * **[!UICONTROL Unsubscription link]**: Infoga en länk till en tjänst för avprenumeration. När prenumeranter klickar på länken dirigeras de till den startsida för prenumerationen som refereras till i den valda tjänsten. [Läs mer](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. Ange önskad URL-adress i motsvarande fält, eller välj en landningssida eller en tjänst, och definiera länkinställningar och format.

1. Lägg till en **[!UICONTROL Label]** och en **[!UICONTROL Link]**.

1. Spara ändringarna.

1. När länken har skapats kan du fortfarande ändra den från fliken **[!UICONTROL Settings]**.

   * Du kan redigera länken och ändra dess **[!UICONTROL Target]**.
   * Du kan välja att stryka under länken eller inte genom att markera motsvarande alternativ.

   ![](assets/message-tracking-link-settings.png){zoomable="yes"}

>[!NOTE]
>
>E-postmeddelanden av marknadsföringstyp måste innehålla en länk för avanmälan, vilket inte krävs för transaktionsmeddelanden. Meddelandekategorin (**[!UICONTROL Marketing]** eller **[!UICONTROL Transactional]**) definieras på kanalytnivå och när meddelandet skapas.

En specifik länk till spegelsidan bör läggas till i alla e-postmeddelanden. Läs mer om speglingssidan i [det här avsnittet](mirror-page.md).

## Hantera spårning {#manage-tracking}

Med [e-post-Designer](create-email-content.md) kan du hantera spårade URL-adresser, till exempel redigera spårningstypen för varje länk.

1. Klicka på ikonen **[!UICONTROL Links]** i den vänstra rutan om du vill visa en lista över alla URL:er för ditt innehåll som ska spåras.

   Med den här listan kan du ha en centraliserad vy och hitta varje URL i e-postinnehållet.

1. Om du vill redigera en länk klickar du på motsvarande pennikon.

   ![](assets/message-tracking-edit-links.png){zoomable="yes"}

1. Du kan ändra **[!UICONTROL Tracking Type]** om det behövs:

   ![](assets/message-tracking-edit-a-link.png){zoomable="yes"}

   För varje spårad URL kan du ange spårningsläget till något av följande värden:

   * **[!UICONTROL Tracked]**: Aktiverar spårning på den här URL:en.
   * **[!UICONTROL Opt out]**: Utser den här URL:en som en avanmälnings- eller avanmälnings-URL.
   * **[!UICONTROL Mirror page]**: Den här URL:en är en URL för en spegelsida.
   * **[!UICONTROL Never]**: Aktiverar aldrig spårning av den här URL:en. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Lägg till en **[!UICONTROL Category]** i länken för att gruppera spårade länkar och klicka på **[!UICONTROL Save]**.

   ![](assets/message-tracking-edit-a-link_2.png){zoomable="yes"}

1. När leveransen är klar öppnar du leveransrapporten. Under menyn **[!UICONTROL Tracking]** visar rapporten **[!UICONTROL URLs and click streams]** vilka URL:er från din leverans som är mest besökta. [Läs mer](../reporting/gs-reports.md)
