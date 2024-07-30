---
audience: end-user
title: Leveransrapporter via e-post
description: Lär dig hur du får tillgång till och använder e-postleveransrapporter
exl-id: 2a0bd3e9-5d75-47c8-bd6a-b3e0b1ce0a01
source-git-commit: 39dcf11797339ee9800da6c5a32b1a1c3470529a
workflow-type: tm+mt
source-wordcount: '2165'
ht-degree: 0%

---

# Rapport om e-postleverans {#email-report}

**Rapporten om e-postleverans** innehåller omfattande insikter och data som är specifika för e-postkanalen. Den ger detaljerad information om prestanda, effektivitet och resultat för era individuella leveranser och ger er en heltäckande översikt.

## Leveranssammanfattning {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Rapportsändning"
>abstract="Fliken **Skickar** i din rapport ger djupgående insikter om besökarnas interaktioner med dina leveranser och eventuella fel som de har påträffat."

### Inledande målpopulation {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Inledande målpopulation"
>abstract="Diagrammet **Inledande målpopulation** visar data i förhållande till dina mottagare och meddelanden baserat på resultatet av leveransförberedelsen."

Diagrammet **[!UICONTROL Initial target population]** visar data i förhållande till dina mottagare. Mätvärden beräknas under färdigställandet av leveransen och visar: den initiala målgruppen, antalet meddelanden som ska skickas, antalet exkluderade mottagare.

![](assets/reporting_email_1.png){zoomable="yes"}

För musen över en del av diagrammet för att visa det exakta talet.

