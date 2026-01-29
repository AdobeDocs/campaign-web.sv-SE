---
audience: end-user
title: Skapa en SMS-leverans
description: Lär dig hur du skapar och skickar SMS med Adobe Campaign Web
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 7f7063572b95df9c289e614cb217239f579ddb27
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---

# Skapa en SMS-leverans {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="SMS-leveransegenskaper"
>abstract="Egenskaperna innehåller vanliga leveransparametrar som hjälper dig att namnge och klassificera leveransen. Om leveransen använder ett utökat schema är specifika fält för anpassade alternativ tillgängliga."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definiera SMS-målgruppen"
>abstract="Skapa en ny målgrupp eller välj en befintlig genom att klicka på knappen **Välj målgrupp** . Lägg till en kontrollgrupp om det behövs för att mäta effekten av leveransen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Ange en kontrollgrupp"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Val av SMS-mall"
>abstract="Välj en fördefinierad mall för att starta SMS-leveransen. Leveransmallar gör att ni kan återanvända anpassat innehåll och anpassade inställningar för alla kampanjer och leveranser."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/start/delivery-template" text="Använd leveransmallar"

Du kan skapa en fristående SMS-leverans eller skapa ett SMS i samband med ett kampanjarbetsflöde. Stegen nedan beskriver hur du får en fristående SMS-leverans (en bild). Om du arbetar i ett kampanjarbetsflöde beskrivs stegen för att skapa i [det här avsnittet](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Så här skapar du en ny fristående SMS-leverans:

1. Bläddra till menyn **[!UICONTROL Deliveries]** i den vänstra listen och klicka på knappen **[!UICONTROL Create delivery]**.

1. Välj SMS som kanal under avsnittet **[!UICONTROL Channel]** och välj en mall. [Läs mer om mallar](../msg/delivery-template.md)

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

   ![Skärmbild som visar knappen Skapa leverans och SMS-kanalval](assets/sms_create_1.png){zoomable="yes"}

1. Ange en **[!UICONTROL Label]** för leveransen och öppna listrutan **[!UICONTROL Additional options]**. Om leveransen använder ett utökat schema är specifika **anpassade alternativ**-fält tillgängliga.

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en specifik mapp.
   * **[!UICONTROL Delivery code]**: Organisera dina leveranser med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange leveransens natur för klassificeringssyften.
   +++

1. Klicka på knappen **[!UICONTROL Select audience]** om du vill ange en befintlig målgrupp eller skapa en egen. [Läs mer om målgrupper](../audience/about-recipients.md).

   ![Skärmbild som visar knappen Välj publik](assets/sms_create_2.png){zoomable="yes"}

   Lär dig hur du väljer en befintlig målgrupp på [den här sidan](../audience/add-audience.md).

   Lär dig hur du skapar en ny publik på [den här sidan](../audience/one-time-audience.md).

1. Aktivera alternativet **[!UICONTROL Enable control group]** om du vill ange en kontrollgrupp för att mäta effekten av leveransen. Meddelanden skickas inte till den kontrollgruppen, så du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](../audience/control-group.md)

1. Du kan konfigurera SMS-leveransen som en flerspråkig leverans för att skicka meddelanden baserat på det språk som används i profilen. [Läs mer](../msg/multilingual.md).

1. Klicka på **[!UICONTROL Edit content]** för att börja designa innehållet i SMS-meddelandet. [Läs mer](content-sms.md)

   ![Skärmbild med knappen Redigera innehåll](assets/sms_create_4.png){zoomable="yes"}

   Från den här skärmen kan du även [simulera ditt innehåll](../preview-test/preview-test.md) och [konfigurera erbjudanden](../msg/offers.md).

1. Om du vill schemalägga leveransen till ett visst datum och en viss tid aktiverar du alternativet **[!UICONTROL Enable scheduling]**. När du har initierat leveransen skickas meddelandet automatiskt på exakt det datum och klockslag som du anger för mottagaren. Läs mer om leveransplanering i [det här avsnittet](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Använd aktiviteten **Schemaläggaren** när en leverans skickas i ett arbetsflödes kontext. Läs mer på [den här sidan](../workflows/activities/scheduler.md).

1. Klicka på **[!UICONTROL Settings]** för att komma åt avancerade alternativ som är relaterade till din leveransmall. [Läs mer](../advanced-settings/delivery-settings.md)

   ![Skärmbild med inställningsknappen](assets/sms_create_3.png){zoomable="yes"}