---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 11%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

Ändringar och förbättringar som är tillgängliga med tidigare versioner visas på sidorna [2024](release-notes-24.md) och [2025](release-notes-25.md) .

## Version 25 juli {#25-7-release}

### Nya funktioner {#25-7-features}

Följande funktioner är tillgängliga från och med juli.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Stöd för anpassad CSS i e-post-Designer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>När du utformar dina e-postmeddelanden kan du nu lägga till din egen anpassade CSS direkt i e-post-Designer. Med den här funktionen kan du använda avancerad och specifik formatering, vilket ger större flexibilitet och kontroll över utseendet på innehållet.</p>
<p>Mer information finns i den <a href="../email/custom-css.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Varumärken</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan ni skapa och anpassa era egna varumärken för att tydligt definiera er visuella och verbala identitet i alla slags kommunikation. Med varumärkesjusteringspoängen kan ni få feedback i realtid om hur väl ert innehåll speglar ert varumärkes ton, stil och riktlinjer, så att ni kan hålla er enhetliga med varje budskap ni skickar.
</p>
<p>Mer information finns i den <a href="../content/brands.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Leveransvarningar</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Funktionen för leveransvarning är ett varningssystem som gör att en grupp användare automatiskt kan ta emot meddelanden som innehåller information om hur leveransen utförs.</p>
<p>Mer information finns i den <a href="../msg/delivery-alerting.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>Dynamisk rapportering</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu har ni tillgång till Dynamic Reporting som tillhandahåller helt anpassningsbara realtidsrapporter för att mäta effekten av era marknadsföringsaktiviteter. Det ger åtkomst till profildata, vilket möjliggör demografiska analyser efter profildimensioner som kön, ort och ålder, utöver funktionella e-postkampanjdata som öppningar och klick. Dynamisk rapportering finns också för flerspråkiga e-postleveranser och transaktionsmeddelanden.</p>
<p>Den här funktionen är bara tillgänglig på begäran. Kontakta din Adobe-representant för att få åtkomst. Servern måste uppgraderas till minst 8.8.1. Mer information finns i versionsinformationen för klientkonsolen <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank"></a>.
<p>Mer information finns i den <a href="../reporting/dynamic-reporting/get-started-reporting.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Centraliserad varumärkesprofilering</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Era tekniska administratörer kan nu definiera ett eller flera varumärken för att centralisera de parametrar som påverkar ett varumärkes identitet. Detta inkluderar logotypen, domänen för landningssidans åtkomst-URL eller inställningar för meddelandespårning. Du kan skapa dessa varumärken och länka dem till meddelanden eller landningssidor. Den här konfigurationen hanteras i mallar. Varumärkesalternativ är tillgängliga för alla kanaler, inklusive SMS och direktreklam.</p>
<p>Den här funktionen är endast tillgänglig vid behov, för nya implementeringar. Kontakta din Adobe-representant för att få åtkomst. Servern måste uppgraderas till minst 8.8.1. Mer information finns i versionsinformationen för klientkonsolen <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank"></a>.
<p>Mer information finns i den <a href="../administration/branding/branding-gs.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

Utöver de funktioner som listas ovan innehåller den här versionen även en uppsättning funktioner som är tillgängliga i klientkonsolen:

* [Ny SMS-sändningskontakt](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA-miljöer)
* [Återstående API:er](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (on demand, FDA-miljöer)

Mer information finns i versionsinformationen för klientkonsolen [&#128279;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

-->

### Förbättringar {#25-7-improvements}

* Du kan nu beräkna målpopulationen direkt på varje villkor och grupp i regelbyggaren. Klicka på resultatnumret för att visa en detaljerad lista över poster. [Läs mer](../query/build-query.md#validate-query)

* Du kan nu redigera eller ta bort ett fördefinierat filter direkt från regelbyggaren. [Läs mer](../get-started/predefined-filters.md#manage-predefined-filter)

* När du konfigurerar en SMS-leverans har du nu åtkomst till de **valfria SMPP-parametrarna (TLV)** i avsnittet **SMS**. Den här parametern är densamma som i klientkonsolen. [Läs mer](../advanced-settings/delivery-settings.md#sms-tab)

* Nu kan du aktivera bakgrundsmeddelanden på iOS med det nya alternativet **Innehåll tillgängligt** som finns i avsnittet **Avancerade inställningar** på skärmen för iOS innehållsutgåva. Detta lägger till flaggan `content-available:1` i nyttolasten `aps`. Läs mer [på den här sidan](../push/content-push.md). Se även [den här sidan](../push/rich-push-ios.md)

* Följande förbättringar av landningssidan är nu tillgängliga:

   * Du kan nu hänvisa till en standardstartsida för prenumeration/avprenumeration när du konfigurerar en tjänst. När du utformar ett e-postmeddelande och definierar en länk till den landningssidan, prenumererar användare som skickar landningssidans formulär automatiskt på eller avbryter prenumerationen på den här tjänsten. [Läs mer](../audience/manage-services.md#create-service)
   * Ett nytt alternativ i landningssidans konfiguration gör att anonyma besökare kan komma åt landningssidan. Om du avmarkerar det här alternativet kan endast identifierade användare få åtkomst till och skicka formuläret. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Ett nytt alternativ i landningssidans konfiguration gör det möjligt att lagra ytterligare interna data när landningssidan skickas. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Med ett nytt alternativ kan du använda en landningssida för flera tjänster, vilket gör den dynamisk. När du lägger till en länk till ett e-postmeddelande kan du välja vilken tjänst som helst om du väljer en dynamisk landningssida. Om du väljer en landningssida som har en specifik tjänst kopplad till, kommer den här tjänsten att användas automatiskt (du kan inte välja en annan). [Läs mer](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Villkorligt innehåll stöds nu på landningssidor. [Läs mer](../landing-pages/lp-content.md)
   * Du kan länka en landningssida till en tjänst och skicka ett bekräftelsemeddelande när användare validerar den. [Läs mer](../landing-pages/lp-content.md#lp-message)
   * Du kan lägga till captcha för att skydda din landningssida mot skräppost och missbruk som orsakas av stötar. Detta är icke-störande för kunderna eftersom det inte kräver någon interaktion från dem och baseras på interaktioner med webbplatsen. [Läs mer](../landing-pages/create-lp.md#captcha)
