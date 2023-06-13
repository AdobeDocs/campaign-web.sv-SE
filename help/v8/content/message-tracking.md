---
audience: end-user
title: Spåra meddelanden
description: Lär dig hur du lägger till länkar och spårar skickade meddelanden
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Lägga till länkar och spåra meddelanden {#tracking}

Använd e-postdesignern för att lägga till länkar till ditt innehåll och spåra meddelanden som skickas för att övervaka mottagarnas beteende.

## Infoga länkar {#insert-links}

När du utformar ett meddelande kan du lägga till länkar till innehållet.

>[!NOTE]
>
>När spårning är aktiverat spåras alla länkar i meddelandeinnehållet.

Följ stegen nedan om du vill infoga länkar i ditt e-postinnehåll:

1. Markera ett element och klicka på **[!UICONTROL Insert link]** i kontextverktygsfältet.

   ![](assets/message-tracking-insert-link.png)

1. Lägg till en **[!UICONTROL Label]** och **[!UICONTROL Link]**.

1. Spara ändringarna.

1. När länken har skapats kan du fortfarande ändra den från **[!UICONTROL Settings]** -fliken.

   * Du kan redigera länken och ändra dess **[!UICONTROL Target]**.
   * Du kan välja att stryka under länken eller inte genom att markera motsvarande alternativ.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>E-postmeddelanden av marknadsföringstyp måste innehålla en länk för avanmälan, vilket inte krävs för transaktionsmeddelanden. Meddelandekategorin (**[!UICONTROL Marketing]** eller **[!UICONTROL Transactional]**) definieras vid kanalens ytnivå (dvs. meddelandeförinställning) och när meddelandet skapas.

En specifik länk till spegelsidan bör läggas till i alla e-postmeddelanden. Läs mer om speglingssidan i [det här avsnittet](mirror-page.md).

## Hantera spårning {#manage-tracking}

The [E-postdesigner](create-email-content.md) gör att du kan hantera spårade URL-adresser, till exempel redigera spårningstypen för varje länk.

1. Klicka på **[!UICONTROL Links]** i den vänstra rutan för att visa en lista över alla URL:er för ditt innehåll som ska spåras.

   Med den här listan kan du ha en centraliserad vy och hitta varje URL i e-postinnehållet.

1. Om du vill redigera en länk klickar du på motsvarande pennikon.

   ![](assets/message-tracking-edit-links.png)

1. Du kan ändra **[!UICONTROL Tracking Type]** vid behov:

   ![](assets/message-tracking-edit-a-link.png)

   För varje spårad URL kan du ange spårningsläget till något av följande värden:

   * **[!UICONTROL Tracked]**: Aktiverar spårning på denna URL.
   * **[!UICONTROL Opt out]**: Betraktar denna URL som en avanmälnings- eller avanmälnings-URL.
   * **[!UICONTROL Mirror page]**: Den här URL:en är en URL för en spegelsida.
   * **[!UICONTROL Never]**: Aktiverar aldrig spårning av den här URL:en. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Lägg till en **[!UICONTROL Category]** till länken för att gruppera spårade länkar och klicka på **[!UICONTROL Save]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. När leveransen är klar öppnar du leveransrapporten. Under **[!UICONTROL Tracking]** -menyn, **[!UICONTROL URLs and click streams]** rapporten visar vilka URL:er från din leverans som är mest besökta. [Läs mer](../reporting/gs-reports.md)
