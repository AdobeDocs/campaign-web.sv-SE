---
audience: end-user
title: Kampanjrapporter för push-kanalen
description: Förstå kampanjrapporter för Push-kanalen
badge: label="Beta"
source-git-commit: 72a7cb2577512b9b3dbf239ca664aa8410918ba2
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Kampanjrapporter för push-kanalen {#campaign-reports-push-channel}

Varje kampanjrapport är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel. Rapporterna och mätvärdena för push-kanalen beskrivs nedan. Lär dig hur du får tillgång till dina kampanjrapporter i [den här sidan](campaign-reports.md).

## Leveranssammanfattning {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Leveransöversikt"
>abstract="The **Leveransöversikt** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med leverans av push-meddelanden."

The **[!UICONTROL Delivery Overview]** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med leverans av push-meddelanden. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-summary.png)


+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Total sent]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Total clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

### Inledande målgruppsstatistik {#delivery-summary-push-initial-target}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Inledande målgruppsstatistik"
>abstract="The **Inledande målgruppsstatistik** tabellen visar data som är relativa till dina mottagare"

The **[!UICONTROL Initial target audience statistics]** tabellen visar data som är relativa till mottagarna. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-target.png)


+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista osv.

+++

### Körningsstatistik {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Körningsstatistik"
>abstract="The **Körningsstatistik** tabellen visar hur framgångsrik leveransen är: meddelanden som ska levereras, lyckade resultat, fel och nya karantän."

The **[!UICONTROL Execution statistics]** tabellen visar hur bra leveransen är. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-exec.png)


+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (ogiltig registrering, avvisning av meddelande, nyttolastfel, till exempel) i förhållande till antalet meddelanden som ska levereras.

  Feltyperna för push-meddelanden visas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Genererade klickströmmar {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Genererade klickströmmar"
>abstract="The **Genererade klickströmmar** tabellen visar tillgängliga data i relation till hur mottagarna interagerade med leveransen."

The **[!UICONTROL Generated click streams]** tabellen visar data som är relativa till hur mottagarna interagerade med leveransen. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-clicks.png)

+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Unique clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Total clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat i en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

+++
