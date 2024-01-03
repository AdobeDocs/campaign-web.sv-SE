---
audience: end-user
title: Filterlistor
description: Lär dig filtrera Adobe Campaign webblistor med inbyggda och anpassade filter.
source-git-commit: 843f3ad906d81892f45281ef5734d512b4c8f3d6
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# Filterlistor {#filter-lists}

Adobe Campaign Web innehåller filter i varje objektlista, vilket gör att du kan filtrera information baserat på specifika kontextuella kriterier. Du kan till exempel filtrera leveranser efter status, kanal, kontaktdatum eller mapp. Du kan också dölja tester.

## Använda filter{#apply}

Om du vill använda filter på en lista klickar du på **[!UICONTROL Show filters]** i det övre vänstra hörnet av listan, bredvid sökfältet.

Filterrutan öppnas och tillgängliga filter för den valda listan visas. Du kan t.ex. filtrera kampanjer efter status, start- och slutdatum eller lagringsmapp, medan prenumerationstjänstlistan kan filtreras i kanal- och lagringsmappen.

![](assets/filters-pane.png){width="70%" align="left" zoomable="yes"}

Om du vill filtrera en lista baserat på dina egna kriterier skapar du ett eget filter. Om du vill göra det bläddrar du längst ned i filterrutan och klickar på **Lägg till regler** -knappen. [Lär dig hur du skapar anpassade filter](#custom)

När filtren har tillämpats på en lista visas de under sökfältet. Du kan ta bort ett enskilt filter när som helst eller ta bort alla filter genom att klicka på **Rensa alla** -knappen.

## Skapa egna filter {#custom}

Med anpassade filter kan du förfina listor baserat på dina egna specifika villkor. De är utformade med frågemodelleraren i Campaign. Så här skapar du ett eget filter:

1. Öppna filterrutan och klicka på **Lägg till regler** längst ned i rutan.
1. Frågemodelleraren öppnas. Definiera och kombinera filtervillkor efter behov. Detaljerad information om hur du använder frågemodelleraren finns i [det här avsnittet](../query/query-modeler-overview.md).

   I exemplet nedan visas ett anpassat filter som är utformat för att i kampanjlistan visa SMS-kampanjer som körs av operatorer från avdelningarna Running och Yoga.

   ![](assets/filters-sample.png){width="70%" align="left" zoomable="yes"}

1. När det anpassade filtret har konfigurerats klickar du på **[!UICONTROL Confirm]** för att tillämpa den på listan.
