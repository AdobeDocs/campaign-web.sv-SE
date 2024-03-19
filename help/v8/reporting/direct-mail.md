---
audience: end-user
title: Rapporter om direktreklam
description: Lär dig hur du får åtkomst till och använder rapporter via direktreklam
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Rapport om direktleverans av e-post {#direct-mail-report}

The **Rapport om direktleverans av e-post** ger omfattande insikter och data som är specifika för er direktutskick. Den ger detaljerad information om prestanda, effektivitet och resultat för era individuella leveranser och ger er en heltäckande översikt.

## Leveranssammanfattning {#delivery-summary-direct-mail}

### Leveransöversikt {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Leveransöversikt"
>abstract="The **Leveransöversikt** presenterar nyckeltal (KPI:er) som ger djupgående insikter i hur besökarna interagerar med varje direktutskick. Mätvärdena beskrivs nedan."

The **[!UICONTROL Delivery Overview]** ger detaljerade insikter om hur besökarna interagerar med varje direktutskick och visar viktiga nyckeltal (KPI).  Mätvärdena beskrivs nedan.

![](assets/direct-overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++Läs mer om leveransöversiktssiffror.

* **[!UICONTROL Messages to deliver]**: Totalt antal meddelanden som bearbetats under leveransförberedelsen.

* **[!UICONTROL Targeted]**: Antal användarprofiler som kvalificerar sig som målprofiler för dina direktutskick.

* **[!UICONTROL To exclude]**: Antal användarprofiler, exkluderade från målprofilerna, som inte kommer att ta emot dina direktutskick.
+++

### Inledande målpopulation {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Inledande målpopulation"
>abstract="The **Inledande målpopulation** I diagrammet visas data i förhållande till dina mottagare och meddelanden, baserat på resultatet av leveransförberedelsen."

The **[!UICONTROL Initial target population]** I diagrammet visas data relativt dina mottagare. Mätvärden beräknas under färdigställandet av leveransen och visar: den initiala målgruppen, antalet meddelanden som ska skickas, antalet exkluderade mottagare.

![](assets/direct-mail-delivery-targeted-population.png){zoomable=&quot;yes&quot;}

För musen över en del av diagrammet för att visa det exakta talet.

![](assets/direct-mail-delivery-targeted-population_2.png){zoomable=&quot;yes&quot;}

+++Läs mer om rapportvärden för direktutskick.

* **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

* **[!UICONTROL To deliver]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Exclusion]**: Totalt antal mottagare exkluderade från målpopulationen.
+++

### Leveransstatistik {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="Leveransstatistik"
>abstract="The **Leveransstatistik** diagram visar hur din direktutskick lyckades och vilka fel som inträffade."

The **[!UICONTROL Delivery statistics]** graf ger en omfattande översikt över leveransresultaten och ger detaljerade mätvärden för att mäta framgång och effektivitet.

![](assets/direct-mail-delivery-stats.png){zoomable=&quot;yes&quot;}

+++Läs mer om rapportvärden för kampanjer i direktreklam.

* **[!UICONTROL Message sent]**: Totalt antal meddelanden som ska levereras efter leveransförberedelse.

* **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

* **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

### Orsaker till uteslutning {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Leveransorsaker"
>abstract="The **Orsaker till uteslutning** graf visar distributionen av avvisade meddelanden under färdigställandet av leveransen, indelat i kategorier."

The **[!UICONTROL Causes of exclusion]** I diagrammet ges en detaljerad beskrivning av skälen till att meddelanden inte godkänns under beredningen av leveransen. Uppdelningen är uppdelad enligt olika regler och ger en heltäckande bild av de faktorer som bidrar till att utesluta meddelanden. Exkluderingsregler finns i [Kampanjdokumentation v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/direct-mail-delivery-exclusions.png){zoomable=&quot;yes&quot;}{align="center" zoomable="yes"}

+++Läs mer om orsaker till uteslutning.

* **[!UICONTROL Address in quarantine]**: Feltyp som genereras när adressen placeras i karantän.

* **[!UICONTROL Address not specified]**: Feltyp som genereras när en leverans skickas för att ange att adressen inte finns.

* **[!UICONTROL Bad quality address]**: Feltyp som genereras när kvalitetsklassen för postadresser är för låg.

* **[!UICONTROL Denylisted address]**: Feltyp som genererades när mottagaren blocklist när leveransen utfördes.

* **[!UICONTROL Double]**: Feltyp som genererades när mottagaren exkluderades eftersom dess nyckelvärden inte var unika.

* **[!UICONTROL Control group]**: Mottagarens adress ingår i kontrollgruppen.

* **[!UICONTROL Target limited in size]**: Den maximala leveransstorleken har uppnåtts för mottagaren.

+++

### Undantag {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Undantag"
>abstract="The **[!UICONTROL Exclusions]** tabellen visar en detaljerad beskrivning, per regel, av meddelanden som avvisats under leveransförberedelseprocessen."

The **[!UICONTROL Exclusions]** tabellen innehåller en detaljerad beskrivning, indelad efter specifika regler, av meddelanden som avvisats under leveransfasen. Denna omfattande uppdelning ger en tydlig förståelse för orsakerna till att dessa meddelanden utesluts från leveransprocessen.

![](assets/direct-mail-exclusions.png){zoomable=&quot;yes&quot;}{align="center" zoomable="yes"}

Tillgängliga mått är samma som för [Orsaker till uteslutning](#direct-mail-delivery-exclusions) som beskrivs ovan.
