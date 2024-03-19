---
audience: end-user
title: Skapa en leverans av direktutskick
description: Lär dig skapa direktreklam med Adobe Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 5%

---


# Skapa en leverans av direktutskick {#create-direct-mail}

Du kan skapa en fristående direktutskick eller skapa en direktutskick i ett kampanjarbetsflöde. I stegen nedan beskrivs hur du skickar direktreklam i ett fristående (enstaka) exemplar. Om du arbetar i ett kampanjarbetsflöde beskrivs stegen för att skapa i [det här avsnittet](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Så här skapar du en ny fristående direktutskick:

1. Gå till **[!UICONTROL Deliveries]** till vänster och klicka på  **[!UICONTROL Create delivery]** -knappen.

1. Under **[!UICONTROL Channel]** avsnitt, välja **[!UICONTROL Direct mail]** som kanal och välj en mall. [Läs mer om mallar](../msg/delivery-template.md)

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

   ![](assets/dm-create.png){zoomable=&quot;yes&quot;}

1. Ange en **[!UICONTROL Label]** för leverans och åtkomst till **[!UICONTROL Additional options]** nedrullningsbar meny. Om leveransen baseras på ett utökat schema, **Anpassade alternativ** fält är tillgängliga.

   ![](assets/dm-properties.png){zoomable=&quot;yes&quot;}

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en viss mapp.
   * **[!UICONTROL Delivery code]**: Ordna leveranserna med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange leveransens natur för klassificering.
+++

1. Klicka på **[!UICONTROL Select audience]** för att rikta sig till en befintlig målgrupp eller skapa en egen.

   * [Lär dig hur du väljer en befintlig målgrupp](../audience/add-audience.md)
   * [Lär dig skapa en ny publik](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Mottagarna av direktreklam måste innehålla minst sina namn och postadresser. En adress anses vara fullständig om fälten för namn, postnummer och ort inte är tomma. Mottagare med ofullständiga adresser utesluts från direktutskick.

1. Aktivera **[!UICONTROL Enable control group]** kan du ange en kontrollgrupp för att mäta effekten av leveransen. Meddelanden skickas inte till den kontrollgruppen, så att du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. [Lär dig hur du arbetar med kontrollgrupper](../audience/control-group.md)

1. Klicka **[!UICONTROL Edit content]** för att definiera den information (kolumner) som ska exporteras till extraheringsfilen. [Läs mer](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable=&quot;yes&quot;}

1. Aktivera **[!UICONTROL Enable scheduling]** alternativ. När du har initierat leveransen genereras extraheringsfilen automatiskt vid exakt det datum och klockslag som du har definierat. [Lär dig schemalägga leveranser](../msg/gs-messages.md#gs-schedule).

   >[!NOTE]
   >
   >När en leverans skickas i ett arbetsflödes sammanhang måste du använda **Schemaläggare** aktivitet. Läs mer på [den här sidan](../workflows/activities/scheduler.md).

1. Klicka **[!UICONTROL Settings]** för att få tillgång till avancerade alternativ för leveransmallen. [Läs mer](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable=&quot;yes&quot;}

1. När du är klar klickar du på **[!UICONTROL Review and send]** för att validera och skicka leveransen och generera extraheringsfilen. [Lär dig hur du förhandsgranskar och skickar direktreklam](send-direct-mail.md)

