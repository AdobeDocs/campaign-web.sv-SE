---
audience: end-user
title: Använda aktiviteten Kombinera arbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Kombinera
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 6%

---

# Kombinera {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Kombinera aktivitet"
>abstract="Med aktiviteten **Kombinera** kan du utföra segmentering på den inkommande populationen. Du kan kombinera flera populationer, exkludera delar av dem eller bara hålla data gemensamma för flera mål."

Aktiviteten **Kombinera** är en **målaktivitet**. Med den här aktiviteten kan du segmentera den inkommande populationen. Du kan kombinera flera populationer, exkludera delar av dem eller bara hålla data gemensamma för flera mål. Här är de tillgängliga segmenteringstyperna:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* **Union** grupperar resultatet av flera aktiviteter till ett enda mål.
* **Skärningspunkten** behåller bara de element som är gemensamma för de olika inkommande populationerna i aktiviteten.
* **Uteslutning** utesluter element från en population enligt vissa villkor.

## Konfigurera Kombinera-aktiviteten {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Sammanfogningsalternativ för skärningar"
>abstract="Skärningspunkten behåller endast de element som är gemensamma för de olika inkommande populationerna i aktiviteten. Markera alla tidigare aktiviteter som du vill ansluta till i sektionen Uppsättningar att ansluta."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Alternativ för uteslutningssammanslagning"
>abstract="Uteslutningen utesluter element från en population enligt vissa kriterier. Markera alla tidigare aktiviteter som du vill ansluta till i sektionen Uppsättningar att ansluta."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Välj segmenteringstyp"
>abstract="Välj hur målgrupper ska kombineras. **Union** grupperar resultatet av flera aktiviteter till ett enda mål. **Skärningspunkten** behåller bara de element som är gemensamma för de olika inkommande populationerna i aktiviteten. **Uteslutning** utesluter element från en population enligt vissa villkor."

Följ de här vanliga stegen för att konfigurera aktiviteten **Kombinera**:

![](../assets/workflow-combine.png)

1. Lägg till flera aktiviteter, till exempel **Bygg målgruppsaktiviteter**, för att skapa minst två olika körningsgrenar.
1. Lägg till en **Kombinera**-aktivitet i någon av de tidigare grenarna.
1. Välj segmenteringstyp: [union](#union), [skärningspunkt](#intersection) eller [exkludering](#exclusion).
1. Klicka på **Fortsätt**.
1. Markera alla tidigare aktiviteter som du vill ansluta till i avsnittet **Uppsättningar att ansluta till**.

## Sammanslutning {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Avstämningsalternativ"
>abstract="Välj **Avstämningstypen** för att definiera hur dubbletter ska hanteras. Som standard är alternativet **Tangenter** aktiverat, vilket innebär att aktiviteten endast behåller ett element när element från olika inkommande övergångar har samma nyckel. Använd alternativet **Ett urval kolumner** för att definiera listan med kolumner som datavstämningen ska användas på."

Konfigurera en **union** i aktiviteten **Kombinera** genom att välja **avstämningstypen** och definiera hur dubbletter ska hanteras:

* **Endast tangenter**: Det här är standardläget. Aktiviteten behåller endast ett element när element från olika inkommande övergångar har samma nyckel. Detta alternativ kan endast användas om de inkommande populationerna är homogena.
* **Ett urval kolumner**: Välj det här alternativet om du vill definiera listan med kolumner som datavstämningen ska användas på. Markera först den primära uppsättningen (källdata) och sedan de kolumner som ska användas för kopplingen.

## Skärningspunkt {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Avstämningsalternativ för skärningar"
>abstract="Välj **Avstämningstypen** för att definiera hur dubbletter ska hanteras. Som standard är alternativet **Tangenter** aktiverat, vilket innebär att aktiviteten endast behåller ett element när element från olika inkommande övergångar har samma nyckel. Använd alternativet **Ett urval kolumner** för att definiera listan med kolumner som datavstämningen ska användas på."

Konfigurera en **skärningspunkt** genom att följa de här extra stegen i **Kombinera**-aktiviteten:

1. Välj **Avstämningstypen** för att definiera hur dubbletter hanteras. Se avsnittet [Förena](#union).
1. Markera alternativet **Generera komplement** om du vill bearbeta den återstående populationen. Komplementet innehåller en förening av resultaten av alla inkommande aktiviteter minus skärningspunkten. En ytterligare utgående övergång läggs sedan till i aktiviteten.

## Uteslutning {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Uteslutningsregler"
>abstract="Ändra inkommande tabeller när det behövs. Om du vill utesluta ett mål från en annan dimension returnerar du det här målet till samma måldimension som huvudmålet. Klicka på Lägg till en regel i avsnittet Uteslutningsregler och ange villkoren för dimensionsändring. Datavstämning utförs antingen via ett attribut eller en koppling."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Markera uppsättningar som ska kombineras"
>abstract="I avsnittet **Uppsättningar att gå med i** väljer du den **primära uppsättningen** bland de inkommande övergångarna. Detta är den uppsättning från vilken element utesluts. De andra uppsättningarna matchar element innan de utesluts från den primära uppsättningen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="Uteslutningsregler"
>abstract="Ändra inkommande tabeller när det behövs. Om du vill utesluta ett mål från en annan dimension returnerar du det här målet till samma måldimension som huvudmålet. Klicka på Lägg till en regel i avsnittet Uteslutningsregler och ange villkoren för dimensionsändring. Datavstämning utförs antingen via ett attribut eller en koppling."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="Kombinera skapa komplementfärger"
>abstract="Växla till komplementalternativet Generera om du vill bearbeta den återstående populationen i en ytterligare övergång."

I aktiviteten **Kombinera** konfigurerar du ett **undantag** genom att följa de här extra stegen:

1. I avsnittet **Uppsättningar att gå med i** väljer du den **primära uppsättningen** bland de inkommande övergångarna. Detta är den uppsättning från vilken element utesluts. De andra uppsättningarna matchar element innan de utesluts från den primära uppsättningen.
1. Ändra inkommande tabeller när det behövs. Om du vill utesluta ett mål från en annan dimension returnerar du det här målet till samma måldimension som huvudmålet. Klicka på **Lägg till en regel** i avsnittet **Uteslutningsregler** och ange villkoren för dimensionsändring. Datavstämning utförs antingen via ett attribut eller en koppling.
1. Markera alternativet **Generera komplement** om du vill bearbeta den återstående populationen. Se avsnittet [Skärningspunkt](#intersection).

## Exempel {#combine-examples}

I följande exempel använder en **Kombinera**-aktivitet en **union** för att hämta alla profiler för de två frågorna: personer mellan 18 och 27 år och personer mellan 34 och 40 år.

![](../assets/workflow-union-example.png)

I följande exempel visas **Skärningspunkten** mellan två frågeaktiviteter. Den hämtar profiler som är mellan 18 och 27 år gamla och vars e-postadress har angetts.

![](../assets/workflow-intersection-example.png)

I följande exempel på **Uteslutning** visas två frågor som har konfigurerats för att filtrera profiler som är mellan 18 och 27 år gamla och som har en e-postdomän från Adobe. Profilerna med en e-postdomän från Adobe ingår inte i den första uppsättningen.

![](../assets/workflow-exclusion-example.png)