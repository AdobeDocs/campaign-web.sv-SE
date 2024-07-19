---
audience: end-user
title: Använda aktiviteten Testa arbetsflöde
description: Lär dig hur du använder aktiviteten Testa arbetsflöde
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Test {#test}

Aktiviteten **Test** är en **Flödeskontroll**-aktivitet. Det gör att du kan aktivera övergångar baserat på angivna villkor.

## Konfigurera aktiviteten Testa {#test-configuration}

Följ de här stegen för att konfigurera aktiviteten **Test**:

1. Lägg till en **Test**-aktivitet i arbetsflödet.

1. Som standard visar aktiviteten **[!UICONTROL Test]** ett enkelt booleskt test. Om villkoret som definieras i övergången &quot;Sant&quot; är uppfyllt aktiveras den här övergången. Annars aktiveras standardövergången &quot;Falskt&quot;.

1. Klicka på ikonen **[!UICONTROL Open personalization dialog]** om du vill konfigurera villkoret som är kopplat till en övergång. Använd uttrycksredigeraren för att definiera de regler som krävs för att aktivera den här övergången. Du kan också utnyttja händelsevariabler, villkor och datum/tid-funktioner. [Lär dig hur du arbetar med händelsevariabler och uttrycksredigeraren](../event-variables.md)

   Du kan dessutom ändra fältet **[!UICONTROL Label]** för att anpassa övergångens namn på arbetsytan.

   ![](../assets/workflow-test-default.png)

1. Du kan lägga till flera utdataövergångar i en **[!UICONTROL Test]**-aktivitet. Det gör du genom att klicka på knappen **[!UICONTROL Add condition]** och konfigurera etiketten och tillhörande villkor för varje övergång.

1. Under arbetsflödeskörningen testas varje villkor sekventiellt tills ett av dem uppfylls. Om inga villkor uppfylls fortsätter arbetsflödet längs sökvägen för **[!UICONTROL Default condition]**. Om inget standardvillkor är aktiverat stoppas arbetsflödena nu.

## Exempel {#example}

I det här exemplet aktiveras olika övergångar baserat på antalet profiler som en **[!UICONTROL Build audience]**-aktivitet har som mål:
* Om fler än 10 000 profiler används skickas ett e-postmeddelande.
* För 1 000 till 10 000 profiler skickas ett SMS.
* Om målprofilerna ligger under 1 000 dirigeras de till en&quot;inte kontakt&quot;-övergång.

![](../assets/workflow-test-example.png)

För att göra detta har händelsevariabeln `vars.recCount` utnyttjats i villkoren för e-post och sms för att räkna antalet målprofiler och aktivera lämplig övergång.

![](../assets/workflow-test-example-config.png)
