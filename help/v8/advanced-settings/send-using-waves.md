---
audience: end-user
title: Skicka med påfyllnader
description: Läs mer om leveransinställningar på Campaign Web
badge: label="Begränsad tillgänglighet"
source-git-commit: 3bfcf3c5a5e054995993d38a073733fef8ea4be9
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 1%

---


# Skicka med vågor {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Waves-definition"
>abstract="Definiera vågor för att dela upp leveranser i flera grupper i stället för att skicka stora mängder meddelanden samtidigt."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Vågens storlek"
>abstract="Vågens storlek krävs. Ange antingen ett numeriskt värde (antal meddelanden) eller ett procentvärde (0-100 %) i storleksfältet."

För att balansera lasten kan du dela upp leveranser i flera satser. Konfigurera antalet batchar och deras proportioner i förhållande till hela leveransen.

>[!NOTE]
>
>Du kan bara definiera storleken och fördröjningen mellan två på varandra följande påfyllnader. Det går inte att konfigurera urvalskriterierna för mottagare för varje påfyllnad.

1. Öppna [leveransinställningar](delivery-settings.md#retries) och går till **[!UICONTROL Delivery]** -fliken.
1. Välj **[!UICONTROL Send using multiple waves]** och klicka på **[!UICONTROL Define waves...]** länk.

1. Så här konfigurerar du påfyllnader:

   * **[!UICONTROL Schedule multiple waves of the same size]**.

     Om du till exempel skriver **[!UICONTROL 30%]** i motsvarande fält representerar varje våg 30 % av de meddelanden som ingår i leveransen, utom den sista, som representerar 10 % av meddelandena.

     ![](assets/waves-same-size.png)

     I **[!UICONTROL Interval]** anger du fördröjningen mellan början av två påfyllnader i följd. Om du till exempel skriver **[!UICONTROL 2d]**, startar den första vågen omedelbart, den andra om två dagar, den tredje vågen om fyra dagar och så vidare.

   * **[!UICONTROL Schedule waves according to a calendar]**.

     I **[!UICONTROL Start]** -kolumnen anger du fördröjningen mellan början av två på varandra följande påfyllnader. I **[!UICONTROL Size]** anger du ett fast tal eller ett procenttal.

     I exemplet nedan representerar den första vågen 25 % av det totala antalet meddelanden som ingår i leveransen och börjar omedelbart. Nästa två vågor slutför leveransen och är inställda på att börja med 6 timmars intervall.

     ![](assets/waves-calendar.png)

     En specifik typologikontrollregel, **[!UICONTROL Wave scheduling check]**, säkerställer att den sista vågen planeras före leveransens giltighetsgräns. Kampanjtypologier och deras regler konfigureras i **[!UICONTROL Typology]** -fliken i leveransinställningarna. Läs mer om kontrollregler i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html).

     >[!IMPORTANT]
     >
     >Kontrollera att de sista påfyllnaderna inte överskrider leveransdatumet, som definieras i **[!UICONTROL Validity]** -fliken. Annars kanske vissa meddelanden inte skickas. [Läs mer](delivery-settings.md#validity)
     >
     >Du måste också ge tillräckligt med tid för att försöka igen när du konfigurerar de sista vågorna. [Läs mer](delivery-settings.md#retries)

1. Om du vill övervaka dina utskick går du till [leveransloggar](../monitor/delivery-logs.md).

Du kan se leveranser som redan har skickats i de bearbetade påfyllnaderna (**[!UICONTROL Sent]** status) och de leveranser som ska skickas i de återstående påfyllnaderna (**[!UICONTROL Pending]** status).

De två exemplen nedan är de vanligaste användningsområdena när du använder flera vågor.

* **Under avstämningsprocessen**

  När e-postmeddelanden skickas via en ny plattform, är Internetleverantörer (ISP) misstänkta för IP-adresser som inte känns igen. Om stora mängder e-postmeddelanden plötsligt skickas markerar internetleverantörerna dem ofta som skräppost.

  För att undvika att markeras som skräppost kan du stegvis öka volymen som skickas med vågor. Detta bör säkerställa en smidig utveckling av startfasen och göra det möjligt att minska den totala frekvensen av ogiltiga adresser.

  Använd **[!UICONTROL Schedule waves according to a calendar]** alternativ. Du kan till exempel ställa in den första vågen på 10 %, den andra på 15 % och så vidare.

  ![](assets/waves-ramp-up.png)

* **Kampanjer som involverar ett callcenter**

  När ni hanterar en lojalitetskampanj via telefon har er organisation begränsad kapacitet att behandla antalet samtal till kontaktabonnenter.

  Med hjälp av vågor kan du begränsa antalet meddelanden till 20 per dag, vilket är den dagliga bearbetningskapaciteten för ett callcenter.

  Om du vill göra det väljer du **[!UICONTROL Schedule multiple waves of the same size]** alternativ. Retur **[!UICONTROL 20]** som vågens storlek och **[!UICONTROL 1d]** i **[!UICONTROL Period]** fält.

  ![](assets/waves-call-center.png)