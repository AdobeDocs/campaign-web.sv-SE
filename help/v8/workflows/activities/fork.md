---
audience: end-user
title: Använda arbetsflödesaktiviteten för gaffel
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 2%

---


# Förgrening {#fork}

The **Gaffel** kan du skapa utgående övergångar och starta flera aktiviteter samtidigt.

The **Gaffel** kan du utföra flera olika aktiviteter oberoende av varandra i samma arbetsflöde.

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

