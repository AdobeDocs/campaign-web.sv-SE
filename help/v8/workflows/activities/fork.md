---
audience: end-user
title: Använda arbetsflödesaktiviteten för gaffel
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 12%

---


# Förgrening {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Gaffelaktivitet"
>abstract="The **Gaffel** aktiviteten är en **Flödeskontroll** aktivitet. Det gör att du kan skapa utgående övergångar och starta flera aktiviteter samtidigt."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Gaffelaktivitet"
>abstract="Med förgreningsaktiviteten kan du skapa utgående övergångar och starta flera aktiviteter samtidigt."

The **Gaffel** aktiviteten är en **Flödeskontroll** aktivitet. Det gör att du kan skapa utgående övergångar och starta flera aktiviteter samtidigt.

## Konfiguration

Följ de här stegen för att konfigurera **Gaffel** aktivitet:

1. Lägg till en **Gaffel** till ditt arbetsflöde.
1. Klicka **Lägg till övergång** för att lägga till en ny utgående övergång. Som standard definieras två övergångar.
1. Lägg till en etikett till varje övergång.

## Exempel

I följande exempel använder vi två **Gaffel** verksamhet:

* En före de två frågorna om du vill köra dem samtidigt.
* En efter skärningspunkten, för att skicka ett e-postmeddelande och ett SMS samtidigt till målpopulationen.

![](../assets/workflow-fork-example.png)

