---
audience: end-user
title: Bläddra bland, söka i och filtrera listor
description: Upptäck hur du bläddrar bland och filtrerar listor Campaign Web v8
badge: label="Beta"
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: 3e94514060a501a3a359c38606e5532beaf20f10
workflow-type: tm+mt
source-wordcount: '559'
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

Använd **Visa avancerade attribut** om du vill visa alla attribut för den aktuella listan. [Läs mer](#adv-attributes)

## Sortera data {#sort-lists}

Du kan också sortera objekt i listan genom att klicka på en kolumnrubrik. En pil visas (Upp eller Ned) som anger att listan är sorterad i den kolumnen.

För numeriska kolumner och datumkolumner finns **Upp** anger att listan är sorterad i stigande ordning medan **Ned** pil anger en fallande ordning. För strängar eller alfanumeriska kolumner visas värdena i alfabetisk ordning.

## Inbyggda filter {#list-built-in-filters}

Om du vill hitta objekt snabbare kan du använda sökfältet eller filtrera listan baserat på sammanhangsberoende kriterier.

![](assets/filter.png){width="70%" align="left" zoomable="yes"}

Du kan till exempel filtrera leveranser efter status, kanal, kontaktdatum eller mapp. Du kan också dölja tester.

## Egna filter{#list-custom-filters}

Om du vill skapa anpassade filter för data bläddrar du längst ned i filtren och klickar på knappen **Lägg till regler** för att komma åt regelbyggaren.

Dra och släpp attribut för att skapa filtervillkor i **Avancerade filter** skärm.

![](assets/custom-filter.png){width="70%" align="left" zoomable="yes"}

Använd **Visa avancerade attribut** om du vill visa alla attribut för den aktuella listan. [Läs mer](#adv-attributes)

Regelbyggarens princip för anpassade filter liknar den regel som används för att skapa målgrupper. Detaljerad information om hur det används finns i [Målgruppsdokumentation](../audience/segment-builder.md).

## Använd avancerade attribut {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Visa avancerade attribut"
>abstract="Endast de vanligaste attributen visas som standard i attributlistan. Aktivera **Visa avancerade attribut** växla om du vill visa alla tillgängliga attribut för den aktuella listan på den vänstra paletten i regelbyggaren, till exempel noder, grupperingar, 1-1-länkar och 1-N-länkar."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Avancerade fält för regelbyggaren"
>abstract="Endast de vanligaste attributen visas som standard i attributlistan. Aktivera **Visa avancerade attribut** växla om du vill visa alla tillgängliga attribut för den aktuella listan på den vänstra paletten i regelbyggaren, till exempel noder, grupperingar, 1-1-länkar och 1-N-länkar."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Avancerade attribut för regelbyggaren"
>abstract="Endast de vanligaste attributen visas som standard i attributlistan. Aktivera **Visa avancerade attribut** växla om du vill visa alla tillgängliga attribut för den aktuella listan på den vänstra paletten i regelbyggaren, till exempel noder, grupperingar, 1-1-länkar och 1-N-länkar."


Endast de vanligaste attributen visas som standard i attributlistan och på filterkonfigurationsskärmar. Attribut som angetts som `advanced` attribut i dataschemat döljs från konfigurationsskärmarna.

Aktivera **Visa avancerade attribut** växla om du vill visa alla tillgängliga attribut för den aktuella listan på den vänstra paletten i regelbyggaren, till exempel noder, grupperingar, 1-1-länkar och 1-N-länkar. Attributlistan uppdateras omedelbart.


![](assets/adv-toggle.png){width="70%" align="left" zoomable="yes"}
