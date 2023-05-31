---
audience: end-user
title: Använda aktiviteten Kombinera arbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Kombinera
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 21%

---


# Kombinera {#combine}

Med den här aktiviteten kan du bearbeta uppsättningar på inkommande data. Du kan alltså kombinera flera populationer, utesluta en del av dem eller bara behålla data som är gemensamma för flera mål. Här är de tillgängliga segmenteringstyperna:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* The **Union** kan du gruppera om resultatet av flera aktiviteter till ett enda mål.
* The **Skärningspunkt** gör att du bara kan behålla de element som är gemensamma för de olika inkommande populationerna i aktiviteten.
* The **Uteslutning** gör att du kan utesluta element från en population enligt vissa kriterier.

Följ de här stegen för att konfigurera **Kombinera** aktivitet:

1. Lägg till **Kombinera** aktivitet till någon av de tidigare segmenteringsövergångarna.
1. Välj segmenteringstyp: union, skärning eller uteslutning.
1. Klicka **Fortsätt**.
1. I **Uppsättningar att förena** markerar du alla tidigare aktiviteter du vill delta i.

För **Union** och **Skärningspunkt** måste du välja **Avstämningstyp** för att definiera hur dubbletter hanteras:

    * Endast tangenter: det här är standardläget. Aktiviteten behåller endast ett element när element från olika inkommande övergångar har samma nyckel.  Detta alternativ kan endast användas om de inkommande populationerna är homogena.
    * En markering med kolumner: Välj det här alternativet om du vill definiera listan med kolumner som datavstämningen ska tillämpas på. Du måste först markera den primära uppsättningen (som innehåller källdata) och sedan de kolumner som ska användas för kopplingen.

För **Skärningspunkt** och **Uteslutning** kan du kontrollera **Generera slutförande** om du vill bearbeta den återstående populationen. Komplementet ska innehålla en kombination av resultaten av alla inkommande aktiviteter minus skärningspunkten. En ytterligare utgående övergång läggs sedan till i aktiviteten.

För **Uteslutning** väljer du **Primär uppsättning** från inkommande övergångar, i **Uppsättningar att förena** -avsnitt. Detta är den uppsättning från vilken element utesluts. De andra uppsättningarna matchar element innan de utesluts från den primära uppsättningen.
