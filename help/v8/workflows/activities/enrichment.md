---
audience: end-user
title: Använd arbetsflödesaktiviteten för anrikning
description: Lär dig hur du använder arbetsflödesaktiviteten för anrikning
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '1655'
ht-degree: 0%

---

# Berikning {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Anrikningsaktivitet"
>abstract="The **Berikning** kan du förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter segmenteringsaktiviteter."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Anrikningsaktivitet"
>abstract="När berikningsdata har lagts till i arbetsflödet kan de användas i aktiviteter som lagts till efter Enrichment-aktiviteten för att segmentera kunder i olika grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får genklang hos målgruppen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_simplejoin"
>title="Länkdefinition"
>abstract="Skapa en länk mellan data i arbetstabellen och Adobe Campaign-databasen. Om du till exempel läser in data från en fil som innehåller mottagarnas kontonummer, land och e-postadress måste du skapa en länk till landstabellen för att kunna uppdatera informationen i deras profiler."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_reconciliation"
>title="Anrikningsavstämning"
>abstract="anrikningsavstämning"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Anrikningsdata"
>abstract="Välj de data som ska användas för att förbättra arbetsflödet. Du kan välja två typer av anrikningsdata: ett enskilt anrikningsattribut från måldimensionen, eller en samlingslänk, som är en länk med en 1-N-kardinalitet mellan tabellerna."

The **Berikning** aktiviteten är en **Målinriktning** aktivitet. Det gör att du kan förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter segmenteringsaktiviteter.

Anrikningsdata kan komma antingen:

* **Från samma arbetsregister** som den som är inriktad på ditt arbetsflöde:

  *Ange en grupp kunder som målgrupp och lägg till fältet&quot;Födelsedatum&quot; i den aktuella arbetsregistret*.

* **Från en annan arbetstabell**:

  *Ange kunder som målgrupp och lägg till fälten&quot;Belopp&quot; och&quot;Typ av produkt&quot; från tabellen&quot;Inköp&quot;*.

När anrikningsdata har lagts till i arbetsflödet kan de användas i aktiviteter som lagts till efter **Berikning** aktiviteter för att segmentera kunder i distinkta grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får gensvar hos er målgrupp.

Du kan till exempel lägga till information om kundernas inköp i arbetsflödets arbetsregister och använda dessa data för att anpassa e-postmeddelanden med deras senaste köp eller hur mycket som spenderas på dessa inköp.

## Lägg till en anrikningsaktivitet {#enrichment-configuration}

Följ de här stegen för att konfigurera **Berikning** aktivitet:

1. Lägg till aktiviteter som **Bygg målgrupper** och **Kombinera** verksamhet.
1. Lägg till en **Berikning** aktivitet.
1. Om flera övergångar har konfigurerats i arbetsflödet kan du använda **[!UICONTROL Primary set]** -fält för att definiera vilken övergång som ska användas som primär uppsättning för att berika med data.

## Lägg till anrikningsdata {#enrichment-add}

