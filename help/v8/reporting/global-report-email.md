---
audience: end-user
title: Globala rapporter för e-postkanalen
description: Läs mer om globala rapporter för e-postkanalen
exl-id: 37c575e5-fd18-4a35-a11a-922d5bda1bae
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '1491'
ht-degree: 1%

---

# Globala rapporter för e-postkanalen {#global-report-direct}

De globala rapporterna ger användarna en heltäckande översikt över trafik- och engagemangsmätningar på kanalnivå.

Navigera till **[!UICONTROL Reports]** menyn i **[!UICONTROL Reporting]** -avsnitt. Du kan filtrera dina data beroende på rapportdatumet, mappen eller reglerna. [Läs mer](global-reports.md)

## Leveranssammanfattning {#delivery-summary-email}

### Leveransöversikt {#delivery-overview-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_deliveries_overview_email"
>title="Leveransöversikt"
>abstract="The **Leveransöversikt** presenterar nyckeltal (KPI:er) som ger djupgående insikter om hur er målgrupp interagerar med de e-postleveranser och -kampanjer ni skickar."

The **[!UICONTROL Delivery Overview]** presenterar nyckeltal (KPI:er) som ger djupgående insikter om hur besökarna interagerar med varje e-postleverans. Mätvärdena beskrivs nedan.

![](assets/global_report_email_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om leveransöversiktssiffror.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Total opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Total clicks]**: Totalt antal mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Bounces & errors]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Unsubscribes]**: Antal mottagare som klickat på Avbeställ.
+++

### Målgrupp {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_email"
>title="Inledande målgruppsstatistik"
>abstract="The **Målgrupp** register och diagram ger insikter om mottagarnas engagemang, så att ni kan bedöma hur effektiva era kampanjer och leveranser är."

Tabell och diagram för **[!UICONTROL Targeted Audience]** visa data om era mottagare, med detaljerade mått som anges nedan.

