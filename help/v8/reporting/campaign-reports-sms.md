---
audience: end-user
title: Kampanjrapporter för SMS-kanalen
description: Förstå kampanjrapporter för SMS-kanalen
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Kampanjrapporter för SMS-kanalen {#campaign-reports-sms-channel}

Varje kampanjrapport är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel. Rapporter och mätvärden för SMS-kanalen anges nedan. Lär dig hur du får tillgång till dina kampanjrapporter på [den här sidan](campaign-reports.md).

## Leveranssammanfattning {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Leveransöversikt"
>abstract="Rapporten **Leveransöversikt** innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med SMS-leveransen."

Rapporten **[!UICONTROL Delivery Overview]** innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med SMS-leveransen. Mätvärdena anges nedan.

![Leveransöversiktsrapport med SMS-statistik](assets/campaign_report_sms_1.png){zoomable="yes"}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Total sent]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Errors]**: Totalt antal fel som ackumulerats under leverans och automatisk returbearbetning i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

### Inledande målgruppsstatistik {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Inledande målgruppsstatistik"
>abstract="Tabellen **Inledande målgruppsstatistik** visar data i förhållande till dina mottagare."

Tabellen **[!UICONTROL Initial target audience statistics]** visar data i förhållande till dina mottagare. Mätvärdena anges nedan.

![Inledande statistiktabell över målgrupper som visar mottagardata](assets/campaign_report_sms_2.png){zoomable="yes"}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas, t.ex. adress som saknas, är i karantän eller på blockeringslista.

+++

### Körningsstatistik {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Körningsstatistik"
>abstract="Tabellen **Körningsstatistik** visar hur din leverans lyckades: meddelanden som ska levereras, slutföras, fel och nya karantän."

Tabellen **[!UICONTROL Execution statistics]** innehåller information om leveransframgången. Mätvärdena anges nedan.

![Körningsstatistikregister som visar leveransmått](assets/campaign_report_sms_3.png){zoomable="yes"}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats, i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som ackumulerats under leveranser och automatisk återinläsning, i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter en misslyckad leverans (okänd användare, ogiltig domän), i relation till antalet meddelanden som ska levereras.

  SMS-feltyper visas i [Adobe Campaign v8-dokumentationen (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Genererade klickströmmar {#delivery-summary-sms-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Genererade klickströmmar"
>abstract="Tabellen **Genererade klickströmmar** visar tillgängliga data i relation till hur mottagarna interagerade med leveransen."

Tabellen **[!UICONTROL Generated click streams]** visar data i relation till hur mottagarna interagerade med leveransen. Mätvärdena anges nedan.

![Genererad klickströmstabell som visar interaktionsdata för mottagare](assets/campaign_report_sms_4.png){zoomable="yes"}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som har klickat i en leverans och det beräknade antalet målmottagare som har öppnat en leverans.

+++