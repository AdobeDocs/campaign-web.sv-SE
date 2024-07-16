---
audience: end-user
title: Kampanjrapporter för e-postkanalen
description: Läs mer om kampanjrapporter för e-postkanalen
exl-id: c44c91f8-1f88-4087-8417-34be64a2ab19
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '1432'
ht-degree: 0%

---

# Kampanjrapporter för e-postkanalen {#campaign-reports-email-channel}

Varje kampanjrapport är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel. Rapporter och mätvärden för e-postkanalen anges nedan. Lär dig hur du får åtkomst till dina kampanjrapporter på [den här sidan](campaign-reports.md).

## Leveranssammanfattning {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Leveransöversikt"
>abstract="**Leveransöversikt** innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om hur besökarna interagerar med e-postleveransen."

### Leveransöversikt {#delivery-summary-email-ovv}

Rapporten **[!UICONTROL Delivery Overview]** innehåller nyckeltal (KPI:er) som ger detaljerad information om hur besökarna interagerar med e-postleveransen. Mätvärdena anges nedan.

![](assets/campaign_report_email_1.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

* **[!UICONTROL Bounces]**: Totalt antal fel som har ackumulerats under leverans och automatisk returbearbetning i relation till totalt antal skickade meddelanden.

* **[!UICONTROL Total opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Total clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

### Inledande målgruppsstatistik {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Inledande målgruppsstatistik"
>abstract="Den första målgruppsstatistiktabellen visar data i förhållande till dina mottagare."

Tabellen **[!UICONTROL Initial target audience statistics]** visar data i förhållande till dina mottagare. Mätvärdena anges nedan.

![](assets/campaign_report_email_2.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress som saknas, är i karantän, på blockeringslista, osv.

+++

### Körningsstatistik {#delivery-summary-email-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_exec_stats"
>title="Körningsstatistik"
>abstract="Tabellen **Körningsstatistik** visar hur din leverans lyckades: meddelanden som ska levereras, slutföras, fel och nya karantän."

Tabellen **[!UICONTROL Execution statistics]** innehåller information om leveransframgången. Mätvärdena anges nedan.

![](assets/campaign_report_email_3.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter en misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

  E-postfeltyperna listas i [Adobe Campaign v8-dokumentationen (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

+++

### Reaktionsstatistik {#delivery-summary-email-reaction-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_reaction_stats"
>title="Reaktionsstatistik"
>abstract="Tabellen **Reaktionsstatistik** visar tillgängliga data för mottagaraktivitet för leveransen: antal öppningar, prenumerationer, prenumerationer, prenumerationer, klicka för att spegla sidlänken."

Tabellen **[!UICONTROL Reaction statistics]** innehåller tillgängliga data för mottagaraktivitet för din leverans. Mätvärdena anges nedan.

![](assets/campaign_report_email_4.png){zoomable="yes"}

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
>abstract="Tabellen **Genererade klickströmmar** visar tillgängliga data i relation till hur mottagarna interagerade med leveransen."

Tabellen **[!UICONTROL Generated click streams]** visar data i relation till hur mottagarna interagerade med leveransen. Mätvärdena anges nedan.

![](assets/campaign_report_email_5.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Unique clicks]**: Totalt antal unika mottagare som klickat i en leverans minst en gång.

* **[!UICONTROL Total Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som har klickat i en leverans och det beräknade antalet målmottagare som har öppnat en leverans.

+++

## Ej levererbara {#non-deliverables-email}

### Uppdelning av fel per typ {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_type"
>title="Uppdelning av fel per typ"
>abstract="**Uppdelningen av fel per typ**-tabell och diagram innehåller tillgängliga data för varje feltyp som påträffas: okänd användare, postlåda full, ogiltig domän med mera."

Tabellen och diagrammet **[!UICONTROL Breakdown of errors per type]** innehåller tillgängliga data för eventuella fel som påträffats för varje typ av domän. Mätvärdena anges nedan.

Felen som visas i den här rapporten utlöser karantänprocessen. Mer information om karantänhantering finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

![](assets/campaign_report_email_6.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL User unknown]**: Feltypen som genererades under leveransen indikerar att e-postadressen är ogiltig.

* **[!UICONTROL Invalid domain]**: Feltypen som genererades när en leverans skickades för att ange att domänen för e-postadressen är fel eller inte finns.

* **[!UICONTROL Mailbox full]**: Feltypen som genererades efter fem leveransförsök för att ange att mottagarens inkorg innehåller för många meddelanden.

* **[!UICONTROL Account disabled]**: Feltypen som genererades när en leverans skickades för att ange att adressen inte längre finns.

* **[!UICONTROL Refused]**: Feltypen som genereras när en adress nekas av IAP (Internet Access Provider), till exempel efter att en säkerhetsregel (antispam-programvara) har använts.

* **[!UICONTROL Unreachable]**: Feltyp som inträffar i meddelandedistributionssträngen: incident i SMTP-reläet, domän som inte går att nå temporärt, osv.

* **[!UICONTROL Not connected]**: Feltyp som indikerar att mottagarens mobiltelefon är avstängd eller frånkopplad från nätverket när den skickas.

+++

### Uppdelning av fel per domän {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_domain"
>title="Uppdelning av fel per domän"
>abstract="Tabellen **Uppdelning av fel per domän** och diagrammet visar tillgängliga data för varje feltyp som påträffas beroende på varje domän."

Tabellen och diagrammet **[!UICONTROL Breakdown of errors per domain]** innehåller tillgängliga data för eventuella fel som påträffats i varje domän. Mätvärdena är gemensamma för tabellen **[!UICONTROL Breakdown of errors per type]** och diagrammet som anges ovan.

## Spårningsindikatorer {#tracking-indicators-email}

### Leveransstatistik {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_delivery_statistics_summary"
>title="Leveransstatistik"
>abstract="Diagrammet **Leveransstatistik** visar om leveransen lyckades och om fel uppstod."

Måtten **[!UICONTROL Delivery statistics]** innehåller nyckeltal (KPI:er) som ger detaljerad information om tillgängliga data för skickade e-postmeddelanden. Mätvärdena anges nedan.

![](assets/campaign_report_email_7.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Message(s) to deliver]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Unique opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Total Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Clicks on the opt-out link]**: Antal klick på länken för att avbryta prenumerationen.

* **[!UICONTROL Clicks on the mirror link]**: Antal klick på länken till spegelsidan.

* **[!UICONTROL Estimation of forwards]**: Uppskattning av antalet e-postmeddelanden som vidarebefordrats av målmottagarna.
+++

### Öppen och klickbar frekvens {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_open_clickthrough"
>title="Öppnings- och klickfrekvens"
>abstract="Tabellen **Öppen och klickfrekvens** visar data i relation till mottagarnas engagemang i leveransen."

Tabellen **[!UICONTROL Open and click-trough rate]** visar data i förhållande till dina mottagare. Mätvärdena anges nedan.

![](assets/campaign_report_email_8.png){zoomable="yes"}

+++ Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Sent]**: Totalt antal skickade meddelanden.

* **[!UICONTROL Complaints]**: Antal och procentandel meddelanden för den här domänen som har rapporterats som oönskade av mottagaren.

* **[!UICONTROL Unique Opens]**: Antal och procentandel distinkta mottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Unique Clicks]**: Antal och procentandel distinkta målmottagare som klickade i samma leverans minst en gång.

* **[!UICONTROL Raw reactivity]**: Procentandel av antalet mottagare som klickade i en leverans minst en gång jämfört med antalet mottagare som öppnade en leverans minst en gång.

+++

## URL:er och klickströmmar {#url-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams"
>title="URL:er och klickströmmar"
>abstract="**URL:er och klickningsströmmar**-rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som klickades mest under en leverans."

Rapporten **[!UICONTROL URLs and click streams]** innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som du klickade mest på under en leverans. Mätvärdena anges nedan.

![](assets/campaign_report_email_9.png){zoomable="yes"}

+++ Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som har klickat i en leverans och det beräknade antalet målmottagare som har öppnat en leverans.

* **[!UICONTROL Unique clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Total Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Platform average]** : Detta medelvärde, som visas under varje frekvens (reaktivitet, distinkta klick och kumulerade klick), beräknas för leveranser som skickats under de senaste sex månaderna. Endast leveranser med samma typologi och i samma kanal beaktas. Korrektur ingår inte.

+++

### De tio mest besökta länkarna {#top10-campaign-report-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams_top10"
>title="De tio mest besökta länkarna"
>abstract="Diagrammet och tabellen **Top 10 most visit links** innehåller tillgängliga data för mottagarnas beteende per länk."

Diagrammet och tabellen **[!UICONTROL Top 10 most visited links]** innehåller tillgängliga data för mottagarnas beteende per länk. Mätvärdena anges nedan.

![](assets/campaign_report_email_10.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Percentage]**: Procentandel användare som interagerade med leveransen.

+++

### Klicknedbrytning över tid {#campaign-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_urls_click_breakdown"
>title="Klicknedbrytning över tid"
>abstract="Diagrammet **Klicknedbrytning över tid** visar tillgängliga data för mottagarens beteende per länk."

Diagrammet **[!UICONTROL Breakdown of clicks over time]** innehåller tillgängliga data för mottagarnas beteende per länk.

![](assets/campaign_report_email_11.png){zoomable="yes"}

## Användaraktiviteter {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_user_activities"
>title="Användaraktiviteter"
>abstract="Diagrammet **Användaraktiviteter** visar hur öppningar och klick delas upp i ett diagram."

Rapporten **[!UICONTROL User activities]** visar uppdelningen av öppningar och klick i form av ett diagram. Mätvärden för den här rapporten finns nedan.

![](assets/campaign_report_email_user_activities.png){zoomable="yes"}{align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++
