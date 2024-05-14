---
audience: end-user
title: Kom igång med kampanjer
description: Lär dig hur du börjar med flerkanalskampanjer
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
source-git-commit: 5b42671173e7fd7f024eb7eb03a0836eae7ef622
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---

# Få tillgång till och hantera era kampanjer{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Kampanjschema"
>abstract="Ange eller ändra kampanjschemat."

Klicka på **[!UICONTROL Campaigns]** till vänster.

## Lista över kampanjer {#access-campaigns}

Det finns två flikar i kampanjlistan:

* The **Bläddra** alla befintliga kampanjer visas på fliken. Du kan klicka på en kampanj för att öppna dess instrumentpanel eller skapa en ny kampanj genom att klicka på **Skapa kampanj** -knappen. Se det här [section](create-campaigns.md#create-campaigns).

* The **Mallar** På -fliken visas alla tillgängliga kampanjmallar. Du kan visa en befintlig mall eller skapa en ny. [Läs mer](#manage-campaign-templates).

![Kampanjlista](assets/campaign-list.png)

Som standard visar varje kampanj i listan information om dess aktuella status, start- och slutdatum, skapandedatum, senaste gången den ändrades osv.

Du kan anpassa de kolumner som visas genom att klicka på **Konfigurera kolumn för en anpassad layout** -ikonen i det övre högra hörnet av listan. På så sätt kan du lägga till eller ta bort kolumner och ändra ordning på information i kampanjlistan.

Dessutom finns det ett sökfält och filter som gör det enklare att söka i listan. [Läs mer](../get-started/user-interface.md#list-screens).

Du kan till exempel filtrera efter kampanjschemat. Öppna filterpanelen och använd **Start - slutdatum** avsnitt:

![Kampanjfilter](assets/campaign-filter-on-dates.png)

## Kampanjinstrumentpanel {#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Lista över leveranser i kampanjen"
>abstract="The **Leveranser** På fliken visas alla leveranser som är kopplade till den aktuella kampanjen. Klicka på namnet på en leverans för att redigera den. Använd knappen Skapa leverans för att lägga till en ny leverans för kampanjen."

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Arbetsflödeslista i en kampanj"
>abstract="The **Arbetsflöde** På -fliken visas alla arbetsflöden som är länkade till den aktuella kampanjen."

I **Bläddra** klickar du på ett kampanjnamn för att visa information om kampanjen.

![Kampanjinstrumentpanel](assets/campaign-dashboard.png)

Status och schema för kampanjen visas högst upp på skärmen. Du kan använda **Inställningar** om du vill uppdatera egenskaperna för kampanjen, till exempel etiketten, mappen och beskrivningen. Du kan också ändra kampanjschemat från inställningsskärmen. Läs mer om kampanjschemat i [det här avsnittet](create-campaigns.md#campaign-schedule).

På kampanjpanelen använder du **Loggar** och **Rapporter** knappar för att övervaka kampanjen. Läs mer om detta [section](create-campaigns.md#create-campaigns)

På kontrollpanelen visas två huvudflikar för varje kampanj: Arbetsflöden och Leveranser.

* The **Arbetsflöden** På -fliken visas alla arbetsflöden som är kopplade till kampanjen. På den här fliken kan du även skapa ett nytt arbetsflöde i kampanjen. Se det här [section](create-campaigns.md#create-campaigns).

* The **Leveranser** På fliken visas alla leveranser som har skapats i den aktuella kampanjen. Du kan också skapa en ny leverans i kampanjen. Se det här [section](create-campaigns.md#create-campaigns).

>[!NOTE]
>
>The **Leveranser** visas alla leveranser som är kopplade till kampanjen. Leveranser som har skapats i ett arbetsflöde kan dock inte tas bort därifrån. Om du vill ta bort en leverans som har skapats i ett arbetsflöde måste du ta bort leveransaktiviteten från arbetsflödet. [Läs mer](../msg/gs-messages.md#delivery-delete).


## Ta bort en kampanj {#campaign-delete}

Du kan ta bort en kampanj på två sätt:

* Klicka på ellipsknappen i listan över kampanjer och välj sedan **Ta bort**

  ![Ta bort en kampanj från listan över kampanjer](assets/delete-a-campaign-from-list.png)

* från själva kampanjen klickar du på **Mer** knapp och markera **Ta bort**

  ![Ta bort en kampanj från kampanjinstrumentpanelen](assets/delete-a-campaign-from-dashboard.png)


## Duplicera en kampanj {#campaign-duplicate}

Du kan duplicera en kampanj på två sätt:

* Klicka på ellipsknappen i listan över kampanjer och välj sedan **Duplicera**

* från själva kampanjen klickar du på **Mer** knapp och markera **Duplicera**

I båda fallen måste du bekräfta dupliceringen för att skapa den nya kampanjen. Kampanjens etikett **Kopia av`<label of the initial campaign`**. Bläddra till kampanjinställningarna för att uppdatera den här etiketten.


## Arbeta med kampanjmallar{#manage-campaign-templates}

Kampanjmallar innehåller förkonfigurerade inställningar som kan återanvändas för att skapa nya kampanjer. Det finns en uppsättning inbyggda mallar som hjälper dig att komma igång. Du kan skapa och konfigurera kampanjmallar och sedan skapa kampanjer utifrån dessa mallar.

En kampanjmall kan lagra följande information:

* kampanjen **Inställningar**
* kampanjen  **Schema**
* arbetsflödesmallar
* leveransmallar

Så här skapar du en kampanjmall:

1. Klicka på **[!UICONTROL Campaigns]** -menyn, bläddra till **Mallar** klickar du på **[!UICONTROL Create template]** -knappen.
1. Välj **Mall** att använda. På så sätt kan du basera den nya mallen på en mall som du tidigare har skapat.
1. Ange en etikett för mallen.
1. Om det behövs kan du ändra följande **Ytterligare alternativ**: internt namn, mapp, tilldelad, beskrivning och typ.
1. Definiera **Schema** av er kampanj. Lär dig hur du ställer in kampanjschemat i [det här avsnittet](create-campaigns.md#campaign-schedule)
1. Klicka **Skapa**.
1. Lägg till arbetsflöden och leveransmallar i kampanjen.