![](assets/reporting_email_1.1.png){zoomable="yes"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL To deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal mottagare exkluderade från målpopulationen.
+++

### Leveransstatistik {#email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Leveransstatistik"
>abstract="Diagrammet **Leveransstatistik** visar om leveransen lyckades och om fel uppstod."

Diagrammet **[!UICONTROL Delivery statistics]** visar om leveransen lyckades. Mätvärdena anges nedan.

![](assets/reporting_email_2.png){zoomable="yes"}

+++Läs mer om rapportstatistik för e-postkampanjer.

* **[!UICONTROL Message sent]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter en misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

### Orsaker till uteslutning  {#email-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Leveransorsaker"
>abstract="Diagrammet **Orsaker till uteslutning** och tabellen visar nedbrytningen per regel för meddelanden som avvisats under leveransförberedelsen."

Diagrammet **[!UICONTROL Causes of exclusion]** och tabellen visar detaljerna per regel för meddelanden som avvisats under leveransförberedelsen. Uteslutningsreglerna finns i dokumentationen för [Campaign v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/reporting_email_3.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL User unknown]**: Feltypen som genererades under leveransen indikerar att e-postadressen är ogiltig.

* **[!UICONTROL Invalid domain]**: Feltypen som genererades när en leverans skickades för att ange att domänen för e-postadressen är fel eller inte finns.

* **[!UICONTROL Mailbox full]**: Feltypen som genererades efter fem leveransförsök för att ange att mottagarens inkorg innehåller för många meddelanden.

* **[!UICONTROL Account disabled]**: Feltypen som genererades när en leverans skickades för att ange att adressen inte längre finns.

* **[!UICONTROL Refused]**: Feltypen som genereras när en adress nekas av IAP (Internet Access Provider), till exempel efter att en säkerhetsregel (antispam-programvara) har använts.

* **[!UICONTROL Unreachable]**: Feltyp som inträffar i meddelandedistributionssträngen: incident i SMTP-reläet, domän som inte går att nå temporärt, osv.

* **[!UICONTROL Not connected]**: Feltyp som indikerar att mottagarens mobiltelefon är avstängd eller frånkopplad från nätverket när den skickas.

+++

## Leveranskapacitet {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Leveranskapacitet"
>abstract="Rapporten **Leveransflöde** innehåller detaljerad information om hela plattformens leveransflöde inom en angiven tidsram."

Den här rapporten innehåller detaljerad information om hela plattformens leveransflöde inom en angiven tidsram. Det primära måttet som används för att mäta hastigheten för meddelandeleverans är antalet meddelanden som skickas per timme.

![](assets/reporting_email_3.1.png){zoomable="yes"}{align="center" zoomable="yes"}


## Sändningsstatistik {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Sändningsstatistik"
>abstract="Rapporten **Sändningsstatistik** innehåller tillgängliga data för eventuella fel som påträffats i varje domän."

Tabellen **[!UICONTROL Broadcast statistics]** innehåller tillgängliga data för eventuella fel som påträffats i varje domän. Mätvärdena anges nedan.

![](assets/reporting_email_4.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Processed emails]**: Totalt antal meddelanden som har bearbetats av leveransservern.

* **[!UICONTROL Delivered]**: Procentandel av antalet meddelanden som bearbetats jämfört med det totala antalet meddelanden som bearbetats.

* **[!UICONTROL Hard bounces]**: Procentandel av antalet &quot;hårda&quot; studsar, permanenta fel, t.ex. fel e-postadress, jämfört med det totala antalet bearbetade meddelanden.

* **[!UICONTROL Soft bounces]**: Procentandel av antalet &quot;mjuka&quot; studsar, tillfälliga fel som en fullständig inkorg, jämfört med det totala antalet bearbetade meddelanden

* **[!UICONTROL Opens]**: Procentandel av antalet målmottagare som öppnade ett meddelande minst en gång jämfört med antalet meddelanden som bearbetades.

* **[!UICONTROL Clicks]**: Procentandel av antalet personer som klickade i en leverans minst en gång jämfört med antalet meddelanden som bearbetades.

* **[!UICONTROL Unsubscriptions]**: Procentandel av antalet klickningar på en länk för att avbryta prenumerationen jämfört med antalet meddelanden som har bearbetats.
+++

## Ej levererbara {#non-deliverables-email}

### Uppdelning av fel per typ {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Uppdelning av fel per typ"
>abstract="**Uppdelningen av fel per typ** innehåller tillgängliga data för varje feltyp som påträffas: okänd användare, postlåda full, ogiltig domän med mera."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type_table"
>title="Uppdelning av fel per typ"
>abstract="Tabellen **Uppdelning av fel per typ** innehåller en omfattande beskrivning av förekomsten av varje feltyp."

Tabellen och diagrammet **[!UICONTROL Breakdown of errors per type]** innehåller tillgängliga data för feltypen. Mätvärdena anges nedan.

Felen som visas i den här rapporten utlöser karantänprocessen. Mer information om karantänhantering finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

![](assets/campaign_report_email_6.png){zoomable="yes"}{align="left" zoomable="yes"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL User unknown]**: Feltypen som genererades under leveransen indikerar att e-postadressen är ogiltig.

* **[!UICONTROL Invalid domain]**: Feltypen som genererades när en leverans skickades för att ange att domänen för e-postadressen är fel eller inte finns.

* **[!UICONTROL Mailbox full]**: Feltypen som genererades efter fem leveransförsök för att ange att mottagarens inkorg innehåller för många meddelanden.

* **[!UICONTROL Account disabled]**: Feltypen som genererades när en leverans skickades för att ange att adressen inte längre finns.

* **[!UICONTROL Refused]**: Feltypen som genereras när en adress nekas av IAP (Internet Access Provider), till exempel efter att en säkerhetsregel (antispam-programvara) har använts.

* **[!UICONTROL Unreachable]**: Feltyp som inträffar i meddelandedistributionssträngen: incident i SMTP-reläet, domän som inte går att nå temporärt, osv.

* **[!UICONTROL Not connected]**: Feltyp som indikerar att mottagarens mobiltelefon är avstängd eller frånkopplad från nätverket när den skickas.

+++

### Uppdelning av fel per domän {#email-delivery-breakdown-domain}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Uppdelning av fel per domän"
>abstract="Diagrammet **Uppdelning av fel per domän** visar tillgängliga data för varje feltyp som påträffas beroende på varje domän."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain_table"
>title="Uppdelning av fel per domän"
>abstract="Tabellen **Uppdelning av fel per domän** innehåller en omfattande beskrivning av förekomsten av varje fel beroende på vilken domän som används."

Tabellen och diagrammet **[!UICONTROL Breakdown of errors per domain]** visar tillgängliga data för eventuella fel som påträffats i varje domän.

![](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

Klicka på ikonen bredvid namnet på varje domän för att se information.

![](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

Tillgängliga mått är samma som för [uppdelningen av fel efter typ](#email-delivery-breakdown-type) som beskrivs ovan.

## Spårningsindikatorer {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Rapporteringsspårning"
>abstract="Fliken **Spårning** i rapporten innehåller värdefulla data, inklusive mottagarnas beteende per länk, information om öppningar och klickningar samt detaljerad information om de URL:er som du klickade mest på under en leverans."


### Leveransstatistik  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Leveransstatistik"
>abstract="Rapporten **Leveransstatistik** innehåller nyckeltal (KPI:er) som ger detaljerad information om data som är tillgängliga för skickade e-postmeddelanden: lyckade, öppnade, klickade med mera."


Rapporten **[!UICONTROL Delivery statistics]** innehåller nyckeltal (KPI:er) som ger detaljerad information om tillgängliga data för skickade e-postmeddelanden. Mätvärdena anges nedan.

![](assets/reporting_email_5.png){zoomable="yes"}{align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Distinct opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Clicks on the opt-out link]**: Antal klick på länken för att avbryta prenumerationen.

* **[!UICONTROL Clicks on the mirror link]**: Antal klick på länken till spegelsidan.

* **[!UICONTROL Estimation of forwards]**: Uppskattning av antalet e-postmeddelanden som vidarebefordrats av målmottagarna.
+++

### Öppnings- och klickfrekvens {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Öppnings- och klickfrekvens"
>abstract="Tabellen **Öppen och klickfrekvens** visar data i relation till mottagarnas engagemang i leveransen."



Tabellen **[!UICONTROL Open and click-through rate]** visar data i förhållande till dina mottagare. Mätvärdena anges nedan.

![](assets/reporting_email_6.png){zoomable="yes"}{align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Sent]**: Totalt antal skickade meddelanden.

* **[!UICONTROL Complaints]**: Antal meddelanden för den här domänen som har rapporterats som oönskade av mottagaren.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

* **[!UICONTROL Clicks]**: Antal distinkta målmottagare som klickade i samma leverans minst en gång.

* **[!UICONTROL Raw reactivity]**: Procentandel av antalet mottagare som klickade i en leverans minst en gång jämfört med antalet mottagare som öppnade en leverans minst en gång.
+++

## URL:er och klickströmmar {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL:er och klickströmmar"
>abstract="**URL:er och klickningsströmmar**-rapporten innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som klickades mest under en leverans."


Rapporten **[!UICONTROL URLs and click streams]** innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som du klickade mest på under en leverans.

![](assets/reporting_email_7.png){zoomable="yes"}{align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som har klickat i en leverans och det beräknade antalet målmottagare som har öppnat en leverans.

* **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Platform average]**: Den här genomsnittliga hastigheten, som visas under varje frekvens (reaktivitet, distinkta klick och kumulerade klick), beräknas för leveranser som skickats under de senaste sex månaderna. Endast leveranser med samma typologi och i samma kanal beaktas. Korrektur ingår inte.

+++

### De tio mest besökta länkarna {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="De tio mest besökta länkarna"
>abstract="Diagrammet och tabellen **Top 10 most visit links** innehåller tillgängliga data för mottagarnas beteende per länk."


Diagrammet och tabellen **[!UICONTROL Top 10 most visited links]** innehåller tillgängliga data för mottagarnas beteende per länk.

![](assets/reporting_email_8.png){zoomable="yes"}{align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Percentage]**: Procentandel användare som interagerade med leveransen.

+++

### Klicknedbrytning över tid {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_click_breakdown"
>title="Klicknedbrytning över tid"
>abstract="Diagrammet **Klicknedbrytning över tid** visar tillgängliga data för mottagarens beteende per länk."


Diagrammet **[!UICONTROL Breakdown of clicks over time]** innehåller tillgängliga data för mottagarnas beteende per länk.

![](assets/reporting_email_9.png){zoomable="yes"}{align="center"}

## Användaraktiviteter {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Användaraktiviteter"
>abstract="Diagrammet **Användaraktiviteter** visar hur öppningar och klick delas upp i ett diagram. Du kan välja tidsperioden för måldata: sista dagen eller timmen eller 30 minuter."

Rapporten **[!UICONTROL User activities]** visar uppdelningen av öppningar och klick i form av ett diagram. Du kan välja tidsperioden för måldata: sista dagen eller timmen eller 30 minuter.

![](assets/reporting_email_10.png){zoomable="yes"}{align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++

## Spårningsstatistik {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Spårningsstatistik"
>abstract="Diagrammet **Spårningsstatistik** innehåller statistik om öppningar och klick. Du kan välja en specifik tidsram för måldata."

Diagrammet **[!UICONTROL Tracking Statistics]** innehåller statistik om öppningar och klick. Du kan välja en specifik tidsram för måldata.

![](assets/reporting_email_11.png){zoomable="yes"}{align="center"}

+++Läs mer om mätvärden för e-postleveransrapporter.

* **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

* **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++

## Indelning av öppningar {#breakdown-opens}

### Uppdelning av öppningar efter enhet {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Uppdelning efter enhet"
>abstract="Rapporten **Uppdelning per enhet** visar hur öppningar fördelats per enhet under perioden. För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje enhetstyp."

Rapporten **Uppdelning efter enhet** visar hur öppningar fördelats per enhet under perioden: persondatorer, Android-enheter, Apple-enheter eller andra.

För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje enhetstyp.

![](assets/reporting_email_13.png){zoomable="yes"}{align="center"}


### Uppdelning av öppningar efter operativsystem {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Uppdelning efter operativsystem"
>abstract="Rapporten **Uppdelning efter operativsystem** visar hur öppningarna är fördelade efter operativsystem under den aktuella perioden. I det första diagrammet visas statistik för öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje operativsystem."

Rapporten **Uppdelning efter operativsystem** visar hur öppningar fördelats efter operativsystem under perioden: Windows-system, Android-system, iOS-system eller andra.

För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila operativsystem. Den andra visar det exakta antalet och procentandelen för varje operativsystem.

![](assets/reporting_email_13.1.png){zoomable="yes"}{align="center"}

### Uppdelning av öppningar efter webbläsare {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Uppdelning efter webbläsare"
>abstract="**Uppdelningen per webbläsare** visar hur öppningar har delats upp per webbläsare under perioden. I det första diagrammet visas statistik för öppningar på datorer och mobila enheter. Den andra visar det exakta antalet och procentandelen för varje webbläsare."

Rapporten **Uppdelning per webbläsare** visar hur öppningarna är uppdelade efter webbläsare: Chrome, Safari, Internet Explorer med flera.

För varje kategori används två diagram. Den första visar statistik om öppningar på datorer och mobila operativsystem. Den andra visar det exakta antalet och procentandelen för varje webbläsare.

![](assets/reporting_email_13.2.png){zoomable="yes"}{align="center"}


## Klickningar {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Rapport om klickningar"
>abstract="Rapporten **Aktivitetsklickningar** visar e-postinnehållet (HTML och/eller text) med procentandelen klick på länkar för varje länk. Personaliseringsblock, ej prenumerationslänkar, spegelsideslänkar och erbjudandelänkar tas med i det totala antalet klickningar, men visas inte i rapporten."

Den här rapporten visar meddelandeinnehållet (HTML och/eller text) med procentandelen klickningar på länkar för varje länk. Personaliseringsblock, ej prenumerationslänkar, spegelsideslänkar och erbjudandelänkar tas med i det totala antalet klickningar, men visas inte i rapporten.

![](assets/reporting11.png){zoomable="yes"}
