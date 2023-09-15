---
audience: end-user
title: Använd aktiviteten Vänta i arbetsflödet
description: Lär dig hur du använder aktiviteten Vänta i arbetsflödet
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 25%

---


# Vänta {#wait}


>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Vänta"
>abstract="The **Vänta** aktiviteten är en **Flödeskontroll** aktivitet. Det används för att en viss tid ska kunna förflyta mellan två aktiviteter som utförs."


The **Vänta** aktiviteten är en **Flödeskontroll** aktivitet. Det används för att en viss tid ska kunna förflyta mellan två aktiviteter som utförs. Om du till exempel vill vänta flera dagar efter en aktivitet där e-post levererats så analyserar du de öppningar och klick som genereras under den här perioden innan du utför några uppföljningsåtgärder (påminnelser via e-post, målgruppsgenerering osv.).

## Konfiguration

Följ de här stegen för att konfigurera **Vänta** aktivitet:

1. Lägg till en **Vänta** i arbetsflödet.

1. Ange **Varaktighet** av väntetiden mellan inkommande och utgående övergångar.

1. Välj tidsenhet i dialogrutan **Perioder** fält: sekunder, minuter, timmar.

## Exempel

I följande exempel visas **Vänta** i vanliga fall. En e-postinbjudan till ett event skickas.  24 timmar efter att det skickats skickas ett SMS-meddelande till samma population.

![](../assets/workflow-wait-example.png)
