---
audience: end-user
title: Bläddra bland, söka i och filtrera listor
description: Upptäck hur du bläddrar bland och filtrerar listor Campaign Web v8
badge: label="Alpha" type="Positive"
source-git-commit: 9f9cb4423d098ae57f429fb2a49e335d413399c1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 1%

---


# Bläddra bland, söka i och filtrera listor {#list-screens}

De flesta länkar från den vänstra navigeringsmenyn visar listor med objekt, t.ex. listan med **Leveranser** eller **Kampanjer**. Vissa av dessa listskärmar är skrivskyddade. Du kan anpassa listvisningen och filtrera listorna enligt nedan.

Om du vill ta bort ett filter klickar du på **Rensa alla** -knappen.

## Anpassa listskärmar {#custom-lists}

Listorna visas i kolumner. Du kan visa ytterligare information genom att ändra kolumnkonfigurationen. Om du vill göra det klickar du på **Konfigurera kolumn för en anpassad layout** -ikonen i det övre högra hörnet av listan.

![](assets/config-columns.png){width="70%" align="left"}

I **Konfigurera kolumner** rastrera, lägga till eller ta bort kolumner och ändra visningsordningen.

Exempel:

![](assets/columns.png){width="70%" align="left"}

I listan visas följande kolumner:

![](assets/column-sample.png){width="70%" align="left"}

Använd **Visa avancerade attribut** om du vill visa alla attribut för den aktuella listan. [Läs mer](#adv-attributes)

## Sortera data {#sort-lists}

Du kan också sortera objekt i listan genom att klicka på en kolumnrubrik. En pil visas (Upp eller Ned) som anger att listan är sorterad i den kolumnen.

För numeriska kolumner och datumkolumner finns **Upp** anger att listan är sorterad i stigande ordning medan **Ned** pil anger en fallande ordning. För strängar eller alfanumeriska kolumner visas värdena i alfabetisk ordning.

## Inbyggda filter {#list-built-in-filters}

Om du vill hitta objekt snabbare kan du använda sökfältet eller filtrera listan baserat på sammanhangsberoende kriterier.

![](assets/filter.png){width="70%" align="left"}

Du kan till exempel filtrera leveranser efter status, kanal, kontaktdatum eller mapp. Du kan också dölja tester.

## Egna filter{#list-custom-filters}

Om du vill skapa anpassade filter för data bläddrar du längst ned i filtren och klickar på **Lägg till regler** -knappen.

Dra och släpp attribut för att skapa filtervillkor i **Avancerade filter** skärm.

![](assets/custom-filter.png){width="70%" align="left"}

Använd **Visa avancerade attribut** om du vill visa alla attribut för den aktuella listan. [Läs mer](#adv-attributes)

## Använd avancerade attribut {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Visa avancerade attribut"
>abstract="Endast de vanligaste attributen visas som standard i attributlistan. Använd den här växeln för att skapa ett filter med avancerade attribut."

Endast de vanligaste attributen visas som standard i attributlistan och på filterkonfigurationsskärmar. Attribut som angetts som `advanced` attribut i dataschemat döljs från konfigurationsskärmarna.

Använd **Visa avancerade attribut** om du vill visa alla tillgängliga attribut för den aktuella listan.