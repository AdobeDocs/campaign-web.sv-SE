---
audience: end-user
title: Globala rapporter för direktreklamkanalen
description: Läs mer om Global-rapporter för direktreklamkanalen
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 1%

---

# Globala rapporter för direktreklamkanalen {#global-report-direct}

De globala rapporterna ger användarna en heltäckande översikt över trafik- och engagemangsmätningar på kanalnivå.

Navigera till **[!UICONTROL Reports]** menyn i **[!UICONTROL Reporting]** -avsnitt. Du kan filtrera dina data beroende på rapportdatumet, mappen eller reglerna. [Läs mer](global-reports.md)

## Leveranssammanfattning {#delivery-summary-direct}

### Leveransöversikt {#delivery-overview-direct}

The **[!UICONTROL Delivery Overview]** presenterar nyckeltal (KPI:er) som ger djupgående insikter om hur besökarna interagerar med varje e-postleverans. Mätvärdena beskrivs nedan.

![](assets/global_report_email_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om leveransöversiktssiffror.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Unsubscribes]**: Antal mottagare som klickat på Avbeställ.
+++

### Målgrupp {#delivery-summary-direct-initial-target}

Tabell och diagram för **[!UICONTROL Targeted Audience]** visa data om era mottagare, med detaljerade mått som anges nedan.

![](assets/global_report_email_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om målgruppsstatistik.

* **[!UICONTROL Targeted audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista osv.

+++

### Leveransstatistik {#delivery-summary-direct-exec-stats}

The **[!UICONTROL Delivery statistics]** tabellen innehåller en beskrivning av hur väl varje direktmejlleverans lyckats, med detaljerade mätvärden som anges nedan.

![](assets/global_report_email_delivery_statistics.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om leveransstatistik.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors / Bounces]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

### Orsaker till uteslutning {#causes-exclusion}

![](assets/global_report_email_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

Diagrammet och tabellen Uteslutningar visar orsakerna till att användarprofiler, som inte ingår i målprofilerna, inte kunde ta emot meddelandet.

## Leveranskapacitet {#delivery-throughput}

Den här rapporten innehåller omfattande information om leveransflödet inom en angiven tidsram. Det nyckeltal som används för att mäta hastigheten för meddelandeleverans är antalet meddelanden som skickas per timme.

## Ej levererbara {#non-deliverables-direct}

### Uppdelning av fel per typ {#delivery-summary-direct-breakdown-per-type}

The **[!UICONTROL Breakdown of errors per type]** tabellen och diagrammet innehåller data om potentiella fel som uppstått i olika domäner, med specifika mått som anges nedan.

Felen som visas i den här rapporten utlöser karantänprocessen. Mer information om karantänhantering finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++Läs mer om indelning av fel per typmått.

* **[!UICONTROL User unknown]**: Feltyp som genererades under leveransen för att ange att adressen är ogiltig.

* **[!UICONTROL Invalid domain]**: Feltyp som genereras när en leverans skickas för att ange att adressens domän är felaktig eller inte finns.

* **[!UICONTROL Mailbox full]**: Feltyp som genererats efter fem leveransförsök för att ange att mottagarens inkorg innehåller för många meddelanden.

* **[!UICONTROL Account disabled]**: Feltyp som genereras när en leverans skickas för att ange att adressen inte längre finns.

* **[!UICONTROL Refused]**: Feltyp som genereras när en adress nekas av IAP (Internet Access Provider), till exempel efter att en säkerhetsregel (antispam-program) har tillämpats.

* **[!UICONTROL Unreachable]**: Feltyp som inträffar i meddelandedistributionssträngen: incident i SMTP-reläet, domän som inte går att nå temporärt, osv.

* **[!UICONTROL Not connected]**: Feltyp som anger att mottagarens mobiltelefon är avstängd eller frånkopplad från nätverket vid tidpunkten för sändningen.

+++

### Uppdelning av fel per domän {#delivery-summary-email-breakdown-per-domain}

The **[!UICONTROL Breakdown of errors per domain]** tabellen och diagrammet visar data relaterade till potentiella fel inom varje domän. Mätvärdena är gemensamma med **[!UICONTROL Breakdown of errors per type]** tabellen och diagrammet som anges ovan.

