---
audience: end-user
title: Kampanjrapporter för e-postkanalen
description: Läs mer om kampanjrapporter för e-postkanalen
badge: label="Begränsad tillgänglighet"
exl-id: c44c91f8-1f88-4087-8417-34be64a2ab19
source-git-commit: ac9a7918045e7ff02ef27c348b28a6ce09802caf
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# Kampanjrapporter för e-postkanalen {#campaign-reports-email-channel}

Varje kampanjrapport är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel. Rapporter och mätvärden för e-postkanalen anges nedan. Lär dig hur du får tillgång till dina kampanjrapporter i [den här sidan](campaign-reports.md).

## Leveranssammanfattning {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Leveransöversikt"
>abstract="The **Leveransöversikt** innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om hur besökarna interagerar med e-postleveransen."

### Leveransöversikt {#delivery-summary-email-ovv}

The **[!UICONTROL Delivery Overview]** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med e-postleveransen. Mätvärdena anges nedan.

![](assets/campaign_report_email_1.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Bounces]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Total opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Total clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

### Inledande målgruppsstatistik {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Inledande målgruppsstatistik"
>abstract="Den första målgruppsstatistiktabellen visar data relativt dina mottagare"

The **[!UICONTROL Initial target audience statistics]** tabellen visar data som är relativa till mottagarna. Mätvärdena anges nedan.

