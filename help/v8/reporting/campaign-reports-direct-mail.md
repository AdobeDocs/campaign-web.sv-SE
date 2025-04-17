---
audience: end-user
title: Kampanjrapporter för Direct-postkanalen
description: Förstå kampanjrapporter för Direct mail channel
exl-id: 7817d4c5-1f97-4b17-8a5f-f1a5b8701fe9
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Kampanjrapporter för Direct-postkanalen {#campaign-reports-direct-mail}

Varje kampanjrapport är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel. Rapporter och mätvärden för direktreklamkanalen finns nedan. Lär dig hur du får åtkomst till dina kampanjrapporter på [den här sidan](campaign-reports.md).

## Leveranssammanfattning {#delivery-summary-direct}

### Leveransöversikt {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_delivery_overview_direct_mail"
>title="Leveransöversikt"
>abstract="I **leveransöversikten** presenteras nyckeltal (KPI:er) som ger djupgående insikter i besökarnas interaktion med varje direktutskick. Mätvärdena beskrivs nedan."

**[!UICONTROL Delivery Overview]** presenterar nyckeltal (KPI:er) som ger djupgående insikter i besökarnas interaktion med varje direktutskick. Mätvärdena beskrivs nedan.

![Översikt över leveransstatistik för direktreklamkampanjer](assets/direct-mail-campaign-overview.png){zoomable="yes"}{align="center"}

+++Läs mer om leveransöversiktssiffror.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Errors]**: Totalt antal fel som ackumulerats under leverans och automatisk returbearbetning i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Total clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

### Inledande målgruppsstatistik {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_target_audience_direct_mail"
>title="Inledande målgruppsstatistik"
>abstract="Mottagardata och meddelandeinformation visas i tabellen **Inledande målgruppsstatistik**, som avspeglar leveransförberedelseanalysen."

Tabellen **[!UICONTROL Initial target audience statistics]** visar data som är relaterade till dina mottagare. Mätvärden beräknas under färdigställandet av leveransen och visar den initiala målgruppen, antalet meddelanden som ska skickas och antalet exkluderade mottagare.

![Statistik för den ursprungliga målgruppen för direktreklamkampanjer](assets/direct-mail-campaign-target-audience.png){zoomable="yes"}

+++Läs mer om statistik för inledande målgrupper.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas, till exempel saknade adresser, adresser i karantän eller adresser på en blockeringslista.

+++

### Körningsstatistik {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_execution_statistics_direct_mail"
>title="Leveransstatistik"
>abstract="Tabellen **Körningsstatistik** innehåller information om hur din direktsändning lyckades och om fel som uppstod."

![Körningsstatistik för direktreklamkampanjer](assets/direct-mail-campaign-exec.png)

Tabellen **[!UICONTROL Execution statistics]** innehåller en beskrivning av resultatet för varje direktutskick, med detaljerade mått som anges nedan.

+++Läs mer om leveransstatistik.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats, i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som ackumulerats under leveranser och automatisk ombunden bearbetning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter en misslyckad leverans (t.ex. okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

### Genererade klickströmmar {#click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_clicks_direct_mail"
>title="Genererade klickströmmar"
>abstract="Tabellen **Genererade klickströmmar** visar tillgängliga data i relation till hur mottagarna interagerade med leveransen."

![Klicka på strömdata för direktreklamkampanjer](assets/direct-mail-campaign-clicks.png){zoomable="yes"}{align="center"}

Tabellen **Genererade klickströmmar** visar orsakerna till att användarprofiler, som inte ingår i målprofilerna, inte kunde ta emot meddelandet.

+++Läs mer om genererade klickströmningsvärden.

* **[!UICONTROL Unique clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Total clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickade i en leverans, i förhållande till det beräknade antalet målmottagare som öppnade en leverans.

+++