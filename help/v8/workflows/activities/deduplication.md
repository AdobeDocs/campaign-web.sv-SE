---
audience: end-user
title: Använd arbetsflödesaktiviteten Deduplicering
description: Lär dig hur du använder arbetsflödesaktiviteten Deduplicering
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 3%

---


# Deduplicering {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Dedupliceringsattribut"
>abstract="På så sätt kan du ange för vilka fält identiska värden gör att dubbletter kan identifieras: e-postadress, förnamn, efternamn osv. I fältordningen kan du ange vilka som ska behandlas först."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Dedupliceringsaktivitet"
>abstract="The **Deduplicering** kan du ta bort dubbletter i resultatet av inkommande aktiviteter. Det används främst efter målinriktningsaktiviteter och före aktiviteter som tillåter användning av målinriktade data."


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generera ett komplement"
>abstract="Du kan generera ytterligare en utgående övergång med den återstående populationen, som har uteslutits som en dubblett. Aktivera **Generera komplement** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Inställningar för borttagning av dubbletter"
>abstract="Om du vill ta bort dubbletter i inkommande data definierar du dedupliceringsmetoden i fälten nedan. Som standard sparas bara en post. Du bör också välja dedupliceringsläget baserat på ett uttryck eller ett attribut. Som standard väljs den post som ska hållas utanför dubbletterna slumpmässigt."

The **Deduplicering** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan du ta bort dubbletter i resultatet av de inkommande aktiviteterna. The **Deduplicering** aktiviteten används vanligtvis efter målinriktningsaktiviteter och före aktiviteter som tillåter användning av måldata.

## Konfigurera aktiviteten Deduplicering{#deduplication-configuration}

Följ de här stegen för att konfigurera **Deduplicering** aktivitet:

![](../assets/workflow-deduplication.png)

1. Lägg till en **Deduplicering** till ditt arbetsflöde.

1. I **Fält som identifierar dubbletter** klickar du på **Lägg till attribut** för att ange de fält där identiska värden gör det möjligt att identifiera dubbletter: e-postadress, förnamn, efternamn osv. I fältordningen kan du ange vilka som ska behandlas först.

1. Välj antalet unika **Dubbletter att behålla**. Standardvärdet för det här fältet är 1. Med värdet 0 kan du behålla alla dubbletter.

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. Välj **Dedupliceringsmetod** att använda:

   * **Slumpmässig markering**: markerar slumpmässigt den post som ska tas bort från dubbletterna.
   * **Använda ett uttryck**: det gör att du kan behålla de poster där det angivna uttryckets värde är det minsta eller det största.
   * **Följ en lista med värden**: låter dig definiera en värdeprioritet för ett eller flera fält. Definiera värdena genom att klicka **Attribut** om du vill markera ett fält eller skapa ett uttryck och sedan lägga till värdena i rätt tabell. Om du vill definiera ett nytt fält klickar du på knappen Lägg till ovanför listan med värden.

1. Kontrollera **Generera komplement** om du vill utnyttja den återstående populationen. Komplementet består av alla dubbletter. Därefter läggs ytterligare en övergång till aktiviteten.

## Exempel{#deduplication-example}

I följande exempel använder vi en dedupliceringsaktivitet för att exkludera dubbletter från målet innan vi skickar en leverans. De identifierade dubbletterna läggs till i en dedikerad målgrupp som kan återanvändas om det behövs. Vi använder **E-post** för att identifiera dubbletter. Vi väljer att behålla 1 post och väljer **Slumpmässig** dedupliceringsmetod.

![](../assets/workflow-deduplication-example.png)
