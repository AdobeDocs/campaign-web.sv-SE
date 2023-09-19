---
audience: end-user
title: Använd aktiviteten Ändra dimensionsarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Ändra dimension
badge: label="Beta"
source-git-commit: 8139ec2f1e94bebacd89ea64af88d0b0babb8781
workflow-type: tm+mt
source-wordcount: '210'
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

The **Ändra dimension** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan ni ändra målgruppsdimensionen när ni skapar en målgrupp. Den här aktiviteten flyttar axeln beroende på datamallen och indatatypen. Du kan till exempel växla från dimensionen &quot;kontrakt&quot; till dimensionen &quot;kunder&quot;.

## Konfigurera aktiviteten Ändra dimension {#configure}

Följ de här stegen för att konfigurera **Ändra dimension** aktivitet:

1. Lägg till en **Ändra dimension** till ditt arbetsflöde.

   ![](../assets/workflow-change-dimension.png)

1. Definiera **Ny måldimension**. Vid dimensionsändring sparas alla poster. Andra alternativ är inte tillgängliga än.

1. Kör arbetsflödet för att visa resultatet. Jämför data i tabellerna före och efter ändringsdimensionsaktiviteten och jämför arbetsflödestabellernas struktur.

## Exempel {#example}


