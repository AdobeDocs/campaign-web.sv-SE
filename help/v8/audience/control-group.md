---
audience: end-user
title: Ange en kontrollgrupp
description: Lär dig hur du anger en kontrollgrupp för dina meddelanden i användargränssnittet för Campaign-webben
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 4%

---

# Ange en kontrollgrupp {#control-group}

En kontrollgrupp är en underpopulation som är exkluderad från leveransen. Du kan definiera en kontrollgrupp för att undvika att skicka meddelanden till en del av publiken och jämföra postleveransbeteendet med huvudmålet. Med det här alternativet kan ni mäta effekten av er kampanj.

➡️ [Upptäck den här funktionen i videon](create-audience.md#video)

## Aktivera kontrollgrupp {#add-a-control-group}

Om du vill lägga till en kontrollgrupp aktiverar du alternativet när du definierar målgruppen för leveransen. Kontrollgruppen kan extraheras slumpmässigt från huvudmålet eller väljas från en viss population. Det finns alltså två sätt att definiera en kontrollgrupp:

* Extrahera ett antal profiler från huvudmålet.
* Uteslut vissa profiler från en lista eller baserat på villkor som definierats i en fråga.

Du kan kombinera båda metoderna när du definierar en kontrollgrupp.

Alla profiler som ingår i kontrollgruppen vid leveransförberedelsesteget tas bort från huvudmålet. De får inte meddelandet.

>[!CAUTION]
>
>Du kan inte använda kontrollgrupper när målpopulationen [ läses in från en extern fil](file-audience.md).

Om du vill lägga till en kontrollgrupp i en leverans aktiverar du alternativet **[!UICONTROL Enable control group]** i avsnittet **Målgrupp** på skärmen där leveransen skapas.

![Aktivera alternativet för kontrollgrupp för att växla på skärmen för leveransskapande](assets/control-group1.png)

## Extrahera från mål {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extraheringsläge"
>abstract="En kontrollgrupp är en uppsättning profiler som är exkluderade från leveransen. För att definiera en kontrollgrupp kan du välja att extrahera – slumpmässigt eller baserat på en sortering – en procentandel eller ett fast antal profiler från målpopulationen."

### Skapa en kontrollgrupp {#build-extract-target}

Om du vill definiera en kontrollgrupp väljer du att extrahera, slumpmässigt eller baserat på en sortering, en procentandel eller ett fast antal profiler från målpopulationen. Om du lägger till en extra fyllning väljer du alternativet **Ingen extrahering** och väljer den extra fyllningen [som anges här](#extra-population).

Definiera först hur profilerna extraheras från målet: slumpmässigt eller baserat på en sortering.

Under avsnittet **Kontrollgrupp** väljer du ett **extraheringsläge**:

* **Slumpmässig**: När leveransen förbereds extraherar Adobe Campaign slumpmässigt ett antal profiler som motsvarar procentvärdet eller det högsta antal som angetts som storleksgränsen.
* **Rankad efter attribut**: Det här alternativet utesluter en uppsättning profiler baserade på specifika attribut i en viss sorteringsordning.

Använd sedan avsnittet **Storleksgräns** för att ange antalet profiler som ska extraheras från huvudmålet. Det kan vara ett obearbetat tal (till exempel 50 profiler som ska uteslutas) eller en procentandel av den initiala målgruppen (till exempel 5 % av huvudmålet).

### Exempel på kontrollgrupp {#control-group-sample}

Om du till exempel vill skapa en kontrollgrupp med de 100 yngsta profilerna gör du så här:

1. Välj fältet **Ålder** som sorteringsvillkor. Lämna sorteringsalternativet **Stigande**.
1. Lägg till fältet **Skapad**. Ändra till sorteringsalternativet **Fallande**.
1. Definiera 100 som tröskelvärde i avsnittet **Storleksgräns**.

   ![Kontrollgruppskonfiguration för yngsta profiler](assets/control-group2.png){zoomable="yes"}

Dessa 100 yngsta profiler exkluderas sedan från huvudmålet.

### Kontrollera kontrollgruppen {#check-control-group}

Visa loggarna för att kontrollera och identifiera de uteslutna profilerna. Ta till exempel ett slumpmässigt undantag för fem profiler.

![Exempel på uteslutna profiler i loggar](assets/control-group4.png){zoomable="yes"}

Efter leveransberedningen ska du granska hur undantagen tillämpades:

* Kontrollera KPI:n **Att exkludera** innan du skickar den till kontrollpanelen för leverans.

  ![Kontrollpanel för leverans som visar KPI:n för att exkludera ](assets/control-group5.png){zoomable="yes"}

* På fliken Loggar i leveransloggarna visas exkluderingssteget.

  ![Leveransloggar med exkluderingssteg](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* Fliken **Uteslutningsorsaker** visar antalet uteslutna profiler för varje typologiregel.

  ![Fliken Uteslutning orsakar som visar undantag för typologiregler](assets/control-group7.png){zoomable="yes"}

Mer information om leveransloggar finns i [avsnittet](../monitor/delivery-logs.md).

## Lägga till en extra population {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Extra population"
>abstract="En kontrollgrupp är en uppsättning profiler som är exkluderade från leveransen. Du kan utesluta en viss population från leveransgruppen genom att välja en befintlig målgrupp eller genom att definiera en fråga."

Ett annat sätt att definiera en kontrollgrupp är att välja en specifik population i en befintlig målgrupp eller definiera en fråga.

Klicka på knappen **[!UICONTROL Select Audience]** i avsnittet **Extra fyllning** i definitionsskärmen för **kontrollgrupp** .

![Skärm för extra populationsval](assets/control-group3.png){zoomable="yes"}

* Om du vill använda en befintlig målgrupp klickar du på **Välj målgrupp**. Läs mer i [det här avsnittet](add-audience.md).
* Om du vill definiera en ny fråga väljer du **Skapa en egen** och definierar exkluderingsvillkoren med hjälp av frågemodelleraren. Läs mer i [det här avsnittet](../query/query-modeler-overview.md).

Profilerna som ingår i målgruppen eller matchar resultatet av frågan är **exkluderad** från leveransmålet. De får inget meddelande.

## Jämför resultaten {#control-group-results}

När leveransen har skickats kan du extrahera de sändande loggarna för att jämföra beteendet mellan de profiler som inte tog emot kommunikationen och det gällande målet. Använd leveransloggarna för att skapa en ny målinriktning.

Kontrollera **Leveransloggarna** om du vill se vilka profiler som har tagits bort från målet. Läs mer [i det här avsnittet](#check-control-group).