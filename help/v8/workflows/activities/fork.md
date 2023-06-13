---
audience: end-user
title: Använda arbetsflödesaktiviteten för gaffel
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 18%

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

