---
title: Arbeta med GenStudio for Performance Marketing i Adobe Campaign
description: Lär dig arbeta med GenStudio for Performance Marketing i Adobe Campaign
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 61e6dcf13fc6a405f5e25328bf336e863701b2fe
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Arbeta med GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="Använda en mall som byggts med GenStudio"
>abstract="Tack vare den smidiga integrationen med Adobe GenStudio for Performance Marketing kan du enkelt importera en GenStudio-mall som har förbättrats med Adobe AI-teknik."

## Kom igång med GenStudio {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} är en generativ AI-tillämpning som gör att marknadsföringsteamen kan skapa egna annonser och e-postmeddelanden för att skapa effektiva, personaliserade marknadsföringskampanjer som följer ert varumärke och följer företagets policy. Genom att utnyttja Adobe AI-teknik får du en omfattande verktygslåda som förenklar komplexa funktioner för att skapa och hantera innehåll så att kreatörerna kan fokusera på innovation.

>[!AVAILABILITY]
>
>Den här funktionen är endast tillgänglig för e-postkanalen.

För att öka marknadsföringens effektivitet och upprätthålla varumärkets enhetlighet kan du sömlöst integrera [!DNL **GenStudio for Performance Marketing**]-upplevelser med [!DNL **Adobe Campaign**]. Detta gör att du kan utnyttja [!DNL GenStudio]s AI-power-innehåll tillsammans med [!DNL Adobe Campaign]s avancerade orkestreringsfunktioner.

>[!INFO]
>
>Mer information finns i [översikten](https://business.adobe.com/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} och i [demon](https://business.adobe.com/products/genstudio-for-performance-marketing.html#demo){target="_blank"} av [!DNL Adobe GenStudio for Performance Marketing].

## Använd GenStudio i Adobe Campaign {#use-genstudio}

Integreringen [!DNL GenStudio for Performance Marketing] och [!DNL Adobe Campaign] gör att du kan låta marknadsförare från ditt företag samarbeta bättre för att effektivisera processerna.

En teknisk marknadsförare, som använder [!DNL Adobe Campaign] för att utveckla och automatisera e-postkampanjer, kan till exempel samarbeta med en resultatmarknadsförare som skapar innehåll med [!DNL GenStudio].

Med den här integreringen kan båda fungera tillsammans för att enkelt integrera varumärkesinnehåll från [!DNL GenStudio] i [!DNL Adobe Campaign] och leverera engagerande e-postmeddelanden som riktar sig till specifika kundsegment och ökar försäljningen.

### Exportera en HTML-mall från Adobe Campaign till GenStudio {#export-from-campaign-to-genstudio}

Först kan du exportera en [!DNL Adobe Campaign] HTML-mall med ditt varumärkes riktlinjer till [!DNL GenStudio for Performance Marketing]. Följ stegen nedan.

1. I [!DNL Adobe Campaign] får du tillgång till innehållet i din e-post. [Lär dig hur](../email/create-email.md#create-content)

1. I e-postmeddelandet för Designer väljer du **[!UICONTROL Export HTML]** från knappen **[!UICONTROL More]**.

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. Överför den här HTML-exporterade mallen till [!DNL GenStudio for Performance Marketing]. <!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >Lär dig hur du överför en HTML-mall till [!DNL GenStudio] i det dedikerade avsnittet [Adobe GenStudio for Performance Marketing-användarhandbok](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"}.<!--GenStudio doc to be updated with Campaign-->

1. I GenStudio använder du den här mallen för att skapa flera e-postvarianter med AI-uppmaningar och spara dem.

   >[!NOTE]
   >
   >Lär dig hur du skapar e-postupplevelser i den dedikerade [sektionen](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"} i GenStudio.

### Utnyttja GenStudio upplevelser i Adobe Campaign {#leverage-genstudio-experiences}

Följ stegen nedan om du vill utnyttja de [!DNL GenStudio] e-postvarianter som du nyss skapade genom att importera dem till [!DNL Adobe Campaign].

1. I [!DNL Adobe Campaign] [skapar du en e-postleverans](../email/create-email.md).

1. Klicka på knappen **[!UICONTROL Edit content]** på kontrollpanelen för e-postleverans. [Läs mer](../email/create-email.md#create-content)

1. Markera **[!UICONTROL Import HTML]** på startsidan för e-post till Designer och klicka på knappen **[!UICONTROL Adobe GenStudio for Performance Marketing]**.

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. Bläddra bland GenStudio upplevelser för att börja bygga ditt innehåll. Ni kan filtrera upplevelserna utifrån flera kriterier som produkter, personer, varumärken eller till och med färger.

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. Välj en upplevelse och klicka på **[!UICONTROL Use]**.

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. Markera den mapp där du vill importera GenStudio-upplevelsen.

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. Det markerade innehållet visas i e-post-Designer.

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >GenStudio-upplevelser [ som skapats från en [!DNL Adobe Campaign] mall](#export-from-ajo-to-genstudio) importeras direkt till e-postens Designer. GenStudio-upplevelser som skapats utan en [!DNL Adobe Campaign]-mall importeras till [kompatibilitetsläge](../email/existing-content.md).

   Använd [redigeringsverktygen för e-postinnehåll](../email/create-email-content.md) och [anpassningsfälten](../personalization/personalize.md) för att redigera din e-post efter behov. Spara innehållet.

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456038/?quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->