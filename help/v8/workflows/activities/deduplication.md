---
audience: end-user
title: Använd arbetsflödesaktiviteten Deduplicering
description: Lär dig hur du använder arbetsflödesaktiviteten Deduplicering
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 12%

---


# Deduplicering {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Gaffelaktivitet"
>abstract="Med aktiviteten Deduplicering kan du.."

Med aktiviteten Deduplicering kan du ta bort dubbletter i resultatet/resultaten av de inkommande aktiviteterna.

Aktiviteten för borttagning av dubbletter används vanligtvis efter målinriktningsaktiviteter och före aktiviteter som tillåter användning av måldata.

## Konfiguration

Följ de här stegen för att konfigurera **Schemaläggare** aktivitet:

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
   * **Använda ett uttryck**: det gör att du kan behålla de poster där det angivna uttryckets värde är det minsta eller det största. ++ Uttryck ++ Sortera
   * **Följ en lista med värden**: låter dig definiera en värdeprioritet för ett eller flera fält. Definiera värdena genom att klicka **Attribut** om du vill markera ett fält eller skapa ett uttryck och sedan lägga till värdena i rätt tabell. Om du vill definiera ett nytt fält klickar du på knappen Lägg till ovanför listan med värden. ++ Sortera

1. Kontrollera **Generera komplement** om du vill utnyttja den återstående populationen. Komplementet består av alla dubbletter. Därefter läggs ytterligare en övergång till aktiviteten.