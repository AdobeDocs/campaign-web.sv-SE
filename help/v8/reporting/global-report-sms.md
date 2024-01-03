---
audience: end-user
title: Globala rapporter för SMS-kanalen
description: Förstå globala rapporter för SMS-kanalen
badge: label="Begränsad tillgänglighet"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 2%

---

# Globala rapporter för SMS-kanalen {#campaign-reports-sms}

De globala rapporterna ger användarna en heltäckande översikt över trafik- och engagemangsmätningar på kanalnivå.

Navigera till **[!UICONTROL Reports]** menyn i **[!UICONTROL Reporting]** -avsnitt. Du kan filtrera dina data beroende på rapportdatumet, mappen eller reglerna. [Läs mer](global-reports.md)

## Leveranssammanfattning {#delivery-summary-sms}

### Leveransöversikt {#delivery-overview-sms}

The **[!UICONTROL Delivery Overview]** rapporten innehåller omfattande nyckeltal (KPI:er) som ger djupgående insikter i besökarnas interaktionsmönster för varje SMS-leverans. Följande mätvärden beskrivs nedan.

![](assets/global_report_sms_delivery_overview.png)

+++Läs mer om leveransöversiktssiffror.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Procentandel meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Click-through rate]**: Procentandel distinkta mottagare som klickade på en leverans minst en gång.

* **[!UICONTROL Errors]**: Procentandel fel som ackumulerats under leverans och automatisk returbehandling i förhållande till det totala antalet skickade meddelanden.

+++

### Målgrupp {#delivery-summary-sms-initial-target}

The **[!UICONTROL Targeted audience]** tabellen och diagrammet innehåller data som är relaterade till mottagarna för varje skickad SMS-leverans. Mätvärdena anges nedan.

![](assets/global_report_sms_targeted_audience.png)

+++Läs mer om målgruppsstatistik.

* **[!UICONTROL Targeted audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista osv.

+++

### Leveransstatistik {#delivery-summary-sms-exec-stats}

The **[!UICONTROL Delivery statistics]** tabellen visar hur bra du har lyckats med varje SMS-leverans. Mätvärdena anges nedan.

![](assets/global_report_sms_delivery_statistics.png)

+++Läs mer om leveransstatistik.

* **[!UICONTROL Total messages]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors / Bounces]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

  SMS-feltyper listas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Orsaker till uteslutning {#causes-exclusion}

The **[!UICONTROL Causes of exclusion]** I diagram och tabeller visas orsakerna till att användarprofiler, som inte ingick i målprofilerna, inte kunde ta emot SMS-leveranser.

Feltyperna listas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Leveranskapacitet {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

Den här rapporten innehåller omfattande information om leveransflödet inom en angiven tidsram.
