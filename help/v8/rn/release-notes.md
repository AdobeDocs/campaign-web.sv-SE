---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 14%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

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
