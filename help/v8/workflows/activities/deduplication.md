---
audience: end-user
title: Använd arbetsflödesaktiviteten Deduplicering
description: Lär dig hur du använder arbetsflödesaktiviteten Deduplicering
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 17%

---

# Deduplicering {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fält som identifierar dubbletter"
>abstract="I **Fält som identifierar dubbletter** klickar du på **Lägg till attribut** för att ange de fält där identiska värden gör det möjligt att identifiera dubbletter, t.ex. e-postadress, förnamn, efternamn osv. I fältordningen kan du ange vilka som ska behandlas först."

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

The **Deduplicering** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan du ta bort dubbletter i resultatet av de inkommande aktiviteterna, till exempel duplicerade profiler i mottagarlistan. The **Deduplicering** aktiviteten används vanligtvis efter målinriktade aktiviteter och före aktiviteter som tillåter användning av måldata.

## Konfigurera aktiviteten Deduplicering{#deduplication-configuration}

Följ de här stegen för att konfigurera **Deduplicering** aktivitet:

![](../assets/workflow-deduplication.png)

1. Lägg till en **Deduplicering** till ditt arbetsflöde.

1. I **Fält som identifierar dubbletter** klickar du på **Lägg till attribut** för att ange de fält där identiska värden gör det möjligt att identifiera dubbletter, t.ex. e-postadress, förnamn, efternamn osv. I fältordningen kan du ange vilka som ska behandlas först.

1. I **Inställningar för borttagning av dubbletter** väljer du antalet unika **Dubbletter att behålla**. Standardvärdet för det här fältet är 1. Med värdet 0 kan du behålla alla dubbletter.

   Om till exempel posterna A och B betraktas som dubbletter av posten Y, och en post C betraktas som en dubblett av posten Z:

   * Om värdet för fältet är 1: endast Y- och Z-posterna behålls.
   * Om värdet för fältet är 0: alla register förs.
   * Om värdet för fältet är 2: Posterna C och Z förvaras och två poster från A, B och Y sparas, av en tillfällighet eller beroende på vilken dedupliceringsmetod som valts därefter.

1. Välj **Dedupliceringsmetod** att använda:

   * **Slumpmässig markering**: markerar slumpmässigt den post som ska tas bort från dubbletterna.
   * **Använda ett uttryck**: det gör att du kan behålla de poster där det angivna uttryckets värde är det minsta eller det största.
   * **Följ en lista med värden**: låter dig definiera en värdeprioritet för ett eller flera fält. Definiera värdena genom att klicka **Attribut** om du vill markera ett fält eller skapa ett uttryck och sedan lägga till värdena i rätt tabell. Om du vill definiera ett nytt fält klickar du på knappen Lägg till ovanför listan med värden.

1. Kontrollera **Generera komplement** om du vill utnyttja den återstående populationen. Komplementet består av alla dubbletter. Därefter läggs ytterligare en övergång till aktiviteten.

## Exempel{#deduplication-example}

I följande exempel använder du en dedupliceringsaktivitet för att exkludera dubbletter från målet innan du skickar en leverans. De identifierade duplicerade profilerna läggs till i en dedikerad målgrupp som kan återanvändas om det behövs. Välj **E-post** adress för att identifiera dubbletterna. Behåll 1 post och välj **Slumpmässig** dedupliceringsmetod.

![](../assets/workflow-deduplication-example.png)
