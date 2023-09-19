---
audience: end-user
title: Kom igång med kampanjer
description: Lär dig hur du börjar med flerkanalskampanjer
badge: label="Beta"
source-git-commit: 1bbbcd0ad2e83bad2e35c28184d13a63da77c081
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 1%

---


# Få tillgång till och hantera era kampanjer{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Kampanjschema"
>abstract="Ange eller ändra kampanjschemat."

Om du vill skapa en ny kampanj eller hantera befintliga kampanjer klickar du på **[!UICONTROL Campaigns]** till vänster.

## Lista över kampanjer {#access-campaigns}

Det finns två flikar i kampanjlistan:

* The **Bläddra** alla befintliga kampanjer visas på fliken. Du kan klicka på en kampanj för att öppna dess instrumentpanel eller skapa en ny kampanj genom att klicka på **Skapa kampanj** -knappen. Se det här [section](create-campaigns.md#create-campaigns).

* The **Mallar** På -fliken visas alla tillgängliga kampanjmallar. Du kan visa en befintlig mall eller skapa en ny. [Läs mer](#manage-campaign-templates).

![Kampanjlista](assets/campaign-list.png)

Som standard visar varje kampanj i listan information om dess aktuella status, skapandedatum, senaste gången den ändrades, osv.

Du kan anpassa de kolumner som visas genom att klicka på **Konfigurera kolumn för en anpassad layout** -ikonen i det övre högra hörnet av listan. På så sätt kan du lägga till ytterligare information i listan. Dessutom finns det ett sökfält och filter som gör det enklare att söka i listan. [Läs mer](../get-started/user-interface.md#list-screens).

Du kan till exempel filtrera efter kampanjschemat. Öppna filterpanelen och använd **Start - slutdatum** avsnitt:

![Kampanjfilter](assets/campaign-filter-on-dates.png)

## Kampanjinstrumentpanel{#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Lista över leveranser i kampanjen"
>abstract="The **Leveranser** På fliken visas alla leveranser som är kopplade till den aktuella kampanjen. Klicka på namnet på en leverans för att redigera den. Använd knappen Skapa leverans för att lägga till en ny leverans för kampanjen."

I **Bläddra** klickar du på en kampanj för att visa information om den.

![Kampanjinstrumentpanel](assets/campaign-dashboard.png)

Status och schema för kampanjen visas högst upp på skärmen. Du kan använda **Konfigurera kampanjinställningar** om du vill ändra kampanjens egenskaper som definierades när kampanjen skapades. Det finns tre knappar som gör att du kan visa loggar, rapportera, duplicera eller ta bort kampanjen. Se det här [section](create-campaigns.md#create-campaigns)

Det finns två flikar:

* The **Arbetsflöden** På -fliken visas alla arbetsflöden som är kopplade till kampanjen. På den här fliken kan du även skapa ett nytt arbetsflöde i kampanjen. Se det här [section](create-campaigns.md#create-campaigns).

* The **Leveranser** På fliken visas alla leveranser som är kopplade till den aktuella kampanjen. Du kan också skapa en ny leverans i kampanjen. Se det här [section](create-campaigns.md#create-campaigns).

## Duplicera och ta bort en kampanj

Du kan duplicera eller ta bort en kampanj:

* Klicka på ellipsknappen i listan över kampanjer och välj sedan **Duplicera** eller **Ta bort**.
* från själva kampanjen klickar du på **Mer** knapp och markera **Duplicera** eller **Ta bort**.

>[!NOTE]
>
>The **Leveranser** visas alla leveranser som är kopplade till kampanjen. Leveranser som har skapats i ett arbetsflöde kan dock inte tas bort därifrån. Om du vill ta bort en leverans som har skapats i ett arbetsflöde måste du ta bort leveransaktiviteten från arbetsflödet. [Läs mer](../msg/gs-messages.md#delivery-delete).

## Arbeta med kampanjmallar{#manage-campaign-templates}

Kampanjmallar innehåller förkonfigurerade inställningar som kan återanvändas för att skapa nya arbetsflöden. Det finns en uppsättning inbyggda mallar som hjälper dig att komma igång. Du kan skapa och konfigurera kampanjmallar och sedan skapa kampanjer utifrån dessa mallar.

En kampanjmall kan lagra följande information:

* kampanjens **Egenskaper** och **Schema** inställningar
* arbetsflödesmallar
* leveransmallar

Så här skapar du en kampanjmall:

1. Klicka på **[!UICONTROL Campaigns]** -menyn, bläddra till **Mallar** klickar du på **[!UICONTROL Create template]** -knappen.
1. Välj **Mall** för att använda och tillhandahålla en etikett för kampanjen. På så sätt kan du basera den nya mallen på en mall som redan har skapats.
1. Om det behövs kan du ändra följande **Ytterligare alternativ**: internt namn, mapp, tilldelad, beskrivning och typ.
1. Definiera **Schema** av er kampanj. Lär dig hur du ställer in kampanjschemat i [det här avsnittet](create-campaigns.md#campaign-schedule)
1. Klicka **Skapa**.
1. Lägg till arbetsflöden och leveransmallar i kampanjen.
