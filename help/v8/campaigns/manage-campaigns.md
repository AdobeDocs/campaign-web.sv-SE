---
audience: end-user
title: Kom igång med kampanjer
description: Lär dig hur du börjar med flerkanalskampanjer
badge: label="Alfa"
source-git-commit: c9954ce69e50e1c8db2532be3292f71ff20f9f74
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---


# Få tillgång till och hantera era kampanjer{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Kampanjschema"
>abstract="Ange eller ändra kampanjschemat."

Om du vill skapa en ny kampanj eller hantera befintliga kampanjer klickar du på **[!UICONTROL Campaigns]** till vänster.

## Kampanjlistan{#access-campaigns}

Det finns två flikar i kampanjlistan:

* The **Bläddra** alla befintliga kampanjer visas på fliken. Du kan klicka på en kampanj för att öppna instrumentpanelen eller skapa en ny kampanj genom att klicka på **Skapa kampanj** -knappen. Se det här [section](create-campaigns.md#create-campaigns).

* The **Mallar** På -fliken visas alla tillgängliga kampanjmallar. Kampanjmallar är förkonfigurerade så att de kan återanvändas när nya kampanjer skapas. De skapas från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html)

![Kampanjlista](assets/campaign-list.png)

Som standard visar varje kampanj i listan information om dess aktuella status, skapandedatum, senaste gången den ändrades, osv.

Du kan anpassa de kolumner som visas genom att klicka på **Konfigurera kolumn för en anpassad layout** -ikonen i det övre högra hörnet av listan. På så sätt kan du lägga till ytterligare information i listan. Dessutom finns det ett sökfält och filter som gör det enklare att söka i listan. [Läs mer](../get-started/user-interface.md#list-screens).

Du kan till exempel filtrera efter kampanjschemat. Öppna filterpanelen och använd **Start - slutdatum** avsnitt:

![Kampanjfilter](assets/campaign-filter-on-dates.png)

## Kontrollpanelen för kampanjer{#campaign-dashboard}

I **Bläddra** klickar du på en kampanj för att visa information om den.

![Kontrollpanel för kampanj](assets/campaign-dashboard.png)

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
