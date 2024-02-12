---
audience: end-user
title: Lägg till en länk till spegelsidan
description: Lär dig hur du lägger till och hanterar länken till spegelsidan
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Lägg till en länk till spegelsidan{#mirror-page}

Spegelsidan är en onlineversion av ditt e-postmeddelande.

De flesta e-postklienter återger bilder utan problem, men vissa förinställningar kan undvika att visa bilder av säkerhetsskäl. Användare kan bläddra till den spegelsida som finns i ett e-postmeddelande, t.ex. om de får problem med återgivningen eller om det finns skadade bilder när de försöker visa dem i sin inkorg. Vi rekommenderar även att du tillhandahåller en onlineversion av tillgänglighetsskäl eller för att uppmuntra social delning.

Spegelsidan som genererats av Adobe Campaign innehåller alla personaliseringsdata.

![exempel på spegellänk](assets/mirror-page-link.png){width="600" align="left"}

## Lägg till en länk till spegelsidan{#link-to-mirror-page}

Det är bra att infoga en länk till spegelsidan. Den här länken kan till exempel vara Visa det här e-postmeddelandet i webbläsaren eller Läs det här online. Den finns ofta i e-postmeddelandets sidhuvud eller sidfot.

I Adobe Campaign kan du infoga en länk till spegelsidan i e-postinnehållet med den dedikerade **personaliseringsblock**. Den inbyggda **Länk till spegelsida** anpassningsblocket infogar följande kod i ditt e-postinnehåll: `<%@ include view='MirrorPage' %>`.

Så här lägger du till en länk till en spegelsida i ditt e-postmeddelande:

1. Markera ett element och klicka på **[!UICONTROL Insert link]** i kontextverktygsfältet.

   ![](assets/message-tracking-mirror-page.png){zoomable=&quot;yes&quot;}

1. Välj **[!UICONTROL Add personalization]** -ikonen för att komma åt personaliseringsmenyn.

   ![](assets/message-tracking-mirror-page_2.png){zoomable=&quot;yes&quot;}

1. Från **[!UICONTROL Content block]** meny, välja **[!UICONTROL Mirror page URL]** och klicka **[!UICONTROL Add]**.

   ![](assets/message-tracking-mirror-page_3.png){zoomable=&quot;yes&quot;}

   Mer information om infogning av anpassade innehållsblock finns i [det här avsnittet](../personalization/personalize.md#personalize-emails).

Spegelsidan skapas automatiskt.

>[!IMPORTANT]
>
>Länkar för spegelsidor genereras automatiskt och kan inte redigeras. De innehåller alla krypterade, personliga data som krävs för att återge det ursprungliga e-postmeddelandet. Om du använder anpassade attribut med stora värden kan det därför generera långa URL-adresser för spegelsidor, vilket kan förhindra länken från att fungera i webbläsare som har en maximal URL-längd.

När e-postmeddelandet har skickats visas innehållet i e-postmeddelandet i sin standardwebbläsare när mottagarna klickar på länken för spegelsidan.

>[!NOTE]
>
>I det testmeddelande som skickas till testprofilerna är länken till spegelsidan inte aktiv. Den aktiveras endast i de slutliga meddelandena.

Som standard är kvarhållningsperioden för en spegelsida 60 dagar. Efter den fördröjningen är spegelsidan inte längre tillgänglig.


## Generering av spegelsida{#mirror-page-generation}

Som standard genereras spegelsidan automatiskt av Adobe Campaign om e-postinnehållet inte är tomt, och om det innehåller en länk till spegelsidan (även Spegellänk).

Du kan styra genereringsläget för e-postspeglingssidan. Alternativ finns i leveransegenskaperna. [Läs mer](../advanced-settings/delivery-settings.md#mirror)
