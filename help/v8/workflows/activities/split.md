---
audience: end-user
title: Använda aktiviteten Dela arbetsflöde
description: Lär dig använda aktiviteten Dela arbetsflöde
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Dela {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Delad aktivitet"
>abstract="The **Dela** Med -aktivitet kan du segmentera inkommande populationer i flera deluppsättningar baserat på olika urvalskriterier, t.ex. filtreringsregler eller populationsstorlek."

The **Dela** aktiviteten är en **Målinriktning** aktivitet som gör att du kan segmentera inkommande populationer i flera deluppsättningar baserat på olika urvalskriterier, t.ex. filtreringsregler eller populationsstorlek.

## Konfigurera aktiviteten Dela {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segment för delad aktivitet"
>abstract="Lägg till så många delmängder som du vill för att segmentera den inkommande populationen.<br/></br>När **Dela** När aktiviteten utförs segmenteras populationen över de olika delmängderna i den ordning som de läggs till i aktiviteten. Innan du startar arbetsflödet bör du kontrollera att du har ordnat delmängderna i den ordning som passar dig med pilknapparna."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Dela aktivitetsfilter"
>abstract="Om du vill använda ett filtervillkor på delmängden klickar du på **[!UICONTROL Create filter]** och konfigurera önskad filtreringsregel med frågemodelleraren. Ta till exempel med profiler från den inkommande populationen vars e-postadress finns i databasen."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Arbeta med frågemodelleraren"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Gräns för delad aktivitet"
>abstract="Om du vill begränsa antalet profiler som markeras av delmängden aktiverar du **[!UICONTROL Enable limit]** och ange antal eller procentandelar av populationen som ska inkluderas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Sortering av delad aktivitet"
>abstract="När du anger en populationsgräns för en delmängd kan du rangordna de valda profilerna baserat på ett visst profilattribut i stigande eller fallande ordning. Aktivera **Aktivera sortering** alternativ. Du kan till exempel begränsa en delmängd så att den endast innehåller de 50 översta profilerna med det högsta inköpspriset."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Delad generering av komplementfärg"
>abstract="När du har konfigurerat alla deluppsättningar kan du välja den återstående populationen som inte matchade någon av deluppsättningarna och inkludera dem i en ytterligare utgående övergång. Aktivera **Generera komplement** alternativ."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Generera alla delmängder i samma tabell"
>abstract="Växla till det här alternativet om du vill gruppera alla delmängder i en enda utdataövergång."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="Hoppa över tom övergång"
>abstract="Växla **[!UICONTROL Skip empty transition]** om du vill inaktivera utdataövergången för den här delmängden om den inkommande populationen är tom."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_enable_overlapping"
>title="Aktivera överlappning av utdatapopulationer"
>abstract="Aktivera överlappning av utdatapopulationer"

Följ de här stegen för att konfigurera **Dela** aktivitet:

1. Lägg till en **Dela** till ditt arbetsflöde.

1. Aktivitetskonfigurationsrutan öppnas med en standarddelmängd. Klicka på **Lägg till segment** om du vill lägga till så många delmängder som behövs för att segmentera den inkommande populationen.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >När **Dela** När aktiviteten utförs segmenteras populationen över de olika delmängderna i den ordning som de läggs till i aktiviteten. Om till exempel den första delmängden återställer 70 % av den ursprungliga populationen, kommer nästa tillagda delmängd endast att tillämpa sina urvalskriterier på de återstående 30 %, och så vidare.
   >
   >Innan du startar arbetsflödet bör du kontrollera att du har beställt delmängderna i den ordning som passar dina behov. Det gör du genom att använda pilknapparna för att ändra positionen för en delmängd.

1. När deluppsättningar har lagts till visar aktiviteten så många utdataövergångar som det finns deluppsättningar. Vi rekommenderar starkt att du ändrar etiketten för varje delmängd så att du enkelt kan identifiera dem på arbetsytan.

1. Konfigurera hur varje delmängd ska filtrera den inkommande populationen. Följ dessa steg för att göra detta:

   1. Öppna delmängden för att visa dess egenskaper.

   1. Om du vill använda ett filtervillkor på delmängden klickar du på **[!UICONTROL Create filter]** och konfigurera önskad filtreringsregel med frågemodelleraren. Ta till exempel med profiler från den inkommande populationen vars e-postadress finns i databasen. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md)

   1. Om du vill begränsa antalet profiler som markeras av delmängden aktiverar du **[!UICONTROL Enable limit]** och ange antal eller procentandelar av populationen som ska inkluderas.

   1. Om du vill inaktivera en övergång om den inkommande populationen är tom växlar du **[!UICONTROL Skip empty transition]** på. Om ingen profil matchar delmängden kommer arbetsflödet inte att övergå till nästa aktivitet.

      ![](../assets/workflow-split-subset.png)


      >[!NOTE]
      >
      >När du anger en populationsgräns för en delmängd kan du rangordna de valda profilerna baserat på ett visst profilattribut i stigande eller fallande ordning. Aktivera **[!UICONTROL Enable sorting]** alternativ. Du kan till exempel begränsa en delmängd så att den endast innehåller de 50 översta profilerna med det högsta inköpspriset.

1. När du har konfigurerat alla deluppsättningar kan du välja den återstående populationen som inte matchade någon av deluppsättningarna och inkludera dem i en ytterligare utgående övergång. Aktivera **[!UICONTROL Generate complement]** alternativ.

   ![](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >The **[!UICONTROL Generate all subsets in the same table]** kan du gruppera alla delmängder till en enda utdataövergång.

Aktiviteten är nu konfigurerad. När arbetsflödet körs segmenteras populationen i de olika deluppsättningarna, i den ordning som de har lagts till i aktiviteten.

## Exempel{#split-example}

I följande exempel **[!UICONTROL Split]** -aktiviteten används för att segmentera en målgrupp i olika delmängder baserat på den kommunikationskanal som vi vill använda:

* **Delmängd 1 &quot;push&quot;**: Den här deluppsättningen omfattar alla profiler som har installerat vårt mobilprogram.
* **Delmängd 2 &quot;sms&quot;**: Användare av mobiltelefoner: För den återstående populationen som inte ingick i delmängd 1 tillämpar delmängd 2 en filtreringsregel för att välja profiler med mobiltelefoner i databasen.
* **Kompletteringsövergång**: Den här övergången fångar alla återstående profiler som inte matchade delmängd 1 eller delmängd 2. Det omfattar profiler som varken har installerat mobilappen eller en mobiltelefon, till exempel användare som inte har installerat mobilappen eller saknar ett registrerat mobilnummer.

![](../assets/workflow-split-example.png)
