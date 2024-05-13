---
audience: end-user
title: Använd aktiviteten Ändra dimensionsarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Ändra dimension
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: 99bdd5220cceb4ab67c3bd4e3a788a28cbe40f8f
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

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

>[!IMPORTANT]
>
>Observera att **[!UICONTROL Change Dimension]** och **[!UICONTROL Change Data source]** aktiviteter ska inte läggas till på en rad. Om du behöver använda båda aktiviteterna i följd måste du inkludera en **[!UICONTROOL Berikning]** mellan dem. Detta garanterar att programmet körs på rätt sätt och förhindrar eventuella konflikter och fel.

## Konfigurera aktiviteten Ändra dimension {#configure}

Följ de här stegen för att konfigurera **Ändra dimension** aktivitet:

1. Lägg till en **Ändra dimension** till ditt arbetsflöde.

   ![](../assets/workflow-change-dimension.png)

1. Definiera **Ny måldimension**. Vid dimensionsändring sparas alla poster. Andra alternativ är inte tillgängliga än.

1. Kör arbetsflödet för att visa resultatet. Jämför data i tabellerna före och efter ändringsdimensionsaktiviteten och jämför arbetsflödestabellernas struktur.

## Exempel {#example}

I det här exemplet vill vi skicka en SMS-leverans till alla profiler som har gjort ett köp. För att göra detta använder vi först en **[!UICONTROL Build audience]** aktivitet som är länkad till en anpassad målgruppsdimension&quot;Inköp&quot; för att rikta sig till alla inköp som har gjorts.

Sedan använder vi en **[!UICONTROL Change dimension]** aktivitet för att ändra arbetsflödets målinriktning till&quot;Mottagare&quot;. På så sätt kan vi rikta in oss på de mottagare som matchar frågan.

![](../assets/workflow-change-dimension-example.png)
