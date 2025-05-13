---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: b730eeeaab5bfc87e8c9c10b6e25bed0e484fb64
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 13%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

Ändringar och förbättringar som är tillgängliga i tidigare versioner visas i [2024](release-notes-24.md) och [2025](release-notes-25.md).

## Uppdateringar maj 25 {#25-5-release}

<table>
<thead>
<tr>
<th><strong>Poäng för varumärkesjustering (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Poängen för varumärkesjustering ger tydlig feedback direkt i e-postdesignern, som hjälper dig att se om innehållet överensstämmer med varumärkets ton, stil och riktlinjer. Den här funktionen är tillgänglig i Beta.</p>
<p>Mer information finns i den <a href="../content/brands-score.md">detaljerade dokumentationen</a>.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

## 25 april {#25-4-release}

**Releasedatum**: 29 april 2025

### Nya funktioner {#25-4-features}

Följande funktioner är tillgängliga för alla användare från och med aprilversionen.

<table>
<thead>
<tr>
<th><strong>Kanal för kundtjänst</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Kundtjänstkanalen är nu tillgänglig i Campaign Web User-gränssnittet. Den här kanalen avser en kommunikationsmetod som används för att hantera och spåra kommunikation eller interaktioner som hanteras via ett callcenter - vanligtvis telefonsamtal som görs av agenter till kunder eller potentiella kunder.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Mer information finns i den <a href="../call-center/gs-call-center.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Nytt regelverktyg</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Det finns nu en ny regelbyggare som hjälper dig att definiera komplexa villkor i ett förbättrat användargränssnitt. Du kan vid behov växla från det gamla till det nya regelverktyget.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Mer information finns i den <a href="../query/query-modeler-overview.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Skapa externa konton</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Som Campaign-administratör kan du nu skapa nya anslutningar med externa system från användargränssnittet i Campaign Web.
Du kan också visa, uppdatera och hantera befintliga externa konton.</p>
<p>Mer information finns i den <a href="../administration/external-account.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

### Förbättringar {#25-4-improvements}

**Förbättrat allmänt gränssnitt**

* Fältbeskrivningen, Lägg till i favoriter och Distribution av värdealternativ för schemaattribut är nu mer synlig i användargränssnittet. Mer information finns i den [detaljerade dokumentationen](../get-started/attributes.md).
* I gränssnittet visas nu datum och tid enligt det primära språk som angetts i inställningarna för Experience League. Den här förbättringen är bara tillgänglig för flera språk. En fullständig lista över vilka språk som stöds finns i [den detaljerade dokumentationen](https://experienceleague.adobe.com/sv/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**E-postredigerare**: För att förbättra tillgängligheten i webbgränssnittet för Campaign finns nu två nya fält i e-post-Designer: de motsvarar elementet `title` och språkattributet i elementet `html` i ditt e-postinnehåll. Du kan definiera de här inställningarna förutom fältet Förrubrik i delen Brödtext för e-post. Mer information finns i den [detaljerade dokumentationen](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Scheman**

* Du kan nu redigera det tillfälliga schemat för en lista från webbgränssnittet i Campaign. Mer information finns i den [detaljerade dokumentationen](../audience/manage-audience.md).
* Du kan nu förhandsgranska anpassade fält i ett schema på en exempelskärm. Mer information finns i den [detaljerade dokumentationen](../administration/custom-fields.md#add).
* Nu kan du flytta anpassade fält i listan genom att dra och släppa. Mer information finns i den [detaljerade dokumentationen](../administration/custom-fields.md#add).


### Nya funktioner i begränsad tillgänglighet {#25-4-features-la}

>[!AVAILABILITY]
>
>Följande funktioner är i Begränsad tillgänglighet (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö. De kräver en uppgradering av Campaign-servern till v8.7.4.
>
>Se följande dokumentationssidor: [Campaign Standard övergång till Campaign v8](../rn/acs-migration.md) och [Funktioner för Campaign Standard-användare](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=sv-SE).

* **Skapa flerspråkig leverans** - Nu kan du skicka flera e-postleveranser på olika språk i Adobe Campaign webbanvändargränssnitt. Med funktionen för flerspråkig leverans kan du välja standardspråk för leveransen samt de olika språk som leveransen kan skickas till. Du kan även förhandsgranska leveransen på de språk du har valt. Mer information finns i den [detaljerade dokumentationen](../email/edit-content.md).

* **Dynamisk rapportering för flerspråkiga** - Dynamisk rapportering är nu tillgänglig för flerspråkiga e-postleveranser. Mer information finns i den [detaljerade dokumentationen](../reporting/global-reports.md).

* **Stöd för SMS REST API (LA)** - Transactional Messaging REST API är nu tillgängligt för SMS-kanalen. När både e-post och mobilePhone finns i nyttolasten kan du använda fältet&quot;önskekanal&quot; för att ange kanalen. Om det inte anges används e-post som standard, såvida inte önskadChannel uttryckligen begär SMS. Mer information finns i den [detaljerade dokumentationen](https://experienceleague.adobe.com/sv/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

