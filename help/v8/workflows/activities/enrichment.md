---
audience: end-user
title: Använd arbetsflödesaktiviteten för anrikning
description: Lär dig hur du använder arbetsflödesaktiviteten för anrikning
badge: label="Alpha" type="Positive"
source-git-commit: 3fb46f0535c8511f21b62949e7604bd54f9993f7
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---


# Berikning {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Anrikningsaktivitet"
>abstract="Med Enrichment-aktiviteten kan du förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter riktade aktiviteter.<br/>När berikningsdata har lagts till i arbetsflödet kan de användas i aktiviteter som lagts till efter Enrichment-aktiviteten för att segmentera kunder i olika grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får genklang hos målgruppen."

The **Berikning** aktiviteten är en **Målinriktning** aktivitet. Det gör att du kan förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter segmenteringsaktiviteter.

Anrikningsdata kan komma antingen:

* **Från samma arbetsregister** som den som är inriktad på ditt arbetsflöde:

  *Ange en grupp kunder som målgrupp och lägg till fältet&quot;Födelsedatum&quot; i den aktuella arbetstabellen*

* **Från en annan arbetstabell**:

  *Ange kunder som målgrupp och lägg till fälten&quot;Belopp&quot; och&quot;Typ av produkt&quot; som kommer från tabellen&quot;Inköp&quot;*.

När anrikningsdata har lagts till i arbetsflödet kan de sedan användas i aktiviteter som lagts till efter **Berikning** aktiviteter för att segmentera kunder i distinkta grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får gensvar hos er målgrupp.

Du kan till exempel lägga till information om kundernas inköp i arbetsflödets arbetsregister och använda dessa data för att anpassa e-postmeddelanden med deras senaste köp eller hur mycket som spenderas på dessa inköp.

## Allmän konfiguration {#general}

Följ de här stegen för att konfigurera **Berikning** aktivitet:

1. Lägg till aktiviteter som **Bygg målgrupper** och **Kombinera** verksamhet.
1. Lägg till en **Berikning** aktivitet.
1. Klicka **Lägg till anrikningsdata**.

![](../assets/workflow-enrichment1.png)

Du kan välja mellan två typer av anrikningsdata: a [single enrichment attribute](#single-attribute) från måldimensionen, eller en [samlingslänk](#collection-link).

## Single enrichment-attribut {#single-attribute}

Här lägger vi bara till ett enda anrikningsattribut, till exempel födelsedatumet. Följ de här stegen:

1. Klicka inuti **Attribut** fält.
1. Välj ett enkelt fält från målgruppsdimensionen, födelsedatumet i vårt exempel.
1. Klicka **Bekräfta**.

![](../assets/workflow-enrichment2.png)

## Samlingslänk {#collection-link}

I det här mer komplicerade fallet väljer vi en samlingslänk som är en länk med en 1-N-kardinalitet mellan tabellerna. Vi hämtar de tre senaste inköpen som är mindre än 100$. Därför måste du definiera:

* ett anrikningsattribut: den **Totalt belopp** fält
* antalet rader som ska hämtas: 3
* ett filter: filtrera bort objekt som är större än 100$
* en sortering: underordnad sortering på **Orderdatum** fält.

### Lägg till attributet

Här väljer du den samlingslänk som ska användas som anrikningsdata.

1. Klicka inuti **Attribut** fält.
1. Klicka **Visa avancerade attribut**.
1. Välj **Totalt belopp** fält från **Inköp** tabell.

![](../assets/workflow-enrichment3.png)

### Definiera samlingsinställningarna

Definiera sedan hur data samlas in och hur många poster som ska hämtas.

1. Välj **Samla in data** i **Välj hur data samlas in** nedrullningsbar meny.
1. Skriv&quot;3&quot; i dialogrutan **Rader att hämta (kolumner att skapa)** fält.

![](../assets/workflow-enrichment4.png)

Om du t.ex. vill få fram genomsnittligt antal inköp för en kund väljer du **Sammanställda data** i stället, och markera **Genomsnittlig** i **Sammanställningsfunktion** nedrullningsbar meny.

![](../assets/workflow-enrichment5.png)

### Definiera filtren

Här definierar vi det högsta värdet för anrikningsattributet. Vi filtrerar bort objekt som är större än 100$.

1. Klicka **Redigera filter**.
1. Lägg till följande två filter: **Totalt belopp** finns AND **Totalt belopp** är mindre än 100. Den första filtrerar NULL-värden så som de skulle visas som det största värdet.
1. Klicka **Bekräfta**.

![](../assets/workflow-enrichment6.png)

### Definiera sorteringen

Vi måste nu använda sortering för att hämta de tre **senaste** inköp.

1. Aktivera **Aktivera sortering** alternativ.
1. Klicka inuti **Attribut** fält.
1. Välj **Orderdatum** fält.
1. Klicka **Bekräfta**.
1. Välj **Fallande** från **Sortera** nedrullningsbar meny.

![](../assets/workflow-enrichment7.png)

<!--

Add other fields
use it in delivery


cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->