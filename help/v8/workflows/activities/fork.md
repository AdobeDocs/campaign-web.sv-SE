---
audience: end-user
title: Använda arbetsflödesaktiviteten för gaffel
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
badge: label="Beta"
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 1%

---

# Förgrening {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Gaffelaktivitet"
>abstract="The **Gaffel** kan du skapa utgående övergångar och starta flera aktiviteter samtidigt."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Fork-aktivitetsövergångar"
>abstract="Som standard skapas två övergångar med **Gaffel** aktivitet. Klicka på **Lägg till övergång** för att definiera ytterligare en utgående övergång och ange dess etikett."

The **Gaffel** aktiviteten är en **Flödeskontroll** aktivitet. Det gör att du kan skapa utgående övergångar och starta flera aktiviteter samtidigt.

## Konfigurera gaffelaktiviteten{#fork-configuration}

Följ de här stegen för att konfigurera **Gaffel** aktivitet:

![](../assets/workflow-fork.png)

1. Lägg till en **Gaffel** till ditt arbetsflöde.
1. Klicka **Lägg till övergång** för att lägga till en ny utgående övergång. Som standard definieras två övergångar.
1. Lägg till en etikett till varje övergång.

## Exempel{#fork-example}

I följande exempel använder vi två **Gaffel** verksamhet:

* En före de två frågorna om du vill köra dem samtidigt.
* En efter skärningspunkten, för att skicka ett e-postmeddelande och ett SMS samtidigt till målpopulationen.

![](../assets/workflow-fork-example.png)
