---
audience: end-user
title: Kampanjrapporter för SMS-kanalen
description: Förstå kampanjrapporter för SMS-kanalen
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Kampanjrapporter för SMS-kanalen {#campaign-reports-sms-channel}

Varje kampanjrapport är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel. Rapporter och mätvärden för SMS-kanalen anges nedan. Lär dig hur du får tillgång till dina kampanjrapporter i [den här sidan](campaign-reports.md).

## Leveranssammanfattning {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Leveransöversikt"
>abstract="The **Leveransöversikt** rapporten innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om hur besökarna interagerar med SMS-leveransen."


The **[!UICONTROL Delivery Overview]** rapporten innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om hur besökarna interagerar med SMS-leveransen. Mätvärdena anges nedan.

![](assets/campaign_report_sms_1.png){zoomable=&quot;yes&quot;}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Total sent]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++


### Inledande målgruppsstatistik {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Inledande målgruppsstatistik"
>abstract="The **Inledande målgruppsstatistik** tabellen visar data som är relativa till dina mottagare"

The **[!UICONTROL Initial target audience statistics]** tabellen visar data som är relativa till mottagarna. Mätvärdena anges nedan.


![](assets/campaign_report_sms_2.png){zoomable=&quot;yes&quot;}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista osv.

+++


### Körningsstatistik {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Körningsstatistik"
>abstract="The **Körningsstatistik** tabellen visar hur framgångsrik leveransen är: meddelanden som ska levereras, lyckade resultat, fel och nya karantän."


The **[!UICONTROL Execution statistics]** tabellen visar hur bra leveransen är. Mätvärdena anges nedan.


![](assets/campaign_report_sms_3.png){zoomable=&quot;yes&quot;}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

  SMS-feltyper listas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Genererade klickströmmar {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Genererade klickströmmar"
>abstract="The **Genererade klickströmmar** tabellen visar tillgängliga data i relation till hur mottagarna interagerade med leveransen."

The **[!UICONTROL Generated click streams]** tabellen visar data som är relativa till hur mottagarna interagerade med leveransen. Mätvärdena anges nedan.

![](assets/campaign_report_sms_4.png){zoomable=&quot;yes&quot;}

+++Läs mer om mätvärden för SMS-kampanjrapporter.

* **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat i en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

+++
