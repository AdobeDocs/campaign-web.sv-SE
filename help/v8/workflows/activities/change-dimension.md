---
audience: end-user
title: Använd aktiviteten Ändra dimensionsarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Ändra dimension
badge: label="Beta"
source-git-commit: fb144e4b7186717dd0c4049d8ce884998a1adefe
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---


# Ändra dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generera ett komplement"
>abstract="Du kan generera ytterligare en utgående övergång med den återstående populationen, som har uteslutits som en dubblett. Aktivera **Generera komplement** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Ändra dimensionsaktivitet"
>abstract="Med den här aktiviteten kan ni ändra målgruppsdimensionen när ni skapar en målgrupp. Axeln flyttas beroende på datamallen och indatamängden. Du kan till exempel växla från dimensionen &quot;kontrakt&quot; till dimensionen &quot;kunder&quot;."

The **Ändra dimension** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan du ändra måldimensionen när du skapar arbetsflödet. Axeln flyttas beroende på datamallen och indatamängden. [Läs mer om målinriktning](../../audience/about-recipients.md#targeting-dimensions)

Du kan till exempel växla ett arbetsflödes målinriktning från&quot;Mottagare&quot; till&quot;Prenumerantprogram&quot; för att skicka push-meddelanden till målmottagarna.

## Konfigurera aktiviteten Ändra dimension {#configure}

Följ de här stegen för att konfigurera **Ändra dimension** aktivitet:

1. Lägg till en **Ändra dimension** till ditt arbetsflöde.

   ![](../assets/workflow-change-dimension.png)

1. Definiera **Ny måldimension**. Vid dimensionsändring sparas alla poster. Andra alternativ är inte tillgängliga än.

1. Kör arbetsflödet för att visa resultatet. Jämför data i tabellerna före och efter ändringsdimensionsaktiviteten och jämför arbetsflödestabellernas struktur.

## Exempel {#example}

I det här exemplet vill vi skicka en SMS-leverans till alla profiler som har gjort ett köp. För att göra detta använder vi först en **[!UICONTROL Build audience]** aktivitet som är länkad till en anpassad målgruppsdimension för inköp för att rikta in alla inköp som har gjorts.

Sedan använder vi en **[!UICONTROL Change dimension]** aktivitet för att ändra arbetsflödets målinriktning till&quot;Mottagare&quot;. På så sätt kan vi rikta in oss på de mottagare som matchar frågan.

![](../assets/workflow-change-dimension-example.png)
