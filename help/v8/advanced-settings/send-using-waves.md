---
audience: end-user
title: Skicka med påfyllnader
description: Läs mer om leveransinställningar på Campaign Web
feature: Email
exl-id: d4cd5fe5-f9ac-44ac-a961-ae45131aeb3e
source-git-commit: e5a17ad1f8316d201dc3b4bc6ce20d61aea7a9c9
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Skicka med vågor {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Dela upp leveranser i flera batchar"
>abstract="I stället för att skicka stora mängder meddelanden samtidigt definierar du vågor för att dela upp leveranser i flera satser. Du kan konfigurera flera vågor av samma storlek eller ange en kalender för de olika vågor som ska skickas."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Definiera storleken på varje våg"
>abstract="Du måste ange en storlek för alla påfyllnader som du lägger till. Ange antingen ett numeriskt värde (antal meddelanden för varje våg) eller ett procentvärde (0-100 %)."

Om du vill balansera inläsningen kan du dela upp e-postleveranser i flera grupper. Konfigurera antalet batchar och deras proportioner i förhållande till hela leveransen samt intervallet mellan två vågor.

>[!NOTE]
>
>Du kan bara definiera storleken och fördröjningen mellan två på varandra följande påfyllnader. Det går inte att justera urvalskriterierna för mottagare för varje påfyllnad.

Följ stegen nedan om du vill skicka leveranser med hjälp av påfyllnader.

1. Öppna [leveransinställningarna](delivery-settings.md#retries).

1. Gå till avsnittet **[!UICONTROL Delivery]**.

1. Välj alternativet **[!UICONTROL Send using multiple waves]**.

1. Så här konfigurerar du påfyllnader:

   * [Schemalägg flera vågor i samma storlek](#waves-same-size)
   * [Schemalägg påfyllnader enligt en kalender](#waves-calendar)

1. Förbered och skicka leveransen som vanligt. [Läs mer](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >Kontrollera att de senaste påfyllnaderna inte överskrider leveransdeadline som definierats på fliken [Giltighet](delivery-settings.md#validity), annars kanske inte vissa meddelanden skickas. En specifik typologikontrollregel, **[!UICONTROL Wave scheduling check]**, säkerställer att den sista påfyllnaden planeras före leveransens giltighetsgräns. Läs mer om kontrollregler i dokumentationen för [Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html).
   >
   >Du måste också ge tillräckligt med tid för att försöka igen när du konfigurerar de sista vågorna. [Läs mer](delivery-settings.md#retries)

1. Gå till [leveransloggarna](../monitor/delivery-logs.md) om du vill övervaka dina utskick. Du kan se leveranser som redan har skickats i de bearbetade påfyllnaderna (**[!UICONTROL Sent]** status) och leveranser som ska skickas i återstående påfyllnader (**[!UICONTROL Pending]** status).

## Schemalägg flera vågor i samma storlek {#waves-same-size}

Om du väljer det här alternativet har alla vågor samma storlek (förutom den sista) och fördröjningen mellan varje våg är alltid densamma.

![](assets/waves-same-size.png){zoomable="yes"}

* Ange storleken för alla vågor som du delar leveransen till. Du kan ange ett procentvärde eller ett numeriskt värde. Endast den sista vågen kan variera i storlek eftersom den måste innehålla det återstående antalet meddelanden.

  Om du till exempel anger **[!UICONTROL 30%]** i fältet **[!UICONTROL Waves size]** representerar de första tre vågorna 30 % av alla meddelanden som ingår i leveransen, och den fjärde står för de återstående 10 %.

* I avsnittet **[!UICONTROL Interval]** anger du fördröjningen mellan början av två på varandra följande påfyllnader. Om du till exempel anger **[!UICONTROL 2 days]** startar den första vågen omedelbart, den andra om två dagar, den tredje vågen om fyra dagar och så vidare.

Ett vanligt användningssätt för flera vågor av samma storlek är att ett callcenter är involverat. När ni hanterar en lojalitetskampanj via telefon har er organisation begränsad kapacitet att behandla antalet samtal till kontaktabonnenter.

Med hjälp av vågor kan du begränsa antalet meddelanden till 20 per dag, vilket är den dagliga bearbetningskapaciteten för ett callcenter.

Välj alternativet **[!UICONTROL Schedule multiple waves of the same size]** om du vill göra det. Ange **[!UICONTROL 20]** som vågstorlek och **[!UICONTROL 1 day]** i fältet **[!UICONTROL Interval]**.

![](assets/waves-call-center.png){zoomable="yes"}

## Schemalägg påfyllnader enligt en kalender {#waves-calendar}

Om du väljer det här alternativet måste du definiera startdag/starttid för varje påfyllnad som du skickar, samt storleken för varje påfyllnad.

* I fälten **[!UICONTROL Start]** anger du fördröjningen mellan början av två på varandra följande påfyllnader.

* Ange ett fast tal eller en procentsats i kolumnen **[!UICONTROL Size]**.

Lägg till så många vågor du vill. Du kan ordna om dem efter dina behov.

>[!NOTE]
>
>Om du använder procenttal får summan för alla vågor inte överstiga 100 %.

I exemplet nedan representerar den första vågen 25 % av det totala antalet meddelanden som ingår i leveransen och börjar omedelbart. Nästa två vågor slutför leveransen och är inställda på att börja med 6 timmars intervall.

![](assets/waves-calendar.png){zoomable="yes"}

Ett vanligt användningsfall för flera vågor enligt en kalender är under uppspelningsprocessen.

När e-postmeddelanden skickas via en ny plattform, är Internetleverantörer (ISP) misstänkta för IP-adresser som inte känns igen. Om stora mängder e-postmeddelanden plötsligt skickas markerar internetleverantörerna dem ofta som skräppost.

För att undvika att markeras som skräppost kan du stegvis öka volymen som skickas med vågor. Detta bör säkerställa en smidig utveckling av startfasen och göra det möjligt att minska den totala frekvensen av ogiltiga adresser.

Använd alternativet **[!UICONTROL Schedule waves according to a calendar]** om du vill göra det. Du kan till exempel ställa in den första vågen på 10 %, den andra på 15 %, den tredje på 20 % och så vidare.

![](assets/waves-ramp-up.png){zoomable="yes"}