![](assets/campaign_report_email_2.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista osv.

+++

### Körningsstatistik {#delivery-summary-email-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_exec_stats"
>title="Körningsstatistik"
>abstract="The **Körningsstatistik** tabellen visar hur framgångsrik leveransen är: meddelanden som ska levereras, lyckade resultat, fel och nya karantän."

The **[!UICONTROL Execution statistics]** tabellen visar hur bra leveransen är. Mätvärdena anges nedan.

![](assets/campaign_report_email_3.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

  E-postfeltyperna listas i [Adobe Campaign v8-dokumentation (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

+++

### Reaktionsstatistik {#delivery-summary-email-reaction-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_reaction_stats"
>title="Reaktionsstatistik"
>abstract="The **Reaktionsstatistik** tabellen visar tillgängliga data för mottagaraktivitet för leveransen: antal öppningar, prenumerationer, avbeställningar, klicka för att spegla sidlänken."

The **[!UICONTROL Reaction statistics]** tabellen innehåller tillgängliga data för mottagaraktivitet för leveransen. Mätvärdena anges nedan.

![](assets/campaign_report_email_4.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Unique opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Total Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Unsubscriptions]**: Antal mottagare som klickat på att avbryta prenumerationen för den aktuella perioden.

* **[!UICONTROL Mirror page]**: Antal mottagare som klickade på länken för spegelsidan.

* **[!UICONTROL Forwards]**: Antal mottagare som klickade och som vidarebefordrat e-postmeddelandet.
+++

### Genererade klickströmmar {#delivery-summary-email-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_click_streams"
>title="Genererade klickströmmar"
>abstract="The **Genererade klickströmmar** tabellen visar tillgängliga data i relation till hur mottagarna interagerade med leveransen."

The **[!UICONTROL Generated click streams]** tabellen visar data som är relativa till hur mottagarna interagerade med leveransen. Mätvärdena anges nedan.

![](assets/campaign_report_email_5.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Unique clicks]**: Totalt antal unika mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Total Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat i en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

+++

## Ej levererbara {#non-deliverables-email}

### Uppdelning av fel per typ {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_type"
>title="Uppdelning av fel per typ"
>abstract="The **Uppdelning av fel per typ** tabellen och diagrammet innehåller tillgängliga data för varje feltyp som påträffas: okänd användare, postlåda full, ogiltig domän med mera."

The **[!UICONTROL Breakdown of errors per type]** tabellen och diagrammet innehåller tillgängliga data för eventuella fel som påträffats för varje typ av domän. Mätvärdena anges nedan.

Felen som visas i den här rapporten utlöser karantänprocessen. Mer information om karantänhantering finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

![](assets/campaign_report_email_6.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

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
>id="acw_campaign_reporting_error_domain"
>title="Uppdelning av fel per domän"
>abstract="The **Uppdelning av fel per domän** tabellen och diagrammet visar tillgängliga data för varje feltyp som påträffas beroende på varje domän."

The **[!UICONTROL Breakdown of errors per domain]** tabellen och diagrammet innehåller tillgängliga data för eventuella fel som påträffats i varje domän. Mätvärdena är gemensamma med **[!UICONTROL Breakdown of errors per type]** tabellen och diagrammet som anges ovan.

## Spårningsindikatorer {#tracking-indicators-email}

### Leveransstatistik {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_delivery_statistics_summary"
>title="Leveransstatistik"
>abstract="The **Leveransstatistik** diagram visar hur framgångsrik leveransen är och vilka fel som har inträffat."

The **[!UICONTROL Delivery statistics]** Mätvärden ger nyckeltal (KPI) som ger detaljerad information om data som är tillgängliga för skickade e-postmeddelanden. Mätvärdena anges nedan.

![](assets/campaign_report_email_7.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Message(s) to deliver]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Unique opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Total Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Clicks on the opt-out link]**: Antal klick på länken för att avbryta prenumerationen.

* **[!UICONTROL Clicks on the mirror link]**: Antal klick på länken till spegelsidan.

* **[!UICONTROL Estimation of forwards]**: Uppskattning av antalet e-postmeddelanden som vidarebefordras av målmottagarna.
+++

### Öppen och klickbar frekvens {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_open_clickthrough"
>title="Öppnings- och klickfrekvens"
>abstract="The **Öppnings- och klickfrekvens** tabellen visar data som är relativa till mottagarnas engagemang i leveransen."

The **[!UICONTROL Open and click-trough rate]** tabellen visar data som är relativa till mottagarna. Mätvärdena anges nedan.

![](assets/campaign_report_email_8.png)

+++ Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Sent]**: Totalt antal skickade meddelanden.

* **[!UICONTROL Complaints]**: Antal och procentandel meddelanden för den här domänen som har rapporterats som oönskade av mottagaren.

* **[!UICONTROL Unique Opens]**: Antal och procentandel distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Unique Clicks]**: Antal och procentandel av distinkta målmottagare som klickade på samma leverans minst en gång.

* **[!UICONTROL Raw reactivity]**: Procentandel av antalet mottagare som klickade på en leverans minst en gång jämfört med antalet mottagare som öppnade en leverans minst en gång.

+++

## URL:er och klickströmmar {#url-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams"
>title="URL:er och klickströmmar"
>abstract="The **URL:er och klickbara strömmar** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som användaren klickade mest på under en leverans."

The **[!UICONTROL URLs and click streams]** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som användaren klickade mest på under en leverans. Mätvärdena anges nedan.

![](assets/campaign_report_email_9.png)

+++ Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat i en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

* **[!UICONTROL Unique clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Total Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Platform average]** : Detta medelvärde, som visas för varje frekvens (reaktivitet, distinkta klick och kumulerade klick), beräknas för leveranser som skickats under de senaste sex månaderna. Endast leveranser med samma typologi och i samma kanal beaktas. Korrektur ingår inte.

+++

### De tio mest besökta länkarna {#top10-campaign-report-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams_top10"
>title="De tio mest besökta länkarna"
>abstract="The **De tio mest besökta länkarna** diagram och tabell innehåller tillgängliga data för mottagarnas beteende per länk."

The **[!UICONTROL Top 10 most visited links]** diagram och tabell innehåller tillgängliga data för mottagarnas beteende per länk. Mätvärdena anges nedan.

![](assets/campaign_report_email_10.png)

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Percentage]**: Procentandel användare som interagerade med leveransen.

+++

### Klicknedbrytning över tid {#campaign-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_urls_click_breakdown"
>title="Klicknedbrytning över tid"
>abstract="The **Klicknedbrytning över tid** diagram visar tillgängliga data för mottagarnas beteende per länk."

The **[!UICONTROL Breakdown of clicks over time]** diagrammet innehåller tillgängliga data för mottagarnas beteende per länk.

![](assets/campaign_report_email_11.png)

## Användaraktiviteter {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_user_activities"
>title="Användaraktiviteter"
>abstract="The **Användaraktiviteter** I diagrammet visas hur öppningar och klickningar delas upp i form av ett diagram."

The **[!UICONTROL User activities]** rapporten visar hur öppningar och klickningar i form av ett diagram är uppdelade. Mätvärden för den här rapporten finns nedan.

![](assets/campaign_report_email_user_activities.png){align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++
