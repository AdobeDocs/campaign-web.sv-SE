---
audience: end-user
title: Lägg till en länk till spegelsidan
description: Lär dig hur du lägger till och hanterar länken till spegelsidan
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 00a612513bcb649d23b2c5b4d5ed05b06a6a80ef
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Spegelsida {#mirror-page}

Spegelsidan är en onlineversion av ditt e-postmeddelande. Att lägga till en länk till spegelsidan är en bra metod för e-postmarknadsföring. Användare kan bläddra till den spegelsida som finns i ett e-postmeddelande, t.ex. om de får problem med återgivningen eller om det finns skadade bilder när de försöker visa dem i sin inkorg. Vi rekommenderar även att du tillhandahåller en onlineversion av tillgänglighetsskäl eller för att uppmuntra social delning.

Spegelsidan som genererats av Adobe Campaign innehåller alla personaliseringsdata.

![Spegellänksexempel](assets/mirror-page-link.png){width="600" align="left"}

## Lägg till en länk till spegelsidan{#link-to-mirror-page}

I Adobe Campaign kan du infoga en länk till spegelsidan i e-postinnehållet med hjälp av det dedikerade **anpassningsblocket**. Det inbyggda anpassningsblocket **Länk för spegling av sida** infogar följande kod i ditt e-postinnehåll: `<%@ include view='MirrorPage' %>`.

Så här lägger du till en länk till en spegelsida i e-postmeddelandet:

1. Markera ett element (text eller bild) och klicka på **[!UICONTROL Insert link]** i det sammanhangsberoende verktygsfältet.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Välj ikonen **[!UICONTROL Add personalization]** för att komma åt anpassningsmenyn.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Välj **[!UICONTROL Mirror page URL]** på menyn **[!UICONTROL Fragments]** och klicka på **[!UICONTROL Add]**. [Lär dig använda uttrycksfragment](../content/use-expression-fragments.md)

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

Spegelsidan skapas automatiskt.

När e-postmeddelandet har skickats visas innehållet i e-postmeddelandet i sin standardwebbläsare när mottagarna klickar på länken för spegelsidan.

Som standard är kvarhållningsperioden för en spegelsida **60 dagar**. Efter den fördröjningen är spegelsidan inte längre tillgänglig.

>[!CAUTION]
>
>* Länkar för spegelsidor genereras automatiskt och kan inte redigeras. De innehåller alla krypterade, personliga data som krävs för att återge det ursprungliga e-postmeddelandet. Om du använder anpassade attribut med stora värden kan det därför generera långa URL-adresser för spegelsidor, vilket kan förhindra länken från att fungera i webbläsare som har en maximal URL-längd.
>
>* I det korrektur som skickas till testprofilerna är länken till spegelsidan inte aktiv. Den är bara aktiv i de slutliga meddelandena.


## Generering av spegelsida {#mirror-page-generation}

Som standard genereras spegelsidan automatiskt av Adobe Campaign om e-postinnehållet inte är tomt, och om det innehåller en länk till spegelsidan (även Spegellänk).

Du kan styra genereringsläget för e-postspeglingssidan. Alternativ finns i leveransegenskaperna. [Läs mer](../advanced-settings/delivery-settings.md#mirror)
