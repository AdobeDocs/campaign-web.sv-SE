---
audience: end-user
title: Kampanjrapporter för push-kanalen
description: Förstå kampanjrapporter för Push-kanalen
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Kampanjrapporter för push-kanalen {#campaign-reports-push-channel}

Varje kampanjrapport är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel. Rapporterna och mätvärdena för push-kanalen beskrivs nedan. Lär dig hur du får åtkomst till dina kampanjrapporter på [den här sidan](campaign-reports.md).

## Leveranssammanfattning {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Leveransöversikt"
>abstract="Rapporten **Leveransöversikt** innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med leveransen av push-meddelanden."

Rapporten **[!UICONTROL Delivery Overview]** innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med leveransen av push-meddelanden. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-summary.png){zoomable="yes"}


+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbearbetning i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Total clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

### Inledande målgruppsstatistik {#delivery-summary-push-initial-target}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Inledande målgruppsstatistik"
>abstract="Tabellen **Inledande målgruppsstatistik** visar data i förhållande till dina mottagare"

Tabellen **[!UICONTROL Initial target audience statistics]** visar data i förhållande till dina mottagare. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-target.png){zoomable="yes"}


+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista, osv.

+++

### Körningsstatistik {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Körningsstatistik"
>abstract="Tabellen **Körningsstatistik** visar hur din leverans lyckades: meddelanden som ska levereras, slutföras, fel och nya karantän."

Tabellen **[!UICONTROL Execution statistics]** innehåller information om leveransframgången. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-exec.png){zoomable="yes"}

+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter en misslyckad leverans (ogiltig registrering, avvisning av meddelande, nyttolastfel, till exempel) i förhållande till antalet meddelanden som ska levereras.

  Feltyper för push-meddelanden visas i [Adobe Campaign v8-dokumentationen (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Genererade klickströmmar {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Genererade klickströmmar"
>abstract="Tabellen **Genererade klickströmmar** visar tillgängliga data i relation till hur mottagarna interagerade med leveransen."

Tabellen **[!UICONTROL Generated click streams]** visar data i relation till hur mottagarna interagerade med leveransen. Mätvärdena anges nedan.

![](assets/campaign-reporting-push-clicks.png){zoomable="yes"}

+++Läs mer om mätvärden för push-kampanjrapporter.

* **[!UICONTROL Unique clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Total clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som har klickat i en leverans och det beräknade antalet målmottagare som har öppnat en leverans.

+++
