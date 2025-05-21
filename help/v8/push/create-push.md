---
audience: end-user
title: Skapa en leverans av push-meddelanden
description: Lär dig hur du skapar ett push-meddelande med Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 1%

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
>abstract="Definiera dina egenskaper för push-leverans. Ange push-filens etikett och använd **ytterligare alternativ** för att konfigurera det interna namnet, leveransmappen och koden. Du kan också ange en egen beskrivning."

Du kan skapa en fristående leverans av push-meddelanden eller skapa ett push-meddelande i samband med ett kampanjarbetsflöde. Stegen nedan beskriver proceduren för en fristående push-leverans (en bild). Om du arbetar i ett kampanjarbetsflöde beskrivs stegen för att skapa i [det här avsnittet](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Skapa en push-leverans {#create-push-delivery}

Så här skapar du en ny fristående push-leverans:

1. Bläddra till menyn **[!UICONTROL Deliveries]** i den vänstra listen och klicka på knappen **[!UICONTROL Create delivery]**.

1. Under avsnittet **[!UICONTROL Channel]** väljer du **Push-meddelande** som kanal och väljer en mall, beroende på vilket operativsystem du har valt: Android eller iOS. [Läs mer om mallar](../msg/delivery-template.md)

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

   ![Skärmbild som visar hur en push-leverans skapas](assets/push_create_1.png){zoomable="yes"}

## Konfigurera leveransinställningarna {#configure-push-settings}

Konfigurera leveransinställningarna enligt nedan:

1. Ange en **[!UICONTROL Label]** för leveransen. Som standard anges etiketten med etiketten för den valda mallen. Den bör uppdateras.

1. Bläddra i listrutan **[!UICONTROL Additional options]** för att anpassa alternativen, om det behövs. Om leveransen baseras på ett utökat schema är specifika **anpassade alternativ**-fält tillgängliga.

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en specifik mapp.
   * **[!UICONTROL Delivery code]**: Organisera dina leveranser med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange leveransens natur för klassificeringssyften.
+++

## Välj publik för push-leverans {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definiera målgruppen för push-meddelanden"
>abstract="Om du vill definiera målgruppen för meddelandet måste du först välja den app som är kopplad till push-leveransen. Som standard skickas ditt push-meddelande till alla prenumeranter på programmet. Du kan förfina en viss målgrupp genom att klicka på knappen **Välj målgrupp** . Lägg till en kontrollgrupp om det behövs för att mäta effekten av leveransen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Ange en kontrollgrupp"

Du måste först välja appen och sedan kan du förfina målgruppen för push-meddelanden enligt följande:

1. I avsnittet **[!UICONTROL Audience]** väljer du det program som du vill använda för leveransen. Som standard skickas ditt push-meddelande till alla prenumeranter på programmet. Du kan förfina till en viss målgrupp genom att klicka på knappen **[!UICONTROL Select audience]**.

   ![Skärmbild som visar målgruppsval för push-leverans](assets/push_create_2.png){zoomable="yes"}

1. Välj en befintlig målgrupp, eller skapa en egen målgrupp, för att förfina målpopulationen för din push-leverans. För push-meddelanden är [måldimensionen](../audience/about-recipients.md#targeting-dimensions) som standard **prenumerantprogrammet** (nms:appSubscriptionRcp), som är länkat till mottagartabellen.

   Lär dig hur du väljer en befintlig målgrupp på [den här sidan](../audience/add-audience.md).

   Lär dig hur du skapar en ny publik på [den här sidan](../audience/one-time-audience.md).

1. Aktivera alternativet **[!UICONTROL Enable control group]** om du vill ange en kontrollgrupp för att mäta effekten av leveransen. Meddelanden skickas inte till den kontrollgruppen, så du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](../audience/control-group.md).

## Definiera innehållet i push-meddelanden {#create-content-push}

Klicka på **[!UICONTROL Edit content]** om du vill definiera innehållet i meddelandet. [Läs mer](content-push.md).

![Skärmbild som visar innehållsredigering för push-leverans](assets/push_create_5.png){zoomable="yes"}

Från den här skärmen kan du även [simulera ditt innehåll](../preview-test/preview-test.md) och [konfigurera erbjudanden](../msg/offers.md).

## Schemalägg leverans {#schedule-push}

När en leverans skickas i ett arbetsflödes kontext måste du använda aktiviteten **Schemaläggaren**. Läs mer på [den här sidan](../workflows/activities/scheduler.md). Stegen nedan gäller endast fristående leveranser.

Så här schemalägger du en fristående push-leverans till ett visst datum och en viss tid:

1. Bläddra till avsnittet **[!UICONTROL Schedule]** i leveransegenskaperna.

1. Använd växlingsknappen **[!UICONTROL Enable scheduling]** för att aktivera den.

1. Ange önskat datum och klockslag för sändning.

När du har initierat leveransen skickas meddelandet automatiskt på exakt det datum och klockslag som du har angett för mottagaren.

![Skärmbild med schemaläggningsalternativ för push-leverans](assets/push_create_3.png){zoomable="yes"}

Läs mer om leveransplanering i [det här avsnittet](../msg/gs-deliveries.md#gs-schedule).

## Avancerade inställningar för leverans {#adv-push}

Klicka på **[!UICONTROL Configure delivery settings]** för att komma åt avancerade alternativ som är relaterade till din leveransmall. [Läs mer](../advanced-settings/delivery-settings.md).

![Skärmbild med avancerade inställningar för push-leverans](assets/push_create_4.png){zoomable="yes"}