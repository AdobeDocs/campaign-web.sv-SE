---
audience: end-user
title: Skapa en leverans av direktutskick
description: Lär dig skapa direktreklam med Adobe Campaign Web
exl-id: 9b5172b2-1880-4768-a33b-8a20ec5a30ab
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 5%

---

# Skapa en leverans av direktutskick {#create-direct-mail}

Du kan skapa en fristående direktutskick eller skapa en direktutskick i ett kampanjarbetsflöde. I stegen nedan beskrivs hur du skickar direktreklam i ett fristående (enstaka) exemplar. Om du arbetar i ett kampanjarbetsflöde beskrivs stegen för att skapa i [det här avsnittet](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Så här skapar du en ny fristående direktutskick:

1. Bläddra till menyn **[!UICONTROL Deliveries]** i den vänstra listen och klicka på knappen **[!UICONTROL Create delivery]**.

1. Under avsnittet **[!UICONTROL Channel]** väljer du **[!UICONTROL Direct mail]** som kanal och väljer en mall. [Läs mer om mallar](../msg/delivery-template.md)

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

   ![](assets/dm-create.png){zoomable="yes"}

1. Ange en **[!UICONTROL Label]** för leveransen och öppna listrutan **[!UICONTROL Additional options]**. Om leveransen baseras på ett utökat schema är specifika **anpassade alternativ**-fält tillgängliga.

   ![](assets/dm-properties.png){zoomable="yes"}

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en specifik mapp.
   * **[!UICONTROL Delivery code]**: Organisera dina leveranser med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange leveransens natur för klassificeringssyften.
+++

1. Klicka på knappen **[!UICONTROL Select audience]** om du vill ange en befintlig målgrupp eller skapa en egen.

   * [Lär dig hur du väljer en befintlig målgrupp](../audience/add-audience.md)
   * [Lär dig skapa en ny publik](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >Mottagarna av direktreklam måste innehålla minst sina namn och postadresser. En adress anses vara fullständig om fälten för namn, postnummer och ort inte är tomma. Mottagare med ofullständiga adresser utesluts från direktutskick.

1. Aktivera alternativet **[!UICONTROL Enable control group]** om du vill ange en kontrollgrupp för att mäta effekten av leveransen. Meddelanden skickas inte till den kontrollgruppen, så att du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. [Lär dig arbeta med kontrollgrupper](../audience/control-group.md)

1. Klicka på **[!UICONTROL Edit content]** för att definiera informationen (kolumnerna) som ska exporteras till extraheringsfilen. [Läs mer](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable="yes"}

1. Om du vill schemalägga leveransen till ett visst datum och en viss tid aktiverar du alternativet **[!UICONTROL Enable scheduling]**. När du har initierat leveransen genereras extraheringsfilen automatiskt vid exakt det datum och klockslag som du har definierat. [Lär dig schemalägga leveranser](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >När en leverans skickas i ett arbetsflödes kontext måste du använda aktiviteten **Schemaläggaren**. Läs mer på [den här sidan](../workflows/activities/scheduler.md).

1. Klicka på **[!UICONTROL Settings]** för att komma åt avancerade alternativ som är relaterade till din leveransmall. [Läs mer](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable="yes"}

1. När leveransen av direktreklam är klar klickar du på knappen **[!UICONTROL Review and send]** för att validera och skicka leveransen och generera extraheringsfilen. [Lär dig hur du förhandsgranskar och skickar direktreklam](send-direct-mail.md)
