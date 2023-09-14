---
audience: end-user
title: Använd aktiviteten Ändra dimensionsarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Ändra dimension
badge: label="Beta"
source-git-commit: ea57053910aa98e79ceb7ef683f890a366a9001b
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 2%

---


# Ändra dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Ändra dimensionsaktivitet"
>abstract="Med aktiviteten Ändra dimension kan du.."

The **Ändra dimension** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan ni ändra målgruppsdimensionen när ni skapar en målgrupp. Den här aktiviteten flyttar axeln beroende på datamallen och indatatypen. Du kan till exempel växla från dimensionen &quot;kontrakt&quot; till dimensionen &quot;kunder&quot;.

Du kan också använda den här aktiviteten för att definiera ytterligare kolumner för det nya målet och definiera villkor för datadeduplicering.

## Konfiguration

Följ de här stegen för att konfigurera **Ändra dimension** aktivitet:

1. Lägg till en **Ändra dimension** till ditt arbetsflöde.

       ![](../assets/workflow-change-dimension.png)
   
1. Välj den nya måldimensionen via fältet Ändra dimension.

Ingenting annat?