---
audience: end-user
title: Använd arbetsflödesaktiviteten Deduplicering
description: Lär dig hur du använder arbetsflödesaktiviteten Deduplicering
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 6%

---

# Deduplicering {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fält som identifierar dubbletter"
>abstract="I avsnittet **Fält som ska identifiera dubbletter** klickar du på knappen **Lägg till attribut** för att ange för vilka fält identiska värden tillåter att dubbletter identifieras, t.ex. e-postadress, förnamn och efternamn. Fältens ordning anger de som ska behandlas först."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Dedupliceringsaktivitet"
>abstract="Aktiviteten **Deduplicering** tar bort dubbletter i resultatet av inkommande aktiviteter. Det används främst efter målinriktningsaktiviteter och före aktiviteter som använder målinriktade data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generera ett komplement"
>abstract="Du kan generera ytterligare en utgående övergång med den återstående populationen uteslutits som dubbletter. Aktivera alternativet **Generera komplement** om du vill göra det."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Inställningar för borttagning av dubbletter"
>abstract="Om du vill ta bort dubbletter i inkommande data definierar du dedupliceringsmetoden i fälten nedan. Som standard sparas bara en post. Välj dedupliceringsläge baserat på ett uttryck eller ett attribut. Som standard väljs den post som ska hållas utanför dubbletterna slumpmässigt."

Aktiviteten **Deduplicering** är en **målaktivitet**. Den här aktiviteten tar bort dubbletter i resultatet av inkommande aktiviteter, t.ex. duplicerade profiler i mottagarlistan. Aktiviteten **Deduplicering** används vanligtvis efter målaktiviteter och före aktiviteter som använder måldata.

## Konfigurera aktiviteten Deduplicering {#deduplication-configuration}

Så här konfigurerar du aktiviteten **Deduplicering**:

![Konfigurationsprocess för deduplicering av arbetsflöde](../assets/workflow-deduplication.png)

1. Lägg till en **borttagning av dubbletter**-aktivitet i arbetsflödet.

1. I avsnittet **Fält som ska identifiera dubbletter** klickar du på knappen **Lägg till attribut** för att ange för vilka fält identiska värden tillåter att dubbletter identifieras, t.ex. e-postadress, förnamn och efternamn. Fältens ordning anger de som ska behandlas först. [Lär dig hur du väljer attribut och lägger till dem i favoriter](../../get-started/attributes.md).

1. I avsnittet **Dedupliceringsinställningar** väljer du antalet unika **dubbletter som ska behållas**. Standardvärdet för det här fältet är 1. Värdet 0 behåller alla dubbletter.

   Om till exempel posterna A och B betraktas som dubbletter av posten Y, och post C betraktas som en dubblett av posten Z:

   * Om värdet för fältet är 1: endast Y- och Z-posterna behålls.
   * Om värdet för fältet är 0: alla register förs.
   * Om fältets värde är 2: posterna C och Z behålls och två poster från A, B och Y behålls, antingen som en slump eller beroende på vald borttagningsmetod.

1. Välj den **borttagningsmetod** som ska användas:

   * **Slumpmässig markering**: Markerar posten slumpmässigt så att den inte innehåller några dubbletter.
   * **Använder ett uttryck**: Behåller poster där värdet för det angivna uttrycket är det minsta eller största.
   * **Värden som inte är tomma**: Behåller posterna som uttrycket inte är tomt för.
   * **Följ en lista med värden**: Definierar en värdeprioritet för ett eller flera fält. Om du vill definiera värdena klickar du på **Attribut** för att välja ett fält eller skapa ett uttryck och lägger sedan till värdena i rätt tabell. Om du vill definiera ett nytt fält klickar du på knappen **Lägg till** som finns ovanför listan med värden.

1. Markera alternativet **Generera komplement** om du vill utnyttja den återstående populationen. Komplementet består av alla dubbletter. Därefter läggs ytterligare en övergång till i aktiviteten.

## Exempel {#deduplication-example}

I följande exempel använder du en dedupliceringsaktivitet för att exkludera dubbletter från målet innan du skickar en leverans. De identifierade duplicerade profilerna läggs till i en dedikerad målgrupp som kan återanvändas om det behövs. Identifiera dubbletterna genom att välja **E-postadress**. Behåll 1 post och välj borttagningsmetoden **Slumpmässig**.

![Exempel på dedupliceringsaktivitet i ett arbetsflöde](../assets/workflow-deduplication-example.png)