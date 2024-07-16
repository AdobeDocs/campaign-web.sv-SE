---
audience: end-user
title: Använda aktiviteten Dela arbetsflöde
description: Lär dig använda aktiviteten Dela arbetsflöde
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: 6ae019bf9f4775dc7eb58e9429a75a8ad69026ff
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# Dela {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Delad aktivitet"
>abstract="Med aktiviteten **Dela** kan du segmentera inkommande populationer i flera deluppsättningar baserat på olika urvalskriterier, t.ex. filtreringsregler eller populationsstorlek."

Aktiviteten **Dela** är en **målaktivitet** som gör att du kan segmentera inkommande populationer i flera deluppsättningar baserat på olika urvalskriterier, till exempel filtreringsregler eller populationsstorlek.

## Konfigurera aktiviteten Dela {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segment för delad aktivitet"
>abstract="Lägg till så många delmängder som du vill för att segmentera den inkommande populationen.<br/></br>När aktiviteten **Dela** körs segmenteras populationen mellan de olika delmängderna i den ordning som de läggs till i aktiviteten. Innan du startar arbetsflödet bör du kontrollera att du har ordnat delmängderna i den ordning som passar dig med pilknapparna."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Dela aktivitetsfilter"
>abstract="Om du vill använda ett filtreringsvillkor för delmängden klickar du på **[!UICONTROL Create filter]** och konfigurerar den önskade filtreringsregeln med frågemodelleraren. Ta till exempel med profiler från den inkommande populationen vars e-postadress finns i databasen."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Arbeta med frågemodelleraren"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Gräns för delad aktivitet"
>abstract="Om du vill begränsa antalet profiler som markeras av delmängden aktiverar du alternativet **[!UICONTROL Enable limit]** och anger antalet eller procentsatserna för den population som ska inkluderas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Sortering av delad aktivitet"
>abstract="När du anger en populationsgräns för en delmängd kan du rangordna de valda profilerna baserat på ett visst profilattribut i stigande eller fallande ordning. Aktivera alternativet **Aktivera sortering** om du vill göra det. Du kan till exempel begränsa en delmängd så att den endast innehåller de 50 översta profilerna med det högsta inköpspriset."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Delad generering av komplementfärg"
>abstract="När du har konfigurerat alla deluppsättningar kan du välja den återstående populationen som inte matchade någon av deluppsättningarna och inkludera dem i en ytterligare utgående övergång. Aktivera alternativet **Generera komplement** om du vill göra det."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Generera alla delmängder i samma tabell"
>abstract="Växla till det här alternativet om du vill gruppera alla delmängder i en enda utdataövergång."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="Hoppa över tom övergång"
>abstract="Aktivera alternativet **[!UICONTROL Skip empty transition]** om du vill inaktivera utdataövergången för den här delmängden om den inkommande populationen är tom."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_enable_overlapping"
>title="Aktivera överlappning av utdatapopulationer"
>abstract=" Med alternativet **[!UICONTROL Enable overlapping of output populations]** kan du hantera populationer som tillhör flera delmängder. När rutan inte är markerad ser delningsaktiviteten till att en mottagare inte kan finnas i flera utdataövergångar, även om den uppfyller villkoren för flera delmängder. De kommer att vara i målet för den första fliken med matchande villkor. När rutan är markerad kan mottagarna hittas i flera delmängder om de uppfyller filtervillkoren. Adobe Campaign rekommenderar att man använder exklusiva kriterier."

Följ de här stegen för att konfigurera aktiviteten **Dela**:

1. Lägg till en **delad**-aktivitet i ditt arbetsflöde.

1. Aktivitetskonfigurationsrutan öppnas med en standarddelmängd. Klicka på knappen **Lägg till segment** om du vill lägga till så många delmängder som behövs för att segmentera den inkommande populationen.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >När aktiviteten **Dela** körs segmenteras populationen över de olika delmängderna i den ordning som de läggs till i aktiviteten. Om till exempel den första delmängden återställer 70 % av den ursprungliga populationen, kommer nästa tillagda delmängd endast att tillämpa sina urvalskriterier på de återstående 30 %, och så vidare.
   >
   >Innan du startar arbetsflödet bör du kontrollera att du har beställt delmängderna i den ordning som passar dina behov. Det gör du genom att använda pilknapparna för att ändra positionen för en delmängd.

