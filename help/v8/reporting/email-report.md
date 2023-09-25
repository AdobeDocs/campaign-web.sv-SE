---
audience: end-user
title: Leveransrapporter via e-post
description: Lär dig hur du får tillgång till och använder e-postleveransrapporter
badge: label="Beta"
source-git-commit: f2ae73ce56e2e5128fecd8b74a6bdb096b8b75ec
workflow-type: tm+mt
source-wordcount: '2082'
ht-degree: 0%

---

# Rapport om e-postleverans {#email-report}

The **Rapport om e-postleverans** erbjuder omfattande insikter och data som är specifika för e-postkanalen. Den ger detaljerad information om prestanda, effektivitet och resultat för era individuella leveranser och ger er en heltäckande översikt.

## Leveranssammanfattning {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Rapportsändning"
>abstract="han **Skickar** i rapporten ger djupgående insikter om besökarnas interaktion med era leveranser och eventuella fel som de har upptäckt."

### Inledande målpopulation {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Inledande målpopulation"
>abstract="The **Inledande målpopulation** I diagrammet visas data i förhållande till dina mottagare och meddelanden, baserat på resultatet av leveransförberedelsen."

The **[!UICONTROL Initial target population]** I diagrammet visas data relativt dina mottagare. Mätvärden beräknas under färdigställandet av leveransen och visar: den initiala målgruppen, antalet meddelanden som ska skickas, antalet exkluderade mottagare.

![](assets/reporting_email_1.png){align="center" zoomable="yes"}

För musen över en del av diagrammet för att visa det exakta talet.

![](assets/reporting_email_1.1.png){align="center" zoomable="yes"}


+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL To deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal mottagare exkluderade från målpopulationen.
+++

### Leveransstatistik {#email-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Leveransstatistik"
>abstract="The **Leveransstatistik** diagram visar hur framgångsrik leveransen är och vilka fel som har inträffat."


The **[!UICONTROL Delivery statistics]** diagram visar hur framgångsrik leveransen är. Mätvärdena anges nedan.

![](assets/reporting_email_2.png){align="center" zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Message sent]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

### Orsaker till uteslutning  {#email-delivery-exclusions}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Leveransstatistik"
>abstract="The **Orsaker till uteslutning** diagram och tabell visar uppdelningen per regel för meddelanden som avvisats under leveransförberedelsen."


The **[!UICONTROL Causes of exclusion]** diagram och tabell visar uppdelningen per regel för meddelanden som avvisats under leveransförberedelsen. Exkluderingsregler finns i [Kampanjdokumentation v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/reporting_email_3.png){align="center" zoomable="yes"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL User unknown]**: Feltyp som genererades under leveransen för att ange att e-postadressen är ogiltig.

* **[!UICONTROL Invalid domain]**: Feltyp som genereras när en leverans skickas för att ange att domänen för e-postadressen är fel eller inte finns.

* **[!UICONTROL Mailbox full]**: Feltyp som genererats efter fem leveransförsök för att ange att mottagarens inkorg innehåller för många meddelanden.

* **[!UICONTROL Account disabled]**: Feltyp som genereras när en leverans skickas för att ange att adressen inte längre finns.

* **[!UICONTROL Refused]**: Feltyp som genereras när en adress nekas av IAP (Internet Access Provider), till exempel efter att en säkerhetsregel (antispam-program) har tillämpats.

* **[!UICONTROL Unreachable]**: Feltyp som inträffar i meddelandedistributionssträngen: incident i SMTP-reläet, domän som inte går att nå temporärt, osv.

* **[!UICONTROL Not connected]**: Feltyp som anger att mottagarens mobiltelefon är avstängd eller frånkopplad från nätverket vid tidpunkten för sändningen.

+++

## Leveranskapacitet {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Widget för leveransgenomströmning"
>abstract="The **Leveransflöde** rapporten innehåller detaljerad information om hela plattformens leveransflöde inom en angiven tidsram."

Den här rapporten innehåller detaljerad information om hela plattformens leveransflöde inom en angiven tidsram. Det primära måttet som används för att mäta hastigheten för meddelandeleverans är antalet meddelanden som skickas per timme.

![](assets/reporting_email_3.1.png){align="center" zoomable="yes"}


## Sändningsstatistik {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Widget för sändningsstatistik"
>abstract="The **Sändningsstatistik** rapporten innehåller tillgängliga data för eventuella fel som påträffats i varje domän."

The **[!UICONTROL Broadcast statistics]** tabellen innehåller tillgängliga data för eventuella fel som påträffats i varje domän. Mätvärdena anges nedan.

![](assets/reporting_email_4.png){align="center" zoomable="yes"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Processed emails]**: Totalt antal meddelanden som har bearbetats av leveransservern.

* **[!UICONTROL Delivered]**: Procentandel av antalet meddelanden som har bearbetats jämfört med det totala antalet bearbetade meddelanden.

