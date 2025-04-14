---
audience: end-user
title: Välj en befintlig målgrupp
description: Lär dig hur du väljer en målgrupp
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Välj en befintlig målgrupp {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Välj en befintlig målgrupp"
>abstract="Bläddra i listan för att välja en befintlig målgrupp. Använd ikonen Visa filter om du vill filtrera listan eller markera en viss mapp."

I det här avsnittet beskrivs hur du väljer en befintlig målgrupp när du definierar målpopulationen för en leverans. När du definierar huvudmålet för en leverans kan du också:
* [Skapa en engångspublik](one-time-audience.md) med frågemodelleraren.
* [Läs in en målgrupp från en extern fil](file-audience.md) (endast för e-post).

Målgrupper som kan användas för leveranser är tillgängliga från den vänstra menyn **Målgrupp**. De kommer från flera källor, till exempel kundkonsolen, målgruppsarbetsflöden för Campaign-webben eller Adobe Experience Platform. [Läs mer om målgrupper](manage-audience.md)

Följ stegen nedan för att välja en befintlig målgrupp för ditt meddelande:

1. Klicka på knappen **[!UICONTROL Select audience]** i sektionen **Målgrupp** i leveransassistenten och välj sedan **[!UICONTROL Select audience]**.

   [I den här skärmbilden visas knappen **Välj målgrupp** i leveransassistenten.](assets/create-audience.png){zoomable="yes"}

1. På den här skärmen visas alla befintliga målgrupper för den aktuella mappen.

   [På den här skärmbilden visas en lista över befintliga målgrupper i den aktuella mappen.](assets/create-audience2.png){zoomable="yes"}

   Om du vill välja en målgrupp från Adobe Experience Platform går du till `AEP Audiences folder` i skärmens filteravsnitt. [Läs mer om Adobe Experience Platform-målgrupper](manage-audience.md#monitor)

   [På den här skärmbilden visas filteravsnittet med AEP Audiences-mappen markerad.](assets/select-audience-folder.png){zoomable="yes"}

1. I filteravsnittet kan du komma åt filteralternativ för att förfina målgruppslistan. Om du vill göra det klickar du på **Lägg till regler** för att komma åt frågemodelleraren, som du kan använda för att skapa avancerade filter för listan över målgrupper. [Lär dig använda frågemodelleraren](../query/query-modeler-overview.md)

   Du kan till exempel definiera en regel som ska filtreras efter målgruppernas ursprung, vilket visas nedan:

   [På den här skärmbilden visas ett filter som tillämpas på målgrupper baserat på deras ursprung.](assets/filter-on-aep-audience.png){zoomable="yes"}

1. Klicka på **Bekräfta** för att lägga till målgruppen som huvudmål för leveransen. När du är klar kan du förfina målgruppen med frågemodelleraren genom att klicka på knappen **Redigera regler** .

   [I den här skärmbilden visas knappen **Redigera regler** för att förfina målgruppen.](assets/refine-audience.png){zoomable="yes"}

1. Ni kan också ställa in en kontrollgrupp för att mäta effekten av era kampanjer. Kontrollgruppen tar inte emot meddelandet. På så sätt kan du jämföra beteendet hos den population som fick meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](control-group.md)