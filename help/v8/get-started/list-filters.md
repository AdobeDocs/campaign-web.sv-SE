---
audience: end-user
title: Bläddra bland, söka i och filtrera listor
description: Upptäck hur du bläddrar bland och filtrerar listor Campaign Web v8
badge: label="Begränsad tillgänglighet"
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: 564524185c6bea11d8159d57ee9c28b47df86f74
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Bläddra bland, söka i och filtrera listor {#list-screens}

De flesta länkar från den vänstra navigeringsmenyn visar listor med objekt, t.ex. listan med **Leveranser** eller **Kampanjer**. Vissa av dessa listskärmar är skrivskyddade. Du kan anpassa listvisningen och filtrera listorna enligt nedan.

Om du vill ta bort ett filter klickar du på **Rensa alla** -knappen.

## Anpassa listskärmar {#custom-lists}

Listorna visas i kolumner. Du kan visa ytterligare information genom att ändra kolumnkonfigurationen. Klicka på **Konfigurera kolumn för en anpassad layout** -ikonen i det övre högra hörnet av listan.

![](assets/config-columns.png){width="70%" align="left" zoomable="yes"}

I **Konfigurera kolumner** rastrera, lägga till eller ta bort kolumner och ändra visningsordningen.

För dessa inställningar:

![](assets/columns.png){width="70%" align="left" zoomable="yes"}

I listan visas följande kolumner:

![](assets/column-sample.png){width="70%" align="left" zoomable="yes"}

## Sortera data {#sort-lists}

Du kan också sortera objekt i listan genom att klicka på en kolumnrubrik. En pil visas (Upp eller Ned) som anger att listan är sorterad i den kolumnen.

För numeriska kolumner och datumkolumner finns **Upp** anger att listan är sorterad i stigande ordning medan **Ned** pil anger en fallande ordning. För strängar eller alfanumeriska kolumner visas värdena i alfabetisk ordning.

## Inbyggda filter {#list-built-in-filters}

Om du vill hitta objekt snabbare kan du använda sökfältet eller filtrera listan baserat på sammanhangsberoende kriterier.

![](assets/filter.png){width="70%" align="left" zoomable="yes"}

Du kan till exempel filtrera leveranser efter status, kanal, kontaktdatum eller mapp. Du kan också dölja tester.

## Egna filter{#list-custom-filters}

Om du vill skapa anpassade filter för data bläddrar du längst ned i filtren och klickar på knappen **Lägg till regler** för att komma åt regelbyggaren.

Definiera och kombinera filtervillkoren i **Avancerade filter** skärm.

![](assets/custom-filter.png){width="70%" align="left" zoomable="yes"}

Anpassade filter har utformats med frågemodelleraren i Campaign. Detaljerad information om hur det används finns i [det här avsnittet](../query/query-modeler-overview.md).

<!--
## Use advanced attributes {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."


Only most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes which were set as `advanced` attributes in the data schema are hidden from the configuration screens. 

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list is updated instantly.


![](assets/adv-toggle.png){width="70%" align="left" zoomable="yes"}
-->