* **[!UICONTROL Hard bounces]**: Procentandel av antalet&quot;hårda&quot; studsar, permanenta fel, t.ex. fel e-postadress, jämfört med det totala antalet bearbetade meddelanden.

* **[!UICONTROL Soft bounces]**: Procentandel av antalet &quot;mjuka&quot; studsar, tillfälliga fel som en fullständig inkorg, jämfört med det totala antalet bearbetade meddelanden

* **[!UICONTROL Opens]**: Procentandel av antalet målmottagare som öppnade ett meddelande minst en gång jämfört med antalet meddelanden som bearbetades.

* **[!UICONTROL Clicks]**: Procentandel av antalet personer som klickade i en leverans minst en gång jämfört med antalet meddelanden som bearbetades.

* **[!UICONTROL Unsubscriptions]**: Procentandel av antalet klick på en länk för att avbryta prenumerationen jämfört med antalet meddelanden som har bearbetats.
+++

## Ej levererbara {#non-deliverables-email}

### Uppdelning av fel per typ {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Uppdelning av fel per typ"
>abstract="The **Uppdelning av fel per typ** tabellen och diagrammet innehåller tillgängliga data för varje feltyp som påträffas: okänd användare, postlåda full, ogiltig domän med mera."

The **[!UICONTROL Breakdown of errors per type]** tabellen och diagrammet innehåller tillgängliga data för feltypen. Mätvärdena anges nedan.

Felen som visas i den här rapporten utlöser karantänprocessen. Mer information om karantänhantering finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

![](assets/campaign_report_email_6.png){align="left" zoomable="yes"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL User unknown]**: Feltyp som genererades under leveransen för att ange att e-postadressen är ogiltig.

* **[!UICONTROL Invalid domain]**: Feltyp som genereras när en leverans skickas för att ange att domänen för e-postadressen är fel eller inte finns.

* **[!UICONTROL Mailbox full]**: Feltyp som genererats efter fem leveransförsök för att ange att mottagarens inkorg innehåller för många meddelanden.

* **[!UICONTROL Account disabled]**: Feltyp som genereras när en leverans skickas för att ange att adressen inte längre finns.

* **[!UICONTROL Refused]**: Feltyp som genereras när en adress nekas av IAP (Internet Access Provider), till exempel efter att en säkerhetsregel (antispam-program) har tillämpats.

* **[!UICONTROL Unreachable]**: Feltyp som inträffar i meddelandedistributionssträngen: incident i SMTP-reläet, domän som inte går att nå temporärt, osv.

* **[!UICONTROL Not connected]**: Feltyp som anger att mottagarens mobiltelefon är avstängd eller frånkopplad från nätverket vid tidpunkten för sändningen.

+++


### Uppdelning av fel per domän {#email-delivery-breakdown-domain}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Uppdelning av fel per domän"
>abstract="The **Uppdelning av fel per domän** tabellen och diagrammet visar tillgängliga data för varje feltyp som påträffas beroende på varje domän."


The **[!UICONTROL Breakdown of errors per domain]** tabellen och diagrammet visar tillgängliga data för eventuella fel som påträffats i varje domän.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Klicka på ikonen bredvid namnet på varje domän för att se information.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Tillgängliga mått är samma som för [Uppdelning av fel efter typ](#email-delivery-breakdown-type) som beskrivs ovan.

## Spårningsindikatorer {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Rapporteringsspårning"
>abstract="The **Spårning** -fliken i rapporten innehåller värdefulla data, inklusive mottagarnas beteende per länk, hur öppningar och klickningar visas samt detaljerad information om de URL:er som klickas oftast under en leverans."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Widgeten Öppna och klickfrekvens"
>abstract="The **Öppnings- och klickfrekvens** tabellen visar data som är relativa till mottagarnas engagemang i leveransen."

### Leveransstatistik  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Leveransstatistik"
>abstract="The **Leveransstatistik** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om data som är tillgängliga för skickade e-postmeddelanden: lyckade, öppnade, klickade med mera."


The **[!UICONTROL Delivery statistics]** rapporten innehåller nyckeltal (KPI) som ger detaljerad information om data som är tillgängliga för skickade e-postmeddelanden. Mätvärdena anges nedan.

![](assets/reporting_email_5.png){align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Distinct opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Clicks on the opt-out link]**: Antal klick på länken för att avbryta prenumerationen.

* **[!UICONTROL Clicks on the mirror link]**: Antal klick på länken till spegelsidan.

* **[!UICONTROL Estimation of forwards]**: Uppskattning av antalet e-postmeddelanden som vidarebefordras av målmottagarna.
+++

### Öppnings- och klickfrekvens {#email-tracking-click-through}

The **[!UICONTROL Open and click-through rate]** tabellen visar data som är relativa till mottagarna. Mätvärdena anges nedan.

![](assets/reporting_email_6.png){align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Sent]**: Totalt antal skickade meddelanden.

* **[!UICONTROL Complaints]**: Antal meddelanden för den här domänen som har rapporterats som oönskade av mottagaren.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Clicks]**: Antal distinkta mottagare som klickat på samma leverans minst en gång.

