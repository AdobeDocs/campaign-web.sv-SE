---
audience: end-user
title: Använda aktiviteten Testa arbetsflöde
description: Lär dig hur du använder aktiviteten Testa arbetsflöde
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---


# Test {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="Testaktivitet"
>abstract="Aktiviteten **Test** är en **Flödeskontroll**-aktivitet. Det gör att du kan aktivera övergångar baserat på angivna villkor."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="Villkor"
>abstract="Aktiviteten **Test** kan ha flera utdataövergångar. Under arbetsflödeskörningen testas varje villkor sekventiellt tills ett av dem uppfylls. Om inga villkor uppfylls fortsätter arbetsflödet längs sökvägen för **[!UICONTROL Default condition]**. Om inget standardvillkor aktiveras stoppas arbetsflödet nu."

Aktiviteten **Test** är en **Flödeskontroll**-aktivitet. Det gör att du kan aktivera övergångar baserat på angivna villkor.

## Konfigurera aktiviteten Testa {#test-configuration}

Följ de här stegen för att konfigurera aktiviteten **Test**:

1. Lägg till en **Test**-aktivitet i arbetsflödet.

1. Som standard visar aktiviteten **[!UICONTROL Test]** ett enkelt booleskt test. Om villkoret som definieras i övergången &quot;Sant&quot; är uppfyllt aktiveras den här övergången. I annat fall aktiveras standardövergången&quot;Falskt&quot;.

1. Klicka på ikonen **[!UICONTROL Open personalization dialog]** om du vill konfigurera villkoret som är kopplat till en övergång. Använd uttrycksredigeraren för att definiera de regler som krävs för att aktivera den här övergången. Du kan också använda händelsevariabler, villkor och datum/tid-funktioner. [Lär dig hur du arbetar med händelsevariabler och uttrycksredigeraren](../event-variables.md).

   Ändra dessutom fältet **[!UICONTROL Label]** för att anpassa övergångens namn på arbetsytan.

   ![Standardkonfiguration för testaktiviteten](../assets/workflow-test-default.png)

1. Lägg till flera utdataövergångar i en **[!UICONTROL Test]**-aktivitet. Det gör du genom att klicka på knappen **[!UICONTROL Add condition]** och konfigurera etiketten och tillhörande villkor för varje övergång.

1. Under arbetsflödeskörningen testas varje villkor sekventiellt tills ett av dem uppfylls. Om inga villkor uppfylls fortsätter arbetsflödet längs sökvägen för **[!UICONTROL Default condition]**. Om inget standardvillkor aktiveras stoppas arbetsflödet nu.

## Exempel {#example}

I det här exemplet aktiveras olika övergångar baserat på antalet profiler som en **[!UICONTROL Build audience]**-aktivitet har som mål:
* Om fler än 10 000 profiler används skickas ett e-postmeddelande.
* För 1 000 till 10 000 profiler skickas ett SMS.
* Om målprofilerna ligger under 1 000 dirigeras de till en&quot;inte kontakt&quot;-övergång.

![Exempel på testaktivitetsövergångar](../assets/workflow-test-example.png)

För att uppnå detta används händelsevariabeln `vars.recCount` i villkoren för e-post och sms för att räkna antalet målprofiler och aktivera lämplig övergång.

![Konfiguration av Exempel på testaktivitet](../assets/workflow-test-example-config.png)
