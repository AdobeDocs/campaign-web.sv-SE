---
audience: end-user
title: Lägg till en länk till spegelsidan
description: Lär dig hur du lägger till och hanterar länken till spegelsidan
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Spegelsida {#mirror-page}

Spegelsidan är en onlineversion av ditt e-postmeddelande. Att lägga till en länk till spegelsidan är en bra vana vid e-postmarknadsföring. Användarna kan till exempel få åtkomst till spegelsidan i ett e-postmeddelande om de får problem med återgivningen eller om brutna bilder visas i inkorgen. Vi rekommenderar även att du tillhandahåller en onlineversion av tillgänglighetsskäl eller för att uppmuntra social delning.

Spegelsidan som genereras av Adobe Campaign innehåller alla personaliseringsdata.

![Exempel på en spegellänk i ett e-postmeddelande](assets/mirror-page-link.png){width="600" align="left"}

## Lägg till en länk till spegelsidan {#link-to-mirror-page}

I Adobe Campaign infogar du en länk till spegelsidan i e-postinnehållet med det dedikerade **personaliseringsblocket**. Det inbyggda anpassningsblocket **Länk för spegling av sida** infogar följande kod i ditt e-postinnehåll: `<%@ include view='MirrorPage' %>`.

Så här lägger du till en länk till en spegelsida i e-postmeddelandet:

1. Markera ett element (text eller bild) och klicka på **[!UICONTROL Insert link]** i det sammanhangsberoende verktygsfältet.

   ![Sammanhangsberoende verktygsfält med alternativet Infoga länk](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Välj ikonen **[!UICONTROL Add personalization]** för att komma åt anpassningsmenyn.

   ![Personalization-menyn i Adobe Campaign](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Välj **[!UICONTROL Mirror page URL]** på menyn **[!UICONTROL Fragments]** och klicka på **[!UICONTROL Add]**. [Lär dig använda uttrycksfragment](../content/use-expression-fragments.md)

   ![Alternativet URL för spegelsida på menyn Fragment](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

Spegelsidan skapas automatiskt.

När e-postmeddelandet skickas kan mottagare som klickar på länken för spegelsidan se e-postinnehållet som visas i deras standardwebbläsare.

Som standard är kvarhållningsperioden för en spegelsida **60 dagar**. Efter den här perioden är spegelsidan inte längre tillgänglig.

>[!CAUTION]
>
>* Spegelsidlänkar genereras automatiskt och kan inte redigeras. De innehåller alla krypterade, personliga data som krävs för att återge det ursprungliga e-postmeddelandet. Om du använder anpassade attribut med stora värden kan det generera långa URL-adresser för spegelsidor, vilket kan förhindra länken från att fungera i webbläsare med en maximal URL-längd.
>
>* I korrekturet som skickas till testprofiler är länken till spegelsidan inte aktiv. Den är bara aktiv i de slutliga meddelandena.

## Generering av spegelsida {#mirror-page-generation}

Som standard genererar Adobe Campaign automatiskt spegelsidan om e-postinnehållet inte är tomt och innehåller en länk till spegelsidan (kallas även spegellänk).

Styr e-postspegelsidans genereringsläge med alternativ som finns i leveransegenskaperna. [Läs mer](../advanced-settings/delivery-settings.md#mirror)