![](assets/global_report_email_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om målgruppsstatistik.

* **[!UICONTROL Targeted audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista osv.

+++

### Leveransstatistik {#delivery-summary-email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_email_delivery_stats"
>title="Leveransstatistik"
>abstract="The **Leveransstatistik** diagram- och tabelldispositionsstatistik, inklusive lyckade leveranser, fel och nya karantän, som ger en kortfattad översikt för att utvärdera leveransresultatet."

The **[!UICONTROL Delivery statistics]** tabellen innehåller en beskrivning av hur väl varje e-postleverans lyckats, med detaljerade mått som beskrivs nedan.

![](assets/global_report_email_delivery_statistics.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om leveransstatistik.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors / Bounces]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

### Orsaker till uteslutning {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusion_email"
>title="Orsaker till uteslutning"
>abstract="The **Orsaker till uteslutning** diagram och tabell visar de specifika orsakerna till att meddelanden nekas under färdigställandet av leveransen, med en detaljerad beskrivning per regel."

![](assets/global_report_email_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

Diagrammet och tabellen Uteslutningar visar orsakerna till att användarprofiler, som inte ingår i målprofilerna, inte kunde ta emot meddelandet.

E-postfeltyperna listas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## Leveranskapacitet {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_email"
>title="Leveranskapacitet"
>abstract="Detta **Leveransflöde** ger omfattande insikter om leveransflöde, framhäv framgångar och felfrekvens inom en viss tidsram."

![](assets/global_report_email_delivery_throughput.png){zoomable=&quot;yes&quot;}{align="center"}

Rapporten Leveransflöde ger djupgående insikter om hur effektiv leveransprocessen är och ger en detaljerad översikt över lyckade resultat och felprocent inom en viss tidsram.

+++Läs mer om leveransstatistik.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

+++

## Ej levererbara {#non-deliverables-email}

### Uppdelning av fel per typ {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_type_email"
>title="Uppdelning av fel per typ"
>abstract="Tabellen och diagrammet som beskriver **Uppdelning av fel per typ** Innehåller information om olika feltyper som påträffas under processen, bland annat okänd användare, postlåda full, ogiltig domän och andra."

![](assets/global_report_email_breakdown_type.png){zoomable=&quot;yes&quot;}{align="center"}

The **[!UICONTROL Breakdown of errors per type]** tabellen och diagrammet innehåller data om potentiella fel som uppstått i olika domäner, med specifika mått som anges nedan.

Felen som visas i den här rapporten utlöser karantänprocessen. Mer information om karantänhantering finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++Läs mer om indelning av fel per typmått.

* **[!UICONTROL User unknown]**: Feltyp som genererades under leveransen för att ange att e-postadressen är ogiltig.

* **[!UICONTROL Invalid domain]**: Feltyp som genereras när en leverans skickas för att ange att domänen för e-postadressen är fel eller inte finns.

* **[!UICONTROL Mailbox full]**: Feltyp som genererats efter fem leveransförsök för att ange att mottagarens inkorg innehåller för många meddelanden.

* **[!UICONTROL Account disabled]**: Feltyp som genereras när en leverans skickas för att ange att adressen inte längre finns.

* **[!UICONTROL Refused]**: Feltyp som genereras när en adress nekas av IAP (Internet Access Provider), till exempel efter att en säkerhetsregel (antispam-program) har tillämpats.

* **[!UICONTROL Unreachable]**: Feltyp som inträffar i meddelandedistributionssträngen: incident i SMTP-reläet, domän som inte går att nå temporärt, osv.

* **[!UICONTROL Not connected]**: Feltyp som anger att mottagarens mobiltelefon är avstängd eller frånkopplad från nätverket vid tidpunkten för sändningen.

+++

### Uppdelning av fel per domän {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_domain_email"
>title="Uppdelning av fel per domän"
>abstract="Tabellen och diagrammet som illustrerar **Uppdelning av fel per domän** presentera data för varje feltyp som påträffas, indelat i specifika domäner."

![](assets/global_report_email_breakdown_domain.png){zoomable=&quot;yes&quot;}{align="center"}

The **[!UICONTROL Breakdown of errors per domain]** tabellen och diagrammet visar data relaterade till potentiella fel inom varje domän. Mätvärdena är gemensamma med **[!UICONTROL Breakdown of errors per type]** tabellen och diagrammet som anges ovan.

## Spårningsindikatorer {#tracking-indicators-email}

### Leveransstatistik {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_global_delivery_statistics_summary_email"
>title="Leveransstatistik"
>abstract="The **Leveransstatistik** KPI:er (Key Performance Indicators) ger en heltäckande översikt över era leveranser och kampanjresultat, och ger insikter om både lyckade leveranser, påträffade fel och användarengagemang."

The **[!UICONTROL Delivery statistics]** Mätvärden innehåller nyckeltal (KPI) som ger detaljerad information om data som är kopplade till varje e-postleverans. Mer information om dessa mått finns nedan.

![](assets/global_report_email_delivery_statistics_tracking.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om leveransstatistik.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Unique opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Total Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Clicks on the opt-out link]**: Antal klick på länken för att avbryta prenumerationen.

* **[!UICONTROL Clicks on the mirror link]**: Antal klick på länken till spegelsidan.

* **[!UICONTROL Estimation of forwards]**: Uppskattning av antalet e-postmeddelanden som vidarebefordras av målmottagarna.
+++

### Öppen och klickbar frekvens {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_open_clickthrough_email"
>title="Öppnings- och klickfrekvens"
>abstract="Tabellen för **Öppet och klickfrekvensen** visar mottagarnas engagemang för er leverans, visar data om öppningsfrekvenser och klickfrekvens för en snabb och insiktsfull översikt."

The **[!UICONTROL Open and click-trough rate]** tabellen visar data som är relativa till mottagarna. Mätvärdena anges nedan.

![](assets/global_report_email_opens.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om Open och click-trough rate metrics.

* **[!UICONTROL Sent]**: Totalt antal skickade meddelanden.

* **[!UICONTROL Complaints]**: Antal och procentandel meddelanden för den här domänen som har rapporterats som oönskade av mottagaren.

* **[!UICONTROL Unique Opens]**: Antal och procentandel distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Unique Clicks]**: Antal och procentandel av distinkta målmottagare som klickade på samma leverans minst en gång.

* **[!UICONTROL Raw reactivity]**: Procentandel av antalet mottagare som klickade på en leverans minst en gång jämfört med antalet mottagare som öppnade en leverans minst en gång.
+++

## URL:er och klickströmmar {#url-email}

### URL:er och klicka på strömmar KPI:er {#url-email-kpis}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_clickstreams_email"
>title="URL:er och klickströmmar"
>abstract="The **URL:er och klickbara strömmar** rapporten innehåller viktiga KPI:er (Key Performance Indicators) som ger detaljerade insikter om de mest klickade URL:erna under en leverans."

The **[!UICONTROL URLs and click streams]** rapporten innehåller nyckeltal (KPI:er) som ger detaljerade insikter om de URL:er som fick det högsta antalet klick under en leverans. Mätvärdena anges nedan.

![](assets/campaign_report_email_9.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om URL:er och klicka på strömma mätvärden.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat i en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

* **[!UICONTROL Unique clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Total Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Platform average]** : Detta medelvärde, som visas för varje frekvens (reaktivitet, distinkta klick och kumulerade klick), beräknas för leveranser som skickats under de senaste sex månaderna. Endast leveranser med samma typologi och i samma kanal beaktas. Korrektur ingår inte.
+++

### De tio mest besökta länkarna {#top10-global-report-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_top10_email"
>title="De tio mest besökta länkarna"
>abstract="The **De tio mest besökta länkarna**  diagram och tabell visar omfattande data om hur mottagarna interagerar med varje länk."

The **[!UICONTROL Top 10 most visited links]** diagram och tabell innehåller tillgängliga data för mottagarnas beteende per länk. Mätvärdena anges nedan.

![](assets/global_report_email_top10.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om de 10 mest besökta länkarna.

* **[!UICONTROL Total Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Percentage]**: Procentandel användare som interagerade med leveransen.

+++

### Klicknedbrytning över tid {#global-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_click_breakdown_email"
>title="Klicknedbrytning över tid"
>abstract="The **Klicknedbrytning över tid** diagram ger en heltäckande bild av hur mottagarna interagerar med länkar under den angivna tidsramen."

The **[!UICONTROL Breakdown of clicks over time]** diagrammet innehåller tillgängliga data för mottagarnas beteende per länk.

![](assets/global_report_email_breakdown_clicks.png){zoomable=&quot;yes&quot;}{align="center"}

## Användaraktiviteter {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_user_activities_email"
>title="Användaraktiviteter"
>abstract="Den grafiska representationen av **Användaraktiviteter** ger en detaljerad beskrivning av mottagarnas interaktioner, möjlighet att portrera och klicka i ett informativt diagramformat."

The **[!UICONTROL User activities]** rapporten visar hur öppningar och klickningar i form av ett diagram är uppdelade. Mätvärden för den här rapporten finns nedan.

![](assets/global_report_email_user.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om mått för användaraktiviteter.

* **[!UICONTROL Total Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Total Opens]**: Totalt antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++
