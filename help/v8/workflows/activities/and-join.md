---
audience: end-user
title: Använda arbetsflödesaktiviteten AND-join
description: Lär dig använda arbetsflödesaktiviteten OCH-join
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# AND-join {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join activity"
>abstract="Med aktiviteten **And-join** kan du synkronisera flera körningsgrenar i ett arbetsflöde. Den aktiveras när alla föregående aktiviteter har slutförts. Detta garanterar att vissa aktiviteter slutförs innan arbetsflödet fortsätter."

Aktiviteten **And-join** är en **Flow control** -aktivitet. Den synkroniserar flera körningsgrenar i ett arbetsflöde.

Den här aktiviteten utlöser sin utgående övergång först när alla inkommande övergångar har aktiverats. Med andra ord aktiveras den när alla föregående aktiviteter har slutförts. Detta garanterar att vissa aktiviteter är slutförda innan du fortsätter att köra arbetsflödet.

## Konfigurera aktiviteten Och-join {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Sammanfogningsalternativ"
>abstract="Välj vilka aktiviteter du vill ansluta till. I listrutan **Primär uppsättning** väljer du vilken ingående övergångspopulation du vill behålla."

Följ de här stegen för att konfigurera aktiviteten **AND-join**:

![Skärmbild som visar konfigurationsgränssnittet för AND-join-aktiviteten.](../assets/workflow-andjoin.png)

1. Lägg till flera aktiviteter, till exempel kanalaktiviteter, för att bilda minst två olika körningsgrenar.
1. Lägg till en **AND-join**-aktivitet i någon av grenarna.
1. I avsnittet **Sammanfogningsalternativ** markerar du alla tidigare aktiviteter som du vill ansluta till.
1. I listrutan **Primär uppsättning** väljer du vilken inkommande övergångspopulation som ska behållas. Den utgående övergången kan bara innehålla en av de ingående övergångspopulationerna.

## Exempel {#and-join-example}

I följande exempel visas två arbetsflödesgrenar med e-post och SMS-leverans. AND-join-utlösarna när båda inkommande övergångar är aktiverade. Push-meddelanden skickas endast när båda leveranserna har slutförts.

![Exempel på ett arbetsflöde med två grenar som visar e-post och SMS-leverans följt av push-meddelanden.](../assets/workflow-andjoin-example.png){zoomable="yes"}