1. Klicka **Lägg till anrikningsdata** och välj det attribut som ska användas för att förbättra data.

   Du kan välja två typer av anrikningsdata: ett enskilt anrikningsattribut från måldimensionen eller en samlingslänk. Var och en av dessa typer beskrivs i exemplen nedan:
   * [Single enrichment-attribut](#single-attribute)
   * [Samlingslänk](#collection-link)

   >[!NOTE]
   >
   >The **Redigera uttrycksknapp** på skärmen för attributval kan du skapa avancerade uttryck för att välja attributet. [Lär dig arbeta med uttrycksredigeraren](../../query/expression-editor.md)

   ![](../assets/workflow-enrichment1.png)

## Skapa länkar mellan tabeller {#create-links}

The **[!UICONTROL Link definition]** kan du skapa en länk mellan data i arbetstabellen och Adobe Campaign-databasen. Om du till exempel läser in data från en fil som innehåller mottagarnas kontonummer, land och e-postadress måste du skapa en länk till landstabellen för att kunna uppdatera informationen i deras profiler.

Det finns flera typer av länkar:

* **[!UICONTROL 1 cardinality simple link]**: Varje post från den primära uppsättningen kan kopplas till en och endast en post från de länkade data.
* **[!UICONTROL 0 or 1 cardinality simple link]**: Varje post i den primära uppsättningen kan kopplas till 0- eller 1-posten från de länkade data, men inte till fler än en.
* **[!UICONTROL N cardinality collection link]**: Varje post från den primära uppsättningen kan kopplas till 0, 1 eller fler (N) poster från länkade data.

Så här skapar du en länk:

1. I **[!UICONTROL Link definition]** klickar du på **[!UICONTROL Add link]** -knappen.

   ![](../assets/workflow-enrichment-link.png)

1. I **Relationstyp** väljer du den typ av länk du vill skapa.

1. Identifiera det mål som du vill länka den primära uppsättningen till:

   * Om du vill länka en befintlig tabell i databasen väljer du **[!UICONTROL Database schema]** och välj önskad tabell i **[!UICONTROL Target schema]** fält.
   * Om du vill länka till data från indataövergången väljer du **Tillfälligt schema** och markera den övergång vars data du vill använda.

1. Definiera avstämningskriterierna för att matcha data från den primära uppsättningen med det länkade schemat. Det finns två typer av kopplingar:

   * **Enkelt hörn**: Välj ett specifikt attribut för att matcha data från de två scheman. Klicka **Lägg till join** och väljer **Källa** och **Mål** attribut som ska användas som avstämningskriterier.
   * **Avancerad join**: Skapa en koppling med avancerade villkor. Klicka **Lägg till join** och klicka på **Skapa villkor** för att öppna frågemodelleraren.

Ett arbetsflödesexempel med hjälp av länkar finns i [Exempel](#link-example) -avsnitt.

## Datavstämning {#reconciliation}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Datavstämning"
>abstract="Arbetsflödesaktiveringsaktiviteten kan nu användas för att stämma av data från Campaign-databasschemat med data från ett annat schema, eller med data från ett tillfälligt schema, till exempel data som överförts med en Läs in filaktivitet."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Se versionsinformation"


The **Berikning** -aktiviteten kan användas för att stämma av data från Campaign-databasschemat med data från ett annat schema, eller med data från ett temporärt schema, till exempel data som överförts med en Läs in filaktivitet. Den här typen av länk definierar en avstämning mot en unik post. Adobe Campaign skapar en länk till en måltabell genom att lägga till en sekundärnyckel i den för att lagra en referens till den unika posten.

Du kan till exempel använda det här alternativet för att stämma av en profils land, som anges i en överförd fil, med något av de länder som är tillgängliga i den dedikerade tabellen i Campaign-databasen.

Följ stegen för att konfigurera **Berikning** aktivitet med en avstämningslänk:

1. Klicka på **Lägg till länk** knappen i **Avstämning** -avsnitt.
1. Identifiera de data som du vill skapa en avstämningslänk med.

   * Om du vill skapa en avstämningslänk med data från Campaign-databasen väljer du **Databasschema** och välj det schema där målet ska lagras.
   * Om du vill skapa en avstämningslänk med data från indataövergången väljer du **Tillfälligt schema** och välj den arbetsflödesövergång där måldata lagras.

1. The **Etikett** och **Namn** fält fylls i automatiskt baserat på det valda målschemat. Du kan ändra deras värden om det behövs.

1. I **Avstämningskriterier** anger du hur du vill att data från käll- och måltabellerna ska stämma överens:

   * **Enkelt hörn**: Stäm av ett specifikt fält från källtabellen med ett annat fält i måltabellen. Klicka på **Lägg till join** och ange **Källa** och **Mål** fält som ska användas för avstämningen.

     >[!NOTE]
     >
     >Du kan använda en eller flera **Enkelt hörn** kriterier, i vilket fall de måste verifieras så att uppgifterna kan sammankopplas.

   * **Avancerad join**: Använd frågemodelleraren för att konfigurera avstämningsvillkoren. Klicka på **Skapa villkor** och sedan definiera dina avstämningskriterier genom att skapa en egen regel med hjälp av AND- och OR-operationer.

I exemplet nedan visas ett arbetsflöde som är konfigurerat för att skapa en länk mellan mottagartabellen för Adobe Campaign-databasen och en tillfällig tabell som genererats av **Läs in fil** aktivitet. I det här exemplet avstäms båda tabellerna med e-postadressen som avstämningskriterier av Enrichment-aktiviteten.

![](../assets/enrichment-reconciliation.png)

## Exempel {#example}

### Single enrichment-attribut {#single-attribute}

Här lägger vi bara till ett enda anrikningsattribut, till exempel födelsedatumet. Följ de här stegen:

1. Klicka inuti **Attribut** fält.
1. Välj ett enkelt fält från målgruppsdimensionen, födelsedatumet i vårt exempel.
1. Klicka **Bekräfta**.

![](../assets/workflow-enrichment2.png)

### Samlingslänk {#collection-link}

I det här mer komplicerade fallet väljer vi en samlingslänk som är en länk med en 1-N-kardinalitet mellan tabellerna. Vi hämtar de tre senaste inköpen som är mindre än 100$. Därför måste du definiera:

* ett anrikningsattribut: **Totalt belopp** fält
* antalet rader som ska hämtas: 3
* ett filter: filtrera bort objekt som är större än 100$
* en sortering: underordnad sortering på **Orderdatum** fält.

#### Lägg till attributet {#add-attribute}

Här väljer du den samlingslänk som ska användas som anrikningsdata.

1. Klicka inuti **Attribut** fält.
1. Klicka **Visa avancerade attribut**.
1. Välj **Totalt belopp** fält från **Inköp** tabell.

![](../assets/workflow-enrichment3.png)

#### Definiera samlingsinställningarna{#collection-settings}

Definiera sedan hur data samlas in och hur många poster som ska hämtas.

1. Välj **Samla in data** i **Välj hur data samlas in** nedrullningsbar meny.
1. Skriv&quot;3&quot; i dialogrutan **Rader att hämta (kolumner att skapa)** fält.

![](../assets/workflow-enrichment4.png)

Om du t.ex. vill få fram genomsnittligt antal inköp för en kund väljer du **Sammanställda data** i stället, och markera **Genomsnittlig** i **Sammanställningsfunktion** nedrullningsbar meny.

![](../assets/workflow-enrichment5.png)

#### Definiera filtren{#collection-filters}

Här definierar vi det högsta värdet för anrikningsattributet. Vi filtrerar bort objekt som är större än 100$. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md)

1. Klicka **Redigera filter**.
1. Lägg till följande två filter: **Totalt belopp** finns AND **Totalt belopp** är mindre än 100. Den första filtrerar NULL-värden så som de skulle visas som det största värdet.
1. Klicka **Bekräfta**.

![](../assets/workflow-enrichment6.png)

#### Definiera sorteringen{#collection-sorting}

Vi måste nu använda sortering för att hämta de tre **senaste** inköp.

1. Aktivera **Aktivera sortering** alternativ.
1. Klicka inuti **Attribut** fält.
1. Välj **Orderdatum** fält.
1. Klicka **Bekräfta**.
1. Välj **Fallande** från **Sortera** nedrullningsbar meny.

![](../assets/workflow-enrichment7.png)

### Berika med länkade data {#link-example}

I exemplet nedan visas ett arbetsflöde som är konfigurerat för att skapa en länk mellan två övergångar. De första övergångarna avser profildata med hjälp av en **Fråga** medan den andra övergången innehåller inköpsdata som lagras i en fil som läses in via en Läs in-filaktivitet.

![](../assets/enrichment-uc-link.png)

* Den första **Berikning** aktivitetslänkar den primära uppsättningen (data från **Fråga** aktivitet) med schemat från **Läs in fil** aktivitet. På så sätt kan vi matcha varje profil som används av frågan med motsvarande inköpsdata.

  ![](../assets/enrichment-uc-link-purchases.png)

* En sekund **Berikning** aktiviteten läggs till för att berika data från arbetsflödestabellen med inköpsdata från **Läs in fil** aktivitet. Detta gör att vi kan använda dessa data i ytterligare aktiviteter, till exempel för att anpassa meddelanden som skickas till kunderna med information om deras köp.

  ![](../assets/enrichment-uc-link-data.png)

