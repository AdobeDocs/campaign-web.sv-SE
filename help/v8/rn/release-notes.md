---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: aea828da825a416dece6c4bee1da6d4e570e4e48
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 13%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

## September-uppdateringar {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI Assistant Content Accelerator</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>När du har skapat och skräddarsytt ditt budskap tar du det till nästa nivå med AI Assistant i Adobe Campaign Web for Content Acceleration. Med det här kraftfulla verktyget kan du optimera effekten av ditt innehåll genom att generera en mängd engagerande text, huvudtitlar och visuellt tilltalande bilder.</p>
<p>Fördjupa dig i en praktisk upplevelse med <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">vår förhandsvisning av aktiva funktioner</a>, som är utformad för att du först ska kunna utforska dess funktioner och till fullo förstå dess funktioner.</a>.</p>
<p>Mer information finns i den <a href="../email/generative-gs.md">detaljerade dokumentationen</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Tillgänglighetsdatum: 12 sept</p>
</td>
</tr>
</tbody>
</table>

## Versionsinformation, augusti {#24-8-release}

**Releasedatum**: 3 september 2024

Följande funktioner och förbättringar är tillgängliga från och med augusti.

* **Distribution av värden** - Vid åtkomst till listan med fält för anpassning kan du nu kontrollera hur värden distribueras för varje fält. Ett dedikerat popup-fönster visar antalet och procentandelen för varje värde. [Läs mer](../query/build-query.md#distribution-values-query)

* **SMTP-parametrar** - SMTP-inställningar är nu tillgängliga i inställningarna för e-postleverans. [Läs mer](../advanced-settings/delivery-settings.md#smtp)

* **Globala variabler** - Nu kan du definiera globala variabler för att definiera värden för leveranser. [Läs mer](../advanced-settings/delivery-settings.md#variables-delivery)

### Nya funktioner i begränsad tillgänglighet {#acs-24-8}

>[!AVAILABILITY]
>
>Följande funktioner är i Begränsad tillgänglighet (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.
>
>Se följande dokumentationssidor: [Campaign Standard övergång till Campaign v8](../rn/acs-migration.md) och [Funktioner för Campaign Standard-användare](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}.

* **Varumärkning för direktreklam** - Tekniska administratörer kan nu definiera ett eller flera varumärken för att centralisera parametrarna som påverkar ett varumärkes identitet. Detta inkluderar logotypen, domänen för landningssidans åtkomst-URL eller inställningar för meddelandespårning. Nu kan du skapa dessa varumärken och länka dem till meddelanden eller landningssidor. Den här konfigurationen hanteras i mallar. [Läs mer](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Prenumerationer med landningssidor** - Nu kan du länka en landningssida till en tjänst och skicka ett bekräftelsemeddelande när användare validerar den. [Läs mer](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visuella fragment** - Nu kan du arkivera visuella innehållsfragment. [Läs mer](../content/create-fragment.md#archive)

* **Captcha på landningssidor** - Nu kan du lägga till captcha för att skydda din landningssida från skräppost och missbruk som orsakas av bottnar. Detta är icke-störande för kunderna eftersom det inte kräver någon interaktion från dem och baseras på interaktioner med webbplatsen. [Läs mer](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
