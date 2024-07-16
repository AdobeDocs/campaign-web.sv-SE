---
audience: end-user
title: Använda arbetsflödesaktiviteten AND-join
description: Lär dig använda arbetsflödesaktiviteten OCH-join
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# AND-join {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join activity"
>abstract="Med aktiviteten **And-join** kan du synkronisera flera körningsgrenar i ett arbetsflöde. Den aktiveras när alla föregående aktiviteter har slutförts. På så sätt kan du se till att vissa aktiviteter är slutförda innan du fortsätter att köra arbetsflödet."

Aktiviteten **And-join** är en **Flow control** -aktivitet. Det gör att du kan synkronisera flera körningsgrenar i ett arbetsflöde.

Den här aktiviteten utlöser endast den utgående övergången när alla inkommande övergångar har aktiverats, det vill säga när alla föregående aktiviteter har slutförts. På så sätt kan du se till att vissa aktiviteter har slutförts innan du fortsätter att köra arbetsflödet.

## Konfigurera aktiviteten Och-join{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Konfigurera aktiviteten AND-join"
>abstract="Välj vilka aktiviteter du vill ansluta till. I listrutan **Primär uppsättning** väljer du vilken ingående övergångspopulation du vill behålla."

Följ de här stegen för att konfigurera aktiviteten **AND-join**:

![](../assets/workflow-andjoin.png)

1. Lägg till flera aktiviteter, till exempel kanalaktiviteter, för att bilda minst två olika utförandegrenar.
1. Lägg till en **AND-join**-aktivitet i någon av grenarna.
1. I avsnittet **Sammanfogningsalternativ** markerar du alla tidigare aktiviteter som du vill ansluta till.
1. I listrutan **Primär uppsättning** väljer du vilken ingående övergångspopulation du vill behålla. Den utgående övergången kan bara innehålla en av de ingående övergångspopulationerna.

## Exempel{#and-join-example}

I följande exempel visas två arbetsflödesgrenar med e-post och SMS-leverans. AND-join utlöses när båda inkommande övergångar är aktiverade. Push-meddelandena skickas sedan först när båda leveranserna är klara.

![](../assets/workflow-andjoin-example.png){zoomable="yes"}
