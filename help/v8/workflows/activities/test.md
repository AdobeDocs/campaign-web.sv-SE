---
audience: end-user
title: Använda aktiviteten Testa arbetsflöde
description: Lär dig hur du använder aktiviteten Testa arbetsflöde
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Test {#test}

The **Testa** aktiviteten är en **Flödeskontroll** aktivitet. Det gör att du kan aktivera övergångar baserat på angivna villkor.

## Konfigurera aktiviteten Testa {#test-configuration}

Följ de här stegen för att konfigurera **Testa** aktivitet:

1. Lägg till en **Testa** till ditt arbetsflöde.

1. Som standard är **[!UICONTROL Test]** aktiviteten utgör ett enkelt booleskt test. Om villkoret som definieras i övergången &quot;Sant&quot; är uppfyllt aktiveras den här övergången. Annars aktiveras standardövergången &quot;Falskt&quot;.

1. Om du vill konfigurera villkoret för en övergång klickar du på **[!UICONTROL Open personalization dialog]** -ikon. Använd uttrycksredigeraren för att definiera de regler som krävs för att aktivera den här övergången. Du kan också utnyttja händelsevariabler, villkor och datum/tid-funktioner. [Lär dig hur du arbetar med händelsevariabler och uttrycksredigeraren](../event-variables.md)

   Dessutom kan du ändra **[!UICONTROL Label]** om du vill anpassa övergångens namn på arbetsytan.

   ![](../assets/workflow-test-default.png)

1. Du kan lägga till flera utdataövergångar i en **[!UICONTROL Test]** aktivitet. Klicka på **[!UICONTROL Add condition]** och konfigurera etiketten och tillhörande villkor för varje övergång.

1. Under arbetsflödeskörningen testas varje villkor sekventiellt tills ett av dem uppfylls. Om inga villkor uppfylls fortsätter arbetsflödet längs sökvägen till **[!UICONTROL Default condition]**. Om inget standardvillkor är aktiverat stoppas arbetsflödena nu.

## Exempel {#example}

I det här exemplet aktiveras olika övergångar baserat på antalet profiler som en **[!UICONTROL Build audience]** aktivitet:
* Om fler än 10 000 profiler används skickas ett e-postmeddelande.
* För 1 000 till 10 000 profiler skickas ett SMS.
* Om målprofilerna ligger under 1 000 dirigeras de till en&quot;inte kontakt&quot;-övergång.

![](../assets/workflow-test-example.png)

För att göra detta `vars.recCount` händelsevariabeln har utnyttjats i villkoren&quot;email&quot; och&quot;sms&quot; för att räkna antalet målprofiler och aktivera lämplig övergång.

![](../assets/workflow-test-example-config.png)
