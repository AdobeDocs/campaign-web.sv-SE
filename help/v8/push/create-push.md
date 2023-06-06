---
audience: end-user
title: Skapa en leverans av push-meddelanden
description: Lär dig hur du skapar ett push-meddelande med Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 7fa6a5adb22b4fc4569b93383a8e269703944582
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 3%

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

1. Under **[!UICONTROL Channel]** väljer du Push-meddelande som kanal och väljer en mall. Läs mer om mallar

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

1. Ange **[!UICONTROL Label]** för leverans och åtkomst till **[!UICONTROL Additional options]** nedrullningsbar meny.

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en viss mapp.
   * **[!UICONTROL Delivery code]**: Ordna leveranserna med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange e-postens natur för klassificeringssyften.
+++

1. Från **[!UICONTROL Audience]** väljer du det program som du vill använda för leveransen.

1. Klicka på **[!UICONTROL Select audience]** för att rikta sig till en befintlig målgrupp eller skapa en egen. Läs mer.

   Observera att ditt push-meddelande som standard skickas till alla prenumeranter på programmet.

1. Aktivera **[!UICONTROL Enable control]** gruppalternativ för att ställa in en kontrollgrupp för att mäta effekten av leveransen, så att du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. Läs mer

1. Klicka **[!UICONTROL Edit content]** för att börja designa innehållet i ditt push-meddelande.

1. Om du vill schemalägga leveransen till ett visst datum och en viss tid aktiverar du **[!UICONTROL Enable scheduling]** alternativ. När du har initierat leveransen skickas meddelandet automatiskt på exakt det datum och klockslag som du har angett för mottagaren.

1. Klicka på Konfigurera leveransinställningar för att komma åt avancerade alternativ som är relaterade till leveransmallen. [Läs mer](../advanced-settings/delivery-settings.md)
