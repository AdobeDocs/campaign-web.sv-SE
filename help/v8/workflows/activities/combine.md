---
audience: end-user
title: Använda aktiviteten Kombinera arbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Kombinera
badge: label="Alpha" type="Positive"
source-git-commit: 3bbdd45571d09258bba34e22de39f5281c02d248
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 16%

---


# Kombinera {#combine}

Med den här aktiviteten kan du bearbeta uppsättningar på inkommande data. Du kan alltså kombinera flera populationer, utesluta en del av dem eller bara behålla data som är gemensamma för flera mål. Här är de tillgängliga segmenteringstyperna:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* The **Union** kan du gruppera om resultatet av flera aktiviteter till ett enda mål.
* The **Skärningspunkt** gör att du bara kan behålla de element som är gemensamma för de olika inkommande populationerna i aktiviteten.
* The **Uteslutning** gör att du kan utesluta element från en population enligt vissa kriterier.

## Konfiguration

Följ de här stegen för att konfigurera **Kombinera** aktivitet:

1. Lägg till flera aktiviteter som **Bygg målgrupper** aktiviteter för att bilda minst två olika utförandegrenar.
1. Lägg till en **Kombinera** aktivitet till någon av de tidigare segmenteringsövergångarna.
1. Välj segmenteringstyp: union, skärning eller uteslutning.
1. Klicka **Fortsätt**.
1. I **Uppsättningar att förena** markerar du alla tidigare aktiviteter du vill delta i.

För **Union** och **Skärningspunkt** måste du välja **Avstämningstyp** för att definiera hur dubbletter hanteras:

    * Endast tangenter: det här är standardläget. Aktiviteten behåller endast ett element när element från olika inkommande övergångar har samma nyckel.  Detta alternativ kan endast användas om de inkommande populationerna är homogena.
    * En markering med kolumner: Välj det här alternativet om du vill definiera listan med kolumner som datavstämningen ska tillämpas på. Du måste först markera den primära uppsättningen (som innehåller källdata) och sedan de kolumner som ska användas för kopplingen.

För **Skärningspunkt** och **Uteslutning** kan du kontrollera **Generera slutförande** om du vill bearbeta den återstående populationen. Komplementet ska innehålla en kombination av resultaten av alla inkommande aktiviteter minus skärningspunkten. En ytterligare utgående övergång läggs sedan till i aktiviteten.

För **Uteslutning** väljer du **Primär uppsättning** från inkommande övergångar, i **Uppsättningar att förena** -avsnitt. Detta är den uppsättning från vilken element utesluts. De andra uppsättningarna matchar element innan de utesluts från den primära uppsättningen.

## Exempel

I följande exempel har vi lagt till en **union** som hämtar alla profiler för de två frågorna: personer mellan 18 och 27 år och personer mellan 34 och 40 år.

![](../assets/workflow-union-example.png)

I följande exempel visas **skärningspunkt** mellan två frågeaktiviteter. Den används här för att hämta profiler som är mellan 18 och 27 år gamla och vars e-postadress har angetts.

![](../assets/workflow-intersection-example.png)

Följande **exkludering** I exemplet visas två frågor som har konfigurerats för att filtrera profiler som är mellan 18 och 27 år gamla och som har en e-postdomän från Adobe. Profilerna med en Adobe e-postdomän exkluderas sedan från den första uppsättningen.

![](../assets/workflow-exclusion-example.png)





