---
audience: end-user
title: Skapa en leverans av push-meddelanden
description: Lär dig hur du skapar ett push-meddelande med Adobe Campaign Web
badge: label="Begränsad tillgänglighet"
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 2%

---

# Skapa en leverans av push-meddelanden {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Push-meddelandemall"
>abstract="Välj en mall för push-meddelanden för att starta din push-leverans. Leveransmallar gör det enkelt att återanvända anpassat innehåll och anpassade inställningar i kampanjer och leveranser."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Använd leveransmallar"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Push-leveransegenskaper"
>abstract="Definiera dina egenskaper för push-leverans. Ange push-filens etikett och använd **Ytterligare alternativ** för att konfigurera internt namn, leveransmapp och kod. Du kan också ange en egen beskrivning."

Du kan skapa en fristående leverans av push-meddelanden eller skapa ett push-meddelande i samband med ett kampanjarbetsflöde. Stegen nedan beskriver proceduren för en fristående push-leverans (en bild). Om du arbetar i ett kampanjarbetsflöde visas stegen för att skapa i [det här avsnittet](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Skapa en push-leverans {#create-push-delivery}

Så här skapar du en ny fristående push-leverans:

1. Gå till **[!UICONTROL Deliveries]** till vänster och klicka på  **[!UICONTROL Create delivery]** -knappen.

1. Under **[!UICONTROL Channel]** avsnitt, välja **Push-meddelande** som kanal och välj en mall, beroende på vilket operativsystem enheten har valt: Android eller iOS. [Läs mer om mallar](../msg/delivery-template.md)

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

   ![](assets/push_create_1.png)

## Konfigurera leveransinställningarna {#configure-push-settings}

Konfigurera leveransinställningarna enligt nedan:

1. Ange en **[!UICONTROL Label]** för leveransen. Som standard anges etiketten med etiketten för den valda mallen. Den bör uppdateras.

1. Sök i **[!UICONTROL Additional options]** för att anpassa alternativen, om det behövs. Om leveransen baseras på ett utökat schema, **Anpassade alternativ** fält är tillgängliga.

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en viss mapp.
   * **[!UICONTROL Delivery code]**: Ordna leveranserna med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange e-postens natur för klassificeringsändamål.
+++


## Välj publik för push-leverans {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definiera målgruppen för push-meddelanden"
>abstract="Om du vill definiera målgruppen för meddelandet måste du först välja den app som är kopplad till push-leveransen. Som standard skickas ditt push-meddelande till alla prenumeranter på programmet. Du kan förfina till en viss målgrupp genom att klicka på **Välj målgrupp** -knappen. Lägg till en kontrollgrupp om det behövs för att mäta effekten av leveransen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Ange en kontrollgrupp"


Du måste först välja appen och sedan kan du förfina målgruppen för push-meddelanden enligt följande:

1. Från **[!UICONTROL Audience]** väljer du det program som du vill använda för leveransen. Som standard skickas ditt push-meddelande till alla prenumeranter på programmet. Du kan förfina till en viss målgrupp genom att klicka på **[!UICONTROL Select audience]** -knappen.

   ![](assets/push_create_2.png)

1. Välj en befintlig målgrupp, eller skapa en egen målgrupp, för att förfina målpopulationen för din push-leverans. Standardvärdet för push-meddelanden [måldimension](../audience/about-recipients.md#targeting-dimensions) är **Prenumerationsprogram** (nms:appSubscriptionRcp), som är länkad till mottagartabellen.

   Lär dig hur du väljer en befintlig målgrupp i [den här sidan](../audience/add-audience.md)

   Lär dig skapa en ny publik i [den här sidan](../audience/one-time-audience.md)

1. Aktivera **[!UICONTROL Enable control group]** kan du ange en kontrollgrupp för att mäta effekten av leveransen. Meddelanden skickas inte till den kontrollgruppen, så att du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](../audience/control-group.md)

## Definiera innehållet i push-meddelanden {#create-content-push}

Om du vill definiera innehållet i meddelandet klickar du på **[!UICONTROL Edit content]**. [Läs mer](content-push.md)

![](assets/push_create_5.png)

Från den här skärmen kan du även [simulera ditt innehåll](../preview-test/preview-test.md) och [konfigurera erbjudanden](../msg/offers.md).

## Schemalägg leverans {#schedule-push}

Aktivera **[!UICONTROL Enable scheduling]** alternativ. När du har initierat leveransen skickas meddelandet automatiskt på exakt det datum och klockslag som du har angett för mottagaren. Läs mer om leveransplanering i [det här avsnittet](../msg/gs-messages.md#gs-schedule)

![](assets/push_create_3.png)


## Avancerade inställningar för leverans {#adv-push}

Klicka **[!UICONTROL Configure delivery settings]** för att få tillgång till avancerade alternativ för leveransmallen. [Läs mer](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png)
