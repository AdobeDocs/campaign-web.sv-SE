---
audience: end-user
title: Använda arbetsflödesaktiviteten AND-join
description: Lär dig använda arbetsflödesaktiviteten OCH-join
badge: label="Begränsad tillgänglighet"
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: a0611ac41957b4bd7796c4c42c40232fba1dfc2b
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# AND-join {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join activity"
>abstract="The **Och-join** kan du synkronisera flera körningsgrenar i ett arbetsflöde. Den aktiveras när alla föregående aktiviteter har slutförts. På så sätt kan du se till att vissa aktiviteter är slutförda innan du fortsätter att köra arbetsflödet."

The **Och-join** aktiviteten är en **Flödeskontroll** aktivitet. Det gör att du kan synkronisera flera körningsgrenar i ett arbetsflöde.

Den här aktiviteten utlöser endast den utgående övergången när alla inkommande övergångar har aktiverats, det vill säga när alla föregående aktiviteter har slutförts. På så sätt kan du se till att vissa aktiviteter har slutförts innan du fortsätter att köra arbetsflödet.

## Konfigurera aktiviteten Och-join{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Konfigurera aktiviteten AND-join"
>abstract="Välj vilka aktiviteter du vill ansluta till. I **Primär uppsättning** väljer du vilken inkommande övergångspopulation som du vill behålla."

Följ de här stegen för att konfigurera **AND-join** aktivitet:

![](../assets/workflow-andjoin.png)

1. Lägg till flera aktiviteter, till exempel kanalaktiviteter, för att bilda minst två olika utförandegrenar.
1. Lägg till en **AND-join** till någon av grenarna.
1. I **Sammanfogningsalternativ** markerar du alla tidigare aktiviteter du vill delta i.
1. I **Primär uppsättning** väljer du vilken inkommande övergångspopulation som du vill behålla. Den utgående övergången kan bara innehålla en av de ingående övergångspopulationerna.

## Exempel{#and-join-example}

I följande exempel visas två arbetsflödesgrenar med e-post och SMS-leverans. AND-join utlöses när båda inkommande övergångar är aktiverade. Push-meddelandena skickas sedan först när båda leveranserna är klara.

![](../assets/workflow-andjoin-example.png){zoomable=&quot;yes&quot;}