1. När deluppsättningar har lagts till visar aktiviteten så många utdataövergångar som det finns deluppsättningar. Vi rekommenderar starkt att du ändrar etiketten för varje delmängd så att du enkelt kan identifiera dem på arbetsytan.

1. Konfigurera hur varje delmängd ska filtrera den inkommande populationen. Följ dessa steg för att göra detta:

   1. Öppna delmängden för att visa dess egenskaper.

   1. Om du vill använda ett filtreringsvillkor för delmängden klickar du på **[!UICONTROL Create filter]** och konfigurerar den önskade filtreringsregeln med frågemodelleraren. Ta till exempel med profiler från den inkommande populationen vars e-postadress finns i databasen. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md)

   1. Om du vill begränsa antalet profiler som markeras av delmängden aktiverar du alternativet **[!UICONTROL Enable limit]** och anger antalet eller procentsatserna för den population som ska inkluderas.

   1. Om du vill inaktivera en övergång om den inkommande populationen är tom aktiverar du alternativet **[!UICONTROL Skip empty transition]**. Om ingen profil matchar delmängden kommer arbetsflödet inte att övergå till nästa aktivitet.

      ![](../assets/workflow-split-subset.png)


      >[!NOTE]
      >
      >När du anger en populationsgräns för en delmängd kan du rangordna de valda profilerna baserat på ett visst profilattribut i stigande eller fallande ordning. Aktivera alternativet **[!UICONTROL Enable sorting]** om du vill göra det. Du kan till exempel begränsa en delmängd så att den endast innehåller de 50 översta profilerna med det högsta inköpspriset.

1. När du har konfigurerat alla deluppsättningar kan du välja den återstående populationen som inte matchade någon av deluppsättningarna och inkludera dem i en ytterligare utgående övergång. Aktivera alternativet **[!UICONTROL Generate complement]** om du vill göra det.

   ![](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >Med alternativet **[!UICONTROL Generate all subsets in the same table]** kan du gruppera alla delmängder till en enda utdataövergång.

1. Med alternativet **[!UICONTROL Enable overlapping of output populations]** kan du hantera populationer som tillhör flera delmängder:

   * När rutan inte är markerad ser delningsaktiviteten till att en mottagare inte kan finnas i flera utdataövergångar, även om den uppfyller villkoren för flera delmängder. De kommer att vara i målet för den första fliken med matchande villkor.
   * När rutan är markerad kan mottagarna hittas i flera delmängder om de uppfyller filtervillkoren. Adobe Campaign rekommenderar att man använder exklusiva kriterier.

Aktiviteten är nu konfigurerad. När arbetsflödet körs segmenteras populationen i de olika deluppsättningarna, i den ordning som de har lagts till i aktiviteten.

## Exempel{#split-example}

I följande exempel används aktiviteten **[!UICONTROL Split]** för att segmentera en målgrupp i distinkta delmängder baserat på kommunikationskanalen som vi vill använda:

* **Delmängd 1 &quot;push&quot;**: Den här delmängden innehåller alla profiler som har installerat vårt mobilprogram.
* **Delmängd 2 &quot;sms&quot;**: Användare av mobiltelefoner: För den återstående populationen som inte ingick i delmängd 1 tillämpar delmängd 2 en filtreringsregel för att välja profiler med mobiltelefoner i databasen.
* **Kompletteringsövergång**: Den här övergången fångar alla återstående profiler som inte matchade delmängd 1 eller delmängd 2. Det omfattar profiler som varken har installerat mobilappen eller en mobiltelefon, till exempel användare som inte har installerat mobilappen eller saknar ett registrerat mobilnummer.

![](../assets/workflow-split-example.png)
