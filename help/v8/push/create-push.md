---
audience: end-user
title: Skapa en leverans av push-meddelanden
description: Lär dig hur du skapar ett push-meddelande med Adobe Campaign Web
badge: label="Beta"
source-git-commit: e934bc041b76511c0f4fec22b6abc41c647e1cb3
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 4%

---

# Skapa en leverans av push-meddelanden {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definiera penselmålgruppen"
>abstract="Välj den bästa målgruppen för ditt push-meddelande."

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Push-meddelandemall"
>abstract="Välj en mall för push-meddelanden för att starta din push-leverans."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Push-leveransegenskaper"
>abstract="Hantera egenskaperna för push-leverans."

1. Från **[!UICONTROL Deliveries]** hemsida, klicka **[!UICONTROL Create delivery]**.

1. Under **[!UICONTROL Channel]** väljer du Push-meddelanden som kanal och väljer en mall beroende på vilket operativsystem du har valt: Android eller iOS. [Läs mer om mallar](../msg/delivery-template.md)

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

   ![](assets/push_create_1.png)

1. Ange en **[!UICONTROL Label]** för leverans och åtkomst till **[!UICONTROL Additional options]** nedrullningsbar meny.

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en viss mapp.
   * **[!UICONTROL Delivery code]**: Ordna leveranserna med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange e-postens natur för klassificeringsändamål.
+++

1. Från **[!UICONTROL Audience]** väljer du det program som du vill använda för leveransen.

1. Klicka på **[!UICONTROL Select audience]** för att rikta sig till en befintlig målgrupp eller skapa en egen. [Läs mer](../audience/about-audiences.md)

   Observera att ditt push-meddelande som standard skickas till alla prenumeranter på programmet.

   ![](assets/push_create_2.png)

1. Aktivera **[!UICONTROL Enable control]** gruppalternativ för att ställa in en kontrollgrupp för att mäta effekten av leveransen, så att du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](../audience/control-group.md)

1. Klicka **[!UICONTROL Edit content]** för att börja designa innehållet i ditt push-meddelande. [Läs mer](content-push.md)

   ![](assets/push_create_5.png)

   Från den här skärmen kan du även [simulera ditt innehåll](../preview-test/preview-test.md) och [konfigurera erbjudanden](../content/offers.md).

1. Aktivera **[!UICONTROL Enable scheduling]** alternativ. När du har initierat leveransen skickas meddelandet automatiskt på exakt det datum och klockslag som du har angett för mottagaren. Läs mer om leveransplanering i [det här avsnittet](../msg/gs-messages.md#gs-schedule)

   ![](assets/push_create_3.png)

1. Klicka **[!UICONTROL Configure delivery settings]** för att få tillgång till avancerade alternativ för leveransmallen. [Läs mer](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_4.png)