* **[!UICONTROL Raw reactivity]**: Procentandel av antalet mottagare som klickade på en leverans minst en gång jämfört med antalet mottagare som öppnade en leverans minst en gång.
+++

## URL:er och klickströmmar {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL:er och klicka på strömwidgeten"
>abstract="The **URL:er och klickbara strömmar** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som användaren klickade mest på under en leverans."

* The **[!UICONTROL URLs and click streams]** rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som användaren klickade mest på under en leverans.

  ![](assets/reporting_email_7.png){align="center"}

  +++Läs mer om mätvärden för e-postleveransrapporter.

   * **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat i en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

   * **[!UICONTROL Platform average]** : Detta medelvärde, som visas för varje frekvens (reaktivitet, distinkta klick och kumulerade klick), beräknas för leveranser som skickats under de senaste sex månaderna. Endast leveranser med samma typologi och i samma kanal beaktas. Korrektur ingår inte.

+++

* **[!UICONTROL Top 10 most visited links]** diagram och tabell innehåller tillgängliga data för mottagarnas beteende per länk.

  ![](assets/reporting_email_8.png){align="center"}

  +++Läs mer om mätvärden för e-postleveransrapporter.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

   * **[!UICONTROL Percentage]**: Procentandel användare som interagerade med leveransen.

+++

* **[!UICONTROL Breakdown of clicks over time]** diagrammet innehåller tillgängliga data för mottagarnas beteende per länk.

  ![](assets/reporting_email_9.png){align="center"}

## Användaraktiviteter {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widgeten Användaraktiviteter"
>abstract="The **Användaraktiviteter** I diagrammet visas hur öppningar och klickningar delas upp i form av ett diagram. Du kan välja tidsperioden för måldata: sista dagen eller timmen eller 30 minuter."

The **[!UICONTROL User activities]** rapporten visar hur öppningar och klickningar i form av ett diagram är uppdelade. Du kan välja tidsperioden för måldata: sista dagen eller timmen eller 30 minuter.

![](assets/reporting_email_10.png){align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++

## Spårningsstatistik {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Widgeten Spårningsstatistik"
>abstract="The **Spårningsstatistik** diagram visar statistik om öppningar och klickningar. Du kan välja en specifik tidsram för måldata."

The **[!UICONTROL Tracking Statistics]** diagram visar statistik om öppningar och klickningar. Du kan välja en specifik tidsram för måldata.

![](assets/reporting_email_11.png){align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++

## Indelning av öppningar {#breakdown-opens}


### Uppdelning av öppningar efter enhet {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Uppdelning efter enhet"
>abstract="The **Uppdelning efter enhet** rapporten visar hur öppningar per enhet har fördelats för perioden. För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje enhetstyp."

The **Uppdelning efter enhet** rapporten visar hur öppningar per enhet har fördelats under perioden: persondatorer, Android-enheter, Apple-enheter eller andra.

För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje enhetstyp.

![](assets/reporting_email_13.png){align="center"}


### Uppdelning av öppningar efter operativsystem {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Uppdelning efter operativsystem"
>abstract="The **Uppdelning efter operativsystem** rapporten visar hur öppningarna fördelats på operativsystem för den berörda perioden. I det första diagrammet visas statistik för öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje operativsystem."

The **Uppdelning efter operativsystem** rapporten visar hur öppningarna fördelats på operativsystem under perioden: Windows-system, Android-system, iOS-system eller andra.

För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila operativsystem. Den andra visar det exakta antalet och procentandelen för varje operativsystem.

![](assets/reporting_email_13.1.png){align="center"}

### Uppdelning av öppningar efter webbläsare {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Uppdelning efter webbläsare"
>abstract="The **Uppdelning efter webbläsare** visar hur öppningar uppdelas efter webbläsare för perioden. I det första diagrammet visas statistik för öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje webbläsare."

The **Uppdelning efter webbläsare** rapporten visar hur öppningarna ser ut i olika webbläsare: Chrome, Safari, Internet Explorer med flera.

För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila operativsystem. Den andra visar det exakta antalet och procentandelen för varje webbläsare.

![](assets/reporting_email_13.2.png){align="center"}


## Klickningar {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Rapport om klickningar"
>abstract="The **Klickningar** I rapporten visas e-postinnehållet (HTML och/eller text) med procentandelen klickningar på länkar för varje länk. Personaliseringsblock, ej prenumerationslänkar, spegelsideslänkar och erbjudandelänkar tas med i det totala antalet klickningar, men visas inte i rapporten."

Den här rapporten visar meddelandeinnehållet (HTML och/eller text) med procentandelen klickningar på länkar för varje länk. Personaliseringsblock, ej prenumerationslänkar, spegelsideslänkar och erbjudandelänkar tas med i det totala antalet klickningar, men visas inte i rapporten.

![](assets/reporting11.png)
