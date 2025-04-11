---
audience: end-user
title: Använd aktiviteten Ändra dimensionsarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Ändra dimension
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Ändra dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generera ett komplement"
>abstract="Du kan generera ytterligare en utgående övergång med den återstående populationen, som har uteslutits som en dubblett. Aktivera alternativet **Generera komplement** om du vill göra det."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Ändra dimensionsaktivitet"
>abstract="Med den här aktiviteten kan ni ändra målgruppsdimensionen när ni skapar en målgrupp. Axeln flyttas beroende på datamallen och indatamängden. Du kan till exempel växla från dimensionen&quot;kontrakt&quot; till dimensionen&quot;kunder&quot;."

Aktiviteten **Ändra dimension** är en **målaktivitet**. Med den här aktiviteten kan du ändra måldimensionen när du skapar arbetsflödet. Axeln flyttas beroende på datamallen och indatamängden. [Läs mer om måldimensioner](../../audience/about-recipients.md#targeting-dimensions).

Du kan till exempel växla ett arbetsflödes målinriktning från&quot;Mottagare&quot; till&quot;Prenumerantprogram&quot; för att skicka push-meddelanden till målmottagarna.

>[!IMPORTANT]
>
>Observera att aktiviteterna **[!UICONTROL Change Dimension]** och **[!UICONTROL Change Data source]** inte ska läggas till på en rad. Om du behöver använda båda aktiviteterna i följd inkluderar du en **[!UICONTROL Enrichment]**-aktivitet mellan dem. Detta garanterar att programmet körs på rätt sätt och förhindrar eventuella konflikter och fel.

## Konfigurera aktiviteten Ändra dimension {#configure}

Följ de här stegen för att konfigurera aktiviteten **Ändra dimension**:

1. Lägg till en **Ändra dimension**-aktivitet i arbetsflödet.

   ![Skärmbild som visar aktiviteten Ändra dimension som har lagts till i ett arbetsflöde](../assets/workflow-change-dimension.png)

1. Definiera den **nya måldimensionen**. Vid dimensionsändring sparas alla poster. Andra alternativ är inte tillgängliga än.

1. Kör arbetsflödet för att visa resultatet. Jämför data i tabellerna före och efter aktiviteten Ändra dimension och jämför arbetsflödestabellernas struktur.

## Exempel {#example}

I det här exemplet skickar du en SMS-leverans till alla profiler som har gjort ett köp. Använd först en **[!UICONTROL Build audience]**-aktivitet som är länkad till en anpassad målinriktningsdimension för inköp för att rikta alla inköp som har gjorts.

Använd sedan en **[!UICONTROL Change dimension]**-aktivitet för att växla arbetsflödets måldimension till&quot;Mottagare&quot;. Detta gör att det går att rikta in mottagarna som matchar frågan.

![Skärmbild som visar ett exempel på aktiviteten Ändra dimension som används i ett arbetsflöde](../assets/workflow-change-dimension-example.png)