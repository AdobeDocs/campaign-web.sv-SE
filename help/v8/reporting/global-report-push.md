---
audience: end-user
title: Globala rapporter för push-kanalen
description: Förstå globala rapporter för push-kanalen
badge: label="Begränsad tillgänglighet"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

# Globala rapporter för push-kanalen {#campaign-reports-push}

De globala rapporterna ger användarna en heltäckande översikt över trafik- och engagemangsmätningar på kanalnivå.

Navigera till **[!UICONTROL Reports]** menyn i **[!UICONTROL Reporting]** -avsnitt. Du kan filtrera dina data beroende på rapportdatumet, mappen eller reglerna. [Läs mer](global-reports.md)

## Leveranssammanfattning {#delivery-summary-push}

### Leveransöversikt {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Översikt över push-leverans"
>abstract="The Push **leveransöversikt** KPI:er ger en grundlig granskning av era push-leveranser och ger detaljerade insikter och specifika data. Den innehåller omfattande information om leveransens prestanda, effektivitet och resultat."

The **[!UICONTROL Delivery Overview]** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med varje leverans av push-meddelanden. Mätvärdena anges nedan.

![](assets/global_report_push_delivery_overview.png)

+++Läs mer om leveransöversiktssiffror.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Total clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

+++

### Målgrupp {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Skjut målpopulationen"
>abstract="The **Målgrupp** diagram och tabeller visar data relaterade till er publik med push-meddelanden, med information om meddelanden som ska levereras och undantag."

The **[!UICONTROL Targeted audience]** tabellen och diagrammet innehåller data som är relaterade till mottagarna för varje sändning av push-meddelanden. Mätvärdena anges nedan.

![](assets/global_report_push_targeted_audience.png)

+++Läs mer om målgruppsstatistik.

* **[!UICONTROL Targeted audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista osv.

+++

### Leveransstatistik {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Statistik för push-leverans"
>abstract="The **Övergripande statistik** rapporten innehåller information om skickade push-meddelanden, inklusive antalet lyckade, misslyckade och karantän."

The **[!UICONTROL Delivery statistics]** tabellen visar hur väl varje push-meddelandeleverans har lyckats. Mätvärdena anges nedan.

![](assets/global_report_push_delivery_statistics.png)

+++Läs mer om leveransstatistik.

* **[!UICONTROL Total messages]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors / Bounces]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (ogiltig registrering, avvisning av meddelande, nyttolastfel, till exempel) i förhållande till antalet meddelanden som ska levereras.

  Feltyperna för push-meddelanden visas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Orsaker till uteslutning {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Uteslutningsorsaker"
>abstract="The **Orsaker till uteslutning** diagram och tabell visar de olika anledningar som gjorde att användarprofiler inte kunde ta emot push-meddelanden."

The **[!UICONTROL Causes of exclusion]** I diagram och tabeller visas orsakerna till att användarprofiler som har uteslutits från målprofilerna inte kunde ta emot meddelandet.

Feltyperna för push-meddelanden visas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## Leveranskapacitet {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Rapport om leveransdataflöde"
>abstract="The **Leveransflöde** rapporten innehåller detaljerad information om hela plattformens leveransflöde för push-meddelanden inom en angiven tidsram."

![](assets/global_report_push_delivery_throughput.png)

The **[!UICONTROL Delivery Throughput]** rapporten ger omfattande insikter om hur effektivt leveranssystemet för push-meddelanden är, och innehåller en detaljerad sammanfattning av lyckade resultat och felprocent under en viss period.

