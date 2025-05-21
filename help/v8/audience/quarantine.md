---
audience: end-user
title: Om karantän
description: Förstå hanteringen av karantänadresser
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Karantänhantering {#quarantines}

Adobe Campaign hanterar karantänadresser för e-post-, push- och SMS-kanaler.

Karantänen gäller bara för en **e-postadress**, ett **telefonnummer** eller en **enhetstoken**, men inte för själva profilen. En profil vars e-postadress är i karantän kan till exempel uppdateras med en ny adress. Profilen kan sedan hanteras av leveransåtgärder igen. Om två profiler delar samma telefonnummer påverkas båda om numret sätts i karantän.

>[!CAUTION]
>
>Karantän i Adobe Campaign är skiftlägeskänsligt.

## Vad är karantän? {#quarantines-what}

Karantän är den metod som används för att **hantera ogiltiga adresser i leveranser**.

Om en leverans har en hög frekvens av ogiltiga adresser kan den betraktas som skräppost. Genom att hantera adresserna med karantän kan du förhindra att de blocklist av internetleverantörer. Detta är viktigt för att du ska kunna behålla ditt rykte.

När en adress sätts i karantän i Adobe Campaign utesluts profilen automatiskt från målet vid leveransanalysen.

Karantän minskar SMS-sändningskostnaderna genom att utesluta felaktiga telefonnummer från leveranser.

Läs mer om karantäner i dokumentationen för [Campaign v8 (konsol)](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"}.

## Varför en adress skickas till karantän {#quarantines-why}

Det finns många skäl till att skicka en adress till karantän:

* Felaktiga telefonnummer för SMS
* För SMS, när profilen svarar på ett SMS-meddelande med ett nyckelord som &quot;STOP&quot;
* För e-post, när ditt meddelande rapporteras som skräppost. Meddelandet dirigeras automatiskt till en teknisk brevlåda som hanteras av Adobe. Användarens e-postadress skickas sedan automatiskt till karantän med Blocklist status.
* En e-postadress kan sättas i karantän, till exempel när postlådan är full, om adressen inte finns eller om e-postservern inte är tillgänglig.

Läs mer om leveransfel i dokumentationen för [Campaign v8 (konsol)](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"}.

## Var hittar du karantänadresserna? {#quarantines-where}

Du kan visa alla karantänadresser i din instans i **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Non deliverables Management]** > **[!UICONTROL Non deliverables and addresses]**. I det här avsnittet listas element i karantän för e-post-, SMS- och push-meddelandekanaler.

![Karantänplats i Adobe Campaign-gränssnitt](assets/quarantine_location.png){zoomable="yes"}

Du kan även få åtkomst till en rapport om karantänen i din instans:

![Karantänrapporter i Adobe Campaign-gränssnitt](assets/quarantine_reports.png){zoomable="yes"}

För varje leverans kan du kontrollera leveranssammanfattningsrapporten. Den visar antalet adresser i karantän i leveransmålet:

![Leveranssammanfattningsrapport med adresser i karantän](assets/quarantine_delivery.png){zoomable="yes"}

Du kan utforska fler alternativ för att hantera karantänadresser i Adobe Campaign Console. [Läs mer](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses).