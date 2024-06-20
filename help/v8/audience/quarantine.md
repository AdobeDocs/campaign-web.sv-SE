---
audience: end-user
title: Om karantän
description: Förstå hanteringen av karantänadresser
source-git-commit: 9abf58c35fcf396e3003f9ecba728cd77df844a1
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Karantän

Adobe Campaign hanterar karantänadresser (e-post, SMS, push-meddelanden).

Karantän gäller endast för en **e-postadress**, a **telefonnummer**, eller en **enhetstoken**, men inte själva profilen. En profil vars e-postadress är placerad i karantän kan till exempel uppdatera sin profil och ange en ny adress. Därefter kan den användas av leveransåtgärder igen. Om två profiler råkar ha samma telefonnummer, påverkas båda om numret sätts i karantän.


>[!CAUTION]
>
>Karantän i Adobe Campaign är skiftlägeskänsligt.

## Vad är karantän?

Karantän är vägen till **hantera ogiltiga adresser i leveranser**.

Om en leverans har en hög frekvens av ogiltiga adresser kan den betraktas som skräppost. Genom att hantera adresserna i karantän kan du undvika att bli blocklist av internetleverantörer. Det här är viktigt för ditt rykte.

När en adress sätts i karantän i Adobe Campaign utesluts profilen automatiskt från målet under leveransanalysen.

Karantänen hjälper dig att minska SMS-sändningskostnaderna genom att utesluta felaktiga telefonnummer från leveranser.

## Varför en adress skickas till karantän

Det kan finnas många skäl till att skicka en adress till karantän:

- Felaktiga telefonnummer för SMS
- För SMS, när profilen svarar på ett SMS-meddelande med ett nyckelord som &quot;STOP&quot;
- För e-post, när ditt meddelande rapporteras som skräppost. Meddelandet dirigeras automatiskt om till en teknisk brevlåda som hanteras av Adobe. Användarens e-postadress skickas sedan automatiskt till karantän med Blocklist status.
- En e-postadress kan sättas i karantän, till exempel när postlådan är full, om adressen inte finns eller om e-postservern inte är tillgänglig.

[Läs mer om leveransfel](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/monitoring-deliveries/understanding-delivery-failures)

## Var hittar du karantänadresserna?

Du kan visa alla karantänadresser för din instans i **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Non deliverables Management]** > **[!UICONTROL Non deliverables and addresses]**. I det här avsnittet listas element i karantän för e-post-, SMS- och push-meddelandekanaler.

![](assets/quarantine_location.png){zoomable="yes"}

Du kan också få rapporten om karantänen i din instans:

![](assets/quarantine_reports.png){zoomable="yes"}

För varje leverans kan du även kontrollera leveranssammanfattningen: den visar antalet adresser i karantän i leveransmålet:

![](assets/quarantine_delivery.png){zoomable="yes"}

Du kan ha fler möjligheter att hantera karantänadresserna i Adobe Campaign Console. [Läs mer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
