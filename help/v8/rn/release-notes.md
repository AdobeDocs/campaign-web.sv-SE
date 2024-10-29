---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 13%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

## Oktober-version {#24-10-release}

**Releasedatum**: 29 okt 2024

Följande funktioner och förbättringar är tillgängliga från och med oktober.

### Funktioner

<table>
<thead>
<tr>
<th><strong>Externa konton</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du konfigurera och hantera externa konton direkt via Adobe Campaign webbanvändargränssnitt. Den här nya funktionen gör det enkelt att konfigurera olika typer av externa konton, till exempel studentmeddelanden (POP3) eller exekveringsinstanser.</p>
<p>Mer information finns i den <a href="../administration/external-account.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transaktionsmeddelanden</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skapa och övervaka transaktionsmeddelanden i gränssnittet för Campaign-webben. Transactional messaging är en specialiserad modul i Adobe Campaign som hanterar utlösta meddelanden. Dessa meddelanden genereras automatiskt som svar på händelser som kommer från informationssystem. Vanliga exempel på sådana händelser är att klicka på knappar eller länkar, överge varukorgar, begära varningar om produkttillgänglighet, skapa eller ändra konto osv.</p>
<p>Mer information finns i den <a href="../transactional-messaging/transactional.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Förbättringar

* **Arbetsflödesaktiviteter** - Du kan nu flytta en aktivitet och alla dess underordnade noder från en övergång till en annan i ett arbetsflöde. En dedikerad **Flytta**-knapp är tillgänglig i aktivitetens egenskapspanel för att utföra detta. [Läs mer](../workflows/orchestrate-activities.md#move)

* **Aktivitet för arbetsflödesberikning**

   * Du kan nu definiera ett alias och en etikett när du skapar ett nytt fält i aktiviteten **Enrichment**. [Läs mer](../workflows/activities/enrichment.md#collection-settings)
   * Nu kan du lägga till erbjudanden för varje profil i aktiviteten **Enrichment**. [Läs mer](../workflows/activities/enrichment.md##add-offers)

* **Distribution av värden** - Vid åtkomst till listan med fält för anpassning kan du nu kontrollera hur värden distribueras för varje fält. Ett dedikerat popup-fönster visar antalet och procentandelen för varje värde. [Läs mer](../query/build-query.md#distribution-values-query)


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
<p>När du har skapat och skräddarsytt ditt budskap går du ett steg längre med AI Assistant Content Accelerator i Adobe Campaign Web. Med det här kraftfulla verktyget kan du optimera effekten av ditt innehåll genom att generera en mängd engagerande text, huvudtitlar och visuellt tilltalande bilder.</p>
<p>Fördjupa dig i en praktisk upplevelse med <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">vår förhandsvisning av aktiva funktioner</a>, som är utformad för att du först ska kunna utforska dess funktioner och till fullo förstå dess funktioner.</a>.</p>
<p>Mer information finns i den <a href="../email/generative-gs.md">detaljerade dokumentationen</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Tillgänglighetsdatum: 12 sept</p>
</td>
</tr>
</tbody>
</table>

## Augustiversion {#24-8-release}

**Releasedatum**: 3 september 2024

Följande funktioner och förbättringar är tillgängliga från och med augusti.

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
