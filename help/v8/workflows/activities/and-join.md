---
audience: end-user
title: Använda arbetsflödesaktiviteten AND-join
description: Lär dig hur du använder arbetsflödesaktiviteten OCH-join
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 1%

---


# AND-join {#join}

The **Och-join** aktiviteten är en **Flödeskontroll** aktivitet. Det gör att du kan synkronisera flera körningsgrenar i ett arbetsflöde.

Den här aktiviteten utlöser endast den utgående övergången när alla inkommande övergångar har aktiverats, det vill säga när alla föregående aktiviteter har slutförts. På så sätt kan du se till att vissa aktiviteter har slutförts innan du fortsätter att köra arbetsflödet.

## Konfiguration

Följ de här stegen för att konfigurera **AND-join** aktivitet:

1. Lägg till flera aktiviteter, t.ex. kanalaktiviteter, för att bilda minst två olika utförandegrenar.
1. Lägg till en **AND-join** till någon av grenarna.
1. I **Sammanfogningsalternativ** markerar du alla tidigare aktiviteter du vill delta i.
1. I **Primär uppsättning** väljer du vilken inkommande övergångspopulation som du vill behålla. Den utgående övergången kan bara innehålla en av de ingående övergångspopulationerna.

## Exempel

I följande exempel visas två arbetsflödesgrenar med e-post och SMS-leverans. AND-join utlöses när båda inkommande övergångar är aktiverade. Push-meddelandena skickas sedan först när båda leveranserna är klara.

![](../assets/workflow-andjoin-example.png)