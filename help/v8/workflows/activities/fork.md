---
audience: end-user
title: Använda arbetsflödesaktiviteten för gaffel
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# Förgrening {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Gaffelaktivitet"
>abstract="Med aktiviteten **Förena** kan du skapa utgående övergångar och starta flera aktiviteter samtidigt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Fork-aktivitetsövergångar"
>abstract="Som standard skapas två övergångar med en **Förgrening**-aktivitet. Klicka på knappen **Lägg till övergång** för att definiera ytterligare en utgående övergång och ange dess etikett."

Aktiviteten **Förena** är en **flödeskontroll**-aktivitet. Det gör att du kan skapa utgående övergångar och starta flera aktiviteter samtidigt.

## Konfigurera gaffelaktiviteten {#fork-configuration}

Följ de här stegen för att konfigurera aktiviteten **Förgrening**:

![Konfiguration av aktivitetskonfiguration för arbetsflöde, bild](../assets/workflow-fork.png)

1. Lägg till en **Förgrening**-aktivitet i ditt arbetsflöde.
1. Klicka på **Lägg till övergång** för att lägga till en ny utgående övergång. Som standard definieras två övergångar.
1. Lägg till en etikett till varje övergång.

## Exempel {#fork-example}

I följande exempel används två **gaffelaktiviteter**:

* En före de två frågorna för att köra dem samtidigt.
* En efter skärningspunkten, för att skicka ett e-postmeddelande och ett SMS samtidigt till målpopulationen.

![Exempel på arbetsflödesgaffel, bild](../assets/workflow-fork-example.png)
