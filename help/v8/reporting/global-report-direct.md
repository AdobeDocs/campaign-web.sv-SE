---
audience: end-user
title: Globala rapporter för direktreklamkanalen
description: Läs mer om Global-rapporter för direktreklamkanalen
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# Globala rapporter för direktreklamkanalen {#global-report-direct}

De globala rapporterna för direktreklam ger användarna en heltäckande översikt över trafik- och engagemangsmått på kanalnivå.

Navigera till menyn **[!UICONTROL Reports]** i avsnittet **[!UICONTROL Reporting]**. Du kan filtrera dina data beroende på rapportens datum, mapp eller regler. [Läs mer](global-reports.md)

## Leveranssammanfattning {#delivery-summary-direct}

### Leveransöversikt {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="Leveransöversikt"
>abstract="I **leveransöversikten** presenteras nyckeltal (KPI:er) som ger djupgående insikter i besökarnas interaktion med varje direktutskick. Mätvärdena beskrivs nedan."

**[!UICONTROL Delivery Overview]** presenterar nyckeltal (KPI:er) som ger djupgående insikter i besökarnas interaktion med varje direktutskick. Mätvärdena beskrivs nedan.

![Den här bilden visar leveransöversiktsmått för direktutskick.](assets/global_report_direct_mail_delivery_overview.png){zoomable="yes"}{align="center"}

+++Läs mer om leveransöversiktssiffror.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Errors]**: Totalt antal fel som ackumulerats under leverans och automatisk returbearbetning i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Unsubscribes]**: Antal mottagare som klickat på länkar för att ta bort prenumeration.

+++

### Målgrupp {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="Målgrupp"
>abstract="Mottagardata och meddelandeinformation visas i diagrammet **Målgrupp**, som avspeglar leveransförberedelseanalysen."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="Målgrupp"
>abstract="Tabellen **Målgrupp** innehåller en detaljerad beskrivning av dina mottagare och motsvarande meddelanden, baserat på resultatet av leveransförberedelseprocessen."

Tabellen och diagrammet för **[!UICONTROL Targeted Audience]** visar data relaterade till dina mottagare, med detaljerade mått angivna nedan.

![Den här bilden visar målgruppsmått för direktreklam.](assets/global_report_direct_mail_targeted_audience.png){zoomable="yes"}{align="center"}

+++Läs mer om målgruppsstatistik.

* **[!UICONTROL Targeted audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas, t.ex. adress som saknas, är i karantän eller på en blockeringslista.

+++

### Leveransstatistik {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="Leveransstatistik"
>abstract="Diagrammet **Leveransstatistik** ger insikter om hur effektiva dina direktleveranser är, inklusive slutförda leveranser och eventuella fel som påträffats."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="Leveransstatistik"
>abstract="Tabellen **Leveransstatistik** innehåller information om hur din direktleverans lyckades och om fel som uppstått."

Diagrammet och tabellen **[!UICONTROL Delivery statistics]** innehåller en beskrivning av framgången för varje direktutskick, med detaljerade mätvärden som anges nedan.

+++Läs mer om leveransstatistik.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats, i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors / Bounces]**: Totalt antal fel som ackumulerats under leveranser och automatisk ombunden bearbetning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter en misslyckad leverans (t.ex. okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

### Orsaker till uteslutning {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="Undantag"
>abstract="Tabellen **Orsaker till uteslutning** visar en detaljerad beskrivning, per regel, av meddelanden som avvisats under leveransförberedelseprocessen."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="Orsaker till uteslutning"
>abstract="Diagrammet **Orsaker till uteslutning** illustrerar distributionen av avvisade meddelanden under förberedelsen för leverans, kategoriserat av varje regel."

![Den här bilden visar orsaken till uteslutningsmått för direktreklam.](assets/global_report_direct_mail_exclusions.png){zoomable="yes"}{align="center"}

Diagrammet och tabellen Uteslutningar visar orsakerna till att användarprofiler, som inte ingår i målprofilerna, inte kunde ta emot meddelandet.

+++Läs mer om orsaker till undantag.

* **[!UICONTROL Address in quarantine]**: Feltypen som genereras när en adress placeras i karantän.

* **[!UICONTROL Address not specified]**: Feltypen som genererades när en leverans skickades för att ange att adressen inte finns.

* **[!UICONTROL Bad quality address]**: Feltypen som genereras när kvalitetsklassen för postadresser är för låg.

* **[!UICONTROL Denylisted address]**: Feltypen som genererades när mottagaren blocklist när leveransen utfördes.

* **[!UICONTROL Double]**: Feltypen som genererades när mottagaren exkluderades eftersom dess nyckelvärden inte var unika.

* **[!UICONTROL Control group]**: Mottagarens adress är en del av kontrollgruppen.

* **[!UICONTROL Target limited in size]**: Den maximala leveransstorleken har uppnåtts för mottagaren.

+++