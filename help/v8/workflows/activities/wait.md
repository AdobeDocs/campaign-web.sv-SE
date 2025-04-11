---
audience: end-user
title: Använd aktiviteten Vänta i arbetsflödet
description: Lär dig hur du använder aktiviteten Vänta i arbetsflödet
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 6%

---

# Vänta {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Vänta på aktivitet"
>abstract="Aktiviteten **Wait** används för att fördröja övergången från en aktivitet till en annan."

Aktiviteten **Wait** är en **Flow control**-aktivitet. Det ger en viss tid att förflyta mellan utförandet av två aktiviteter. Den kan till exempel användas för att vänta flera dagar efter en e-postleveransaktivitet och sedan analysera de öppningar och klickningar som genereras under perioden innan du utför uppföljningsåtgärder, som att skicka ett påminnelsemeddelande eller skapa en målgrupp.

## Konfiguration {#wait-configuration}

Följ de här stegen för att konfigurera aktiviteten **Wait**:

1. Lägg till en **Vänta**-aktivitet i arbetsflödet.

1. Ange **Varaktighet** för väntetiden mellan inkommande och utgående övergångar.

1. Välj tidsenhet i fältet **Perioder**: sekunder, minuter, timmar eller dagar.

## Exempel {#wait-example}

I följande exempel visas aktiviteten **Wait** i ett typiskt fall. En e-postinbjudan till ett event skickas.  Efter 24 timmar skickas en SMS-leverans till samma population.

![Exempel på ett arbetsflöde som använder aktiviteten Vänta för att skicka ett SMS 24 timmar efter en e-postinbjudan.](../assets/workflow-wait-example.png)