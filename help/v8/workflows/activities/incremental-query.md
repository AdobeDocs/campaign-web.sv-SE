---
audience: end-user
title: Använd inkrementell arbetsflödesaktivitet för fråga
description: Lär dig hur du använder arbetsflödesaktiviteten Inkrementell fråga
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 5%

---

# Inkrementell fråga {#incremental-query}

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Inkrementell fråga"
>abstract="Aktiviteten **Inkrementell fråga** är en **målaktivitet** som gör att du kan fråga databasen med hjälp av frågemodelleraren. Varje gång den här aktiviteten körs utesluts resultaten från tidigare körningar. På så sätt kan du bara rikta in dig på nya element."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Inkrementell frågehistorik"
>abstract="Inkrementell frågehistorik"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Inkrementell fråga Bearbetade data"
>abstract="Inkrementell fråga Bearbetade data"

Aktiviteten **Inkrementell fråga** är en **målaktivitet** som gör att du kan fråga databasen på schemalagd basis. Varje gång den här aktiviteten körs utesluts resultaten från tidigare körningar. Detta gör att du bara kan rikta in dig på nya element.

>[!NOTE]
>
>Klientkonsolen för Campaign integrerar aktiviteten **[!UICONTROL Incremental query]** med en inbyggd schemaläggare, men gränssnittet för Campaign Web behandlar den här funktionen separat. Om du vill schemalägga inkrementella frågekörningar lägger du till en **[!UICONTROL Scheduler]**-aktivitet i arbetsflödet före **[!UICONTROL Incremental query]**-aktiviteten. [Lär dig konfigurera en schemaläggaraktivitet](scheduler.md)

**[!UICONTROL Incremental query]**-aktiviteten kan användas för olika syften:

* Segmentera individer för att definiera målet för ett meddelande, en målgrupp eller andra åtgärder.
* Exporterar data. Använd till exempel aktiviteten för att regelbundet exportera nya loggar i filer. Detta är användbart för externa rapporterings- eller affärsinformationsverktyg.

Populationen som redan används av tidigare körningar lagras i arbetsflödet. Två arbetsflöden som startas från samma mall delar inte samma logg. Två uppgifter som baseras på samma inkrementella fråga i samma arbetsflöde använder dock samma logg.

Om resultatet av en inkrementell fråga är lika med 0 under en av körningarna pausas arbetsflödet tills frågan körs nästa gång. De övergångar och aktiviteter som följer efter den stegvisa frågan bearbetas inte före nästa körning.

## Konfigurera aktiviteten Inkrementell fråga {#incremental-query-configuration}

Följ de här stegen för att konfigurera aktiviteten **Inkrementell fråga**:

[Beskrivning: Skärmbild som visar konfigurationsgränssnittet för inkrementell frågeaktivitet i Adobe Campaign.]\
![](../assets/incremental-query.png)

1. Lägg till en **inkrementell frågeaktivitet** i ditt arbetsflöde.

1. I avsnittet **[!UICONTROL Audience]** väljer du **Måldimension** och klickar sedan på **[!UICONTROL Continue]**.

   Målgruppsdimensionen definierar målgruppen för insatsen, t.ex. mottagare, kontraktsanställda, operatörer eller prenumeranter. Som standard är målet markerat bland mottagarna. [Läs mer om måldimensioner](../../audience/about-recipients.md#targeting-dimensions)

1. Använd frågemodelleraren för att definiera frågan, ungefär som hur du skapar en målgrupp när du utformar ett nytt e-postmeddelande. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md)

1. I avsnittet **[!UICONTROL Processed data]** väljer du det inkrementella läge som ska användas:

   * **[!UICONTROL Exclude results of previous execution]**: Varje gång aktiviteten körs exkluderas resultatet från tidigare körningar.

     Poster som redan har valts i tidigare körningar kan loggas i högst ett antal dagar från den dag de angavs. Använd fältet **[!UICONTROL History in days]** för att ange det här värdet. Om värdet är noll rensas mottagarna aldrig från loggen.

   * **[!UICONTROL Use a date field]**: Det här alternativet utesluter resultat från tidigare körningar baserat på ett specifikt datumfält. Välj önskat datumfält i listan med tillgängliga attribut för den valda måldimensionen. Vid efterföljande körningar av arbetsflödet hämtas endast data som ändrats eller skapats efter det senaste körningsdatumet.

     Efter den första körningen av arbetsflödet blir fältet **[!UICONTROL Last execution date]** tillgängligt. Det anger vilket datum som ska användas för nästa körning och uppdateras automatiskt varje gång arbetsflödet körs. Du kan åsidosätta det här värdet manuellt efter dina behov.

   >[!NOTE]
   >
   >Läget **[!UICONTROL Use a date field]** ger större flexibilitet beroende på det valda datumfältet. Om det angivna fältet till exempel motsvarar ett ändringsdatum hämtar datumfältsläget data som uppdaterats nyligen. I det andra läget utesluts inspelningar som redan har gjorts i en tidigare körning, även om de har ändrats sedan den senaste körningen av arbetsflödet.

## Exempel {#incremental-query-example}

I följande exempel visas konfigurationen av ett arbetsflöde som filtrerar profiler i Adobe Campaign-databasen varje vecka. Det riktar sig till personer som prenumererar på Yoga Newsletter och skickar ett välkomstmejl till dem.

![Skärmbild av ett exempel på arbetsflödeskonfiguration för filtrering av profiler som prenumererar på tjänsten Yoga Newsletter.](../assets/incremental-query-example.png)

Arbetsflödet innehåller följande element:

* En **[!UICONTROL Scheduler]**-aktivitet som utför arbetsflödet varje måndag klockan 6.
* En **[!UICONTROL Incremental query]**-aktivitet som riktar sig till alla aktuella prenumeranter under den första körningen och endast nya prenumeranter under efterföljande körningar.
* En **[!UICONTROL Email delivery]**-aktivitet.