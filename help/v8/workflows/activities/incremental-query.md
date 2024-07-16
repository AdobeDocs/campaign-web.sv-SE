---
audience: end-user
title: Använd inkrementell arbetsflödesaktivitet för fråga
description: Lär dig hur du använder arbetsflödesaktiviteten Inkrementell fråga
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 20%

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

Aktiviteten **Inkrementell fråga** är en **målaktivitet** som gör att du kan fråga databasen på schemalagd basis. Varje gång den här aktiviteten körs utesluts resultaten från tidigare körningar. På så sätt kan du bara rikta in dig på nya element.

>[!NOTE]
>
>Klientkonsolen för Campaign integrerar aktiviteten **[!UICONTROL Incremental query]** med en inbyggd schemaläggare, men gränssnittet för Campaign Web behandlar den här funktionen separat. Om du vill schemalägga inkrementella frågekörningar måste du lägga till en **[!UICONTROL Scheduler]**-aktivitet i arbetsflödet före **[!UICONTROL Incremental query]**-aktiviteten. [Lär dig konfigurera en schemaläggaraktivitet](scheduler.md)

Aktiviteten **[!UICONTROL Incremental query]** kan användas för olika typer av användning:

* Segmentera individer för att definiera målet för ett meddelande, en målgrupp osv.
* Exporterar data. Du kan till exempel använda aktiviteten för att regelbundet exportera nya loggar i filer. Det kan vara användbart om du vill använda dina loggdata i externa rapporterings- eller BI-verktyg.

Populationen som redan används av tidigare körningar lagras i arbetsflödet. Det innebär att två arbetsflöden som startas från samma mall inte delar samma logg. Två uppgifter som baseras på samma inkrementella fråga i samma arbetsflöde använder dock samma logg.

Om resultatet av en inkrementell fråga är lika med 0 under en av körningarna pausas arbetsflödet tills frågan körs nästa gång. De övergångar och aktiviteter som följer efter den stegvisa frågan bearbetas därför inte före nästa körning.

## Konfigurera aktiviteten Inkrementell fråga {#incremental-query-configuration}

Följ de här stegen för att konfigurera aktiviteten **Inkrementell fråga**:

![](../assets/incremental-query.png)

1. Lägg till en **inkrementell frågeaktivitet** i ditt arbetsflöde.

1. I avsnittet **[!UICONTROL Audience]** väljer du **Måldimension** och klickar sedan på **[!UICONTROL Continue]**.

   Med målinriktningsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter osv. Som standard är målet markerat bland mottagarna. [Läs mer om måldimensioner](../../audience/about-recipients.md#targeting-dimensions)

1. Använd frågemodelleraren för att definiera frågan, på samma sätt som du skapar en målgrupp när du utformar ett nytt e-postmeddelande. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md)

1. I avsnittet **[!UICONTROL Processed data]** väljer du det inkrementella läge som ska användas:

   * **[!UICONTROL Exclude results of previous execution]**: Varje gång aktiviteten körs exkluderas resultatet från tidigare körningar.

     Poster som redan har valts i tidigare körningar kan loggas i högst ett antal dagar från den dag de angavs som mål. Använd fältet **[!UICONTROL History in days]** om du vill göra det. Om värdet är noll rensas mottagarna aldrig från loggen.

   * **[!UICONTROL Use a date field]**: Med det här alternativet kan du exkludera resultat från tidigare körningar baserat på ett specifikt datumfält. Det gör du genom att välja önskat datumfält i listan över tillgängliga attribut för den valda måldimensionen. Vid nästa körning av arbetsflödet hämtas endast data som har ändrats eller skapats efter det senaste körningsdatumet.

     Efter den första körningen av arbetsflödet blir fältet **[!UICONTROL Last execution date]** tillgängligt. Det anger vilket datum som ska användas för nästa körning och uppdateras automatiskt varje gång arbetsflödet körs. Du kan fortfarande åsidosätta det här värdet genom att ange ett nytt värde manuellt så att det passar dina behov.

   >[!NOTE]
   >
   >**[!UICONTROL Use a date field]**-läget ger större flexibilitet beroende på vilket datumfält som är markerat. Om det angivna fältet till exempel motsvarar ett ändringsdatum, kan du i datumfältsläget hämta data som nyligen uppdaterats, medan det andra läget helt enkelt utelämnar inspelningar som redan har valts i en tidigare körning, även om de har ändrats sedan den senaste körningen av arbetsflödet.

## Exempel {#incremental-query-example}

I följande exempel visas konfigurationen av ett arbetsflöde som varje vecka filtrerar de profiler i Adobe Campaign-databasen som prenumererar på tjänsten Yoga Newsletter så att de får ett välkomstmeddelande.

![](../assets/incremental-query-example.png)

Arbetsflödet består av följande element:

* En **[!UICONTROL Scheduler]**-aktivitet som utför arbetsflödet varje måndag kl. 06.00.
* En **[!UICONTROL Incremental query]**-aktivitet som riktar sig till alla nuvarande prenumeranter under det första utförandet, och sedan endast till de nya prenumeranterna i den veckan under följande körningar.
* En **[!UICONTROL Email delivery]**-aktivitet.
