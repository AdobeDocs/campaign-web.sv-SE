---
audience: end-user
title: Använda arbetsflödesaktiviteten för gaffel
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
badge: label="Alpha" type="Positive"
source-git-commit: 1ac80ffaabea210bbc02588475ad6e81af4820b1
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 17%

---


# Förgrening {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Gaffelaktivitet"
>abstract="Med förgreningsaktiviteten kan du skapa utgående övergångar och starta flera aktiviteter samtidigt."

## Konfiguration

Följ de här stegen för att konfigurera **Gaffel** aktivitet:

1. Lägg till en **Gaffel** till arbetsflödet.
1. Klicka **Lägg till övergång** för att lägga till en ny utgående övergång. Som standard definieras två övergångar.
1. Lägg till en etikett till varje övergång.

## Exempel

I följande exempel använder vi två **Gaffel** verksamhet:

* En före de två frågorna om du vill köra dem samtidigt.
* En efter skärningspunkten, för att skicka ett e-postmeddelande och ett SMS samtidigt till målpopulationen.

![](../assets/workflow-fork-example.png)

