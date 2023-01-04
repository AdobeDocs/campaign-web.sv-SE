---
audience: end-user
title: Ange en kontrollgrupp
description: Webbdokumentation för Campaign v8
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: bc076bb4c841dd8e259ac007ecef8e3cb496a08d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Ange en kontrollgrupp {#control-group}

>[!NOTE]
>
>Dokumentationen håller på att byggas och uppdateras ofta. Den slutliga versionen av detta innehåll är klar i januari 2023.

Du kan använda kontrollgrupper för att undvika att skicka meddelanden till en del av målgruppen för att kunna mäta effekten av kampanjerna.

Det gör du genom att skapa en kontrollgrupp när du definierar målgruppen för leveransen. Profiler läggs slumpmässigt till i kontrollgruppen, filtrerade eller inte, eller baserat på kriterier. Sedan kan du jämföra beteendet hos målpopulationen som fick meddelandet med beteendet hos kontakter som inte var med i målgrupperna.

Kontrollgruppen kan extraheras slumpmässigt från huvudmålet och/eller väljas från en viss målgrupp. Det finns därför två sätt att definiera en kontrollgrupp:

* Extrahera ett antal profiler från huvudmålet.
* Uteslut vissa profiler baserat på villkor som definierats i en fråga.

Du kan använda båda metoderna för att definiera en kontrollgrupp.

Alla profiler som är en del av kontrollgruppen vid leveransens förberedelsesteg tas bort från huvudmålet. De får inte meddelandet när det har skickats.

Om du vill skapa en kontrollgrupp klickar du på **[!UICONTROL Set Control Group]** från **Målgrupp** i leveransassistenten.

![](assets/control-group1.png)

## Extrahera från mål {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extrahera från mål"
>abstract="TBC"

För att definiera en kontrollgrupp kan du välja att extrahera – slumpmässigt eller baserat på en sortering – en procentandel eller ett fast antal profiler från målpopulationen.

Definiera först hur profilerna ska extraheras från målet: slumpmässigt eller baserat på en sortering.

Under **Extrahera från mål** väljer du ett **Uteslutningstyp**:

* **Slumpmässig**: När leveransen förbereds extraherar Adobe Campaign slumpmässigt ett antal profiler som motsvarar procentandelen eller det högsta antal som du anger som storleksgräns.

   ![](assets/control-group.png)

* **Rankad efter attribut**: Med det här alternativet kan du definiera en begränsning baserat på en eller flera sorteringsordningar.

   ![](assets/control-group2.png)

Definiera sedan **Storleksgräns**: du måste ange hur du ska begränsa antalet profiler som du extraherar från huvudmålet.

## Extra population {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Extra population"
>abstract="TBC"

Ett annat sätt att definiera en kontrollgrupp är att utesluta en viss population från målet med hjälp av en befintlig målgrupp eller genom att definiera en fråga.

Från **Extra population** i **Kontrollgrupp** definitionsskärmen klickar du på **[!UICONTROL Select Audience]** -knappen.

![](assets/control-group3.png)

* Om du vill använda en befintlig målgrupp klickar du på **Välj målgrupp**. Se detta [section](add-audience.md).

* Om du vill definiera en ny fråga väljer du **Skapa en egen** och definiera uteslutningskriterierna med segmentbyggaren. Se detta [section](segment-builder.md).

Profilerna som ingår i målgruppen eller som matchar resultatet av frågan kommer att uteslutas från målet.