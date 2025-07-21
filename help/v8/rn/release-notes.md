---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 9%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

Ändringar och förbättringar som är tillgängliga i tidigare versioner visas i [2024](release-notes-24.md) och [2025](release-notes-25.md).

## Uppdateringar 25 juli {#25-7-updates}

>[!AVAILABILITY]
>
>För att få tillgång till dessa uppdateringar måste servern uppgraderas till minst 8.8.1. Mer information finns i versionsinformationen för klientkonsolen [&#128279;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=sv-SE){target="_blank"}.

Tidigare släppt i Begränsad tillgänglighet är följande funktioner nu tillgängliga i alla miljöer (allmän tillgänglighet):

* **Skapa flerspråkig leverans** - Nu kan du skicka flera e-postleveranser på olika språk i Adobe Campaign webbanvändargränssnitt. Med funktionen för flerspråkig leverans kan du välja standardspråk för leveransen samt de olika språk som leveransen kan skickas till. Du kan även förhandsgranska leveransen på de språk du har valt. [Läs mer](../email/edit-content.md#multilingual-delivery).

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=sv-SE){target="_blank"}
-->

* **Leveransavisering** - Leveransaviseringsfunktionen är ett varningshanteringssystem som gör att en grupp användare automatiskt kan ta emot meddelanden som innehåller information om hur deras leveranser utförs. [Läs mer](../msg/delivery-alerting.md)

* **Förbättringar av landningssidor** - Följande förbättringar av landningssidor är nu tillgängliga:

   * Du kan nu hänvisa till en standardstartsida för prenumeration/avprenumeration när du konfigurerar en tjänst. När du utformar ett e-postmeddelande och definierar en länk till den landningssidan, prenumererar användare som skickar landningssidans formulär automatiskt på eller avbryter prenumerationen på den här tjänsten. [Läs mer](../audience/manage-services.md#create-service)
   * Ett nytt alternativ i landningssidans konfiguration gör att anonyma besökare kan komma åt landningssidan. Om du avmarkerar det här alternativet kan endast identifierade användare få åtkomst till och skicka formuläret. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Ett nytt alternativ i landningssidans konfiguration gör det möjligt att lagra ytterligare interna data när landningssidan skickas. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Med ett nytt alternativ kan du använda en landningssida för flera tjänster, vilket gör den dynamisk. När du lägger till en länk till ett e-postmeddelande kan du välja vilken tjänst som helst om du väljer en dynamisk landningssida. Om du väljer en landningssida som har en specifik tjänst kopplad till, kommer den här tjänsten att användas automatiskt (du kan inte välja en annan). [Läs mer](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Villkorligt innehåll stöds nu på landningssidor. [Läs mer](../landing-pages/lp-content.md)
   * Du kan länka en landningssida till en tjänst och skicka ett bekräftelsemeddelande när användare validerar den. [Läs mer](../landing-pages/lp-content.md#lp-message)
   * Du kan lägga till captcha för att skydda din landningssida mot skräppost och missbruk som orsakas av stötar. Detta är icke-störande för kunderna eftersom det inte kräver någon interaktion från dem och baseras på interaktioner med webbplatsen. [Läs mer](../landing-pages/create-lp.md#captcha)

Tidigare släppt i Begränsad tillgänglighet är följande funktioner nu tillgängliga **på begäran**:

* **Dynamisk rapportering** - Nu kan du få tillgång till Dynamisk rapportering som ger helt anpassningsbara realtidsrapporter för att mäta effekten av dina marknadsföringsaktiviteter. Det ger åtkomst till profildata, vilket möjliggör demografiska analyser efter profildimensioner som kön, ort och ålder, utöver funktionella e-postkampanjdata som öppningar och klick. Dynamisk rapportering finns också för flerspråkiga e-postleveranser och transaktionsmeddelanden. [Läs mer](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centraliserad profilering** - Dina tekniska administratörer kan nu definiera ett eller flera varumärken för att centralisera parametrarna som påverkar ett varumärkes identitet. Detta inkluderar logotypen, domänen för landningssidans åtkomst-URL eller inställningar för meddelandespårning. Du kan skapa dessa varumärken och länka dem till meddelanden eller landningssidor. Den här konfigurationen hanteras i mallar. Varumärkesalternativ är tillgängliga för alla kanaler, inklusive SMS och direktreklam. [Läs mer](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Den här funktionen är bara tillgänglig för nya implementeringar.

Utöver de funktioner som listas ovan innehåller den här versionen även en uppsättning funktioner som är tillgängliga i klientkonsolen:

* [Ny SMS-avsändande koppling](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=sv-SE). (FDA-miljöer)
* [Återstående API:er](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=sv-SE) (on demand, FDA-miljöer)

Mer information finns i versionsinformationen för klientkonsolen [&#128279;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=sv-SE){target="_blank"}.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=sv-SE){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/sv/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->