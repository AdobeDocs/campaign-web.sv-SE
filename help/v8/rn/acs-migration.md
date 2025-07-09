---
audience: end-user
title: Övergång från Campaign Standard till Adobe Campaign Web
description: Upptäck webbanvändargränssnittet för kampanj
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 4%

---

# Campaign Standard övergång till Campaign v8 {#acs-to-ac}

Adobe Campaign Standard-användare har nu rätt att gå över till Adobe Campaign Managed Cloud Services v8. Den här övergången har flera fördelar:

* **Robust IT-infrastruktur**: Hanterade molntjänster v8 erbjuder en mer robust IT-infrastruktur, vilket ger bättre prestanda, tillförlitlighet och skalbarhet för kampanjer.
* **Förbättrat stöd**: Managed Cloud Services-teamet erbjuder hjälp i toppklass för att säkerställa en smidig övergång och kontinuerlig plattformsövervakning. Supporten omfattar felsökning och förebyggande underhåll.
* **Integrering med Adobe Experience Platform**: Hanterade molntjänster v8 är sömlöst sammankopplade med Adobe Experience Platform, vilket gör att användare kan utnyttja sina data fullt ut och leverera personaliserade, slagkraftiga kampanjer i alla kanaler.
* **Konsekvent användargränssnitt och upplevelse**: Övergången till hanterade molntjänster v8 stör inte arbetsflödena. Användarna fortsätter att dra nytta av det välbekanta gränssnittet och den välbekanta upplevelsen, vilket minimerar inlärningskurvan för team.

**Lär dig hur du startar [i det här dokumentet](../../adoption/home.md) när en Campaign Standard-användare övergår till Campaign v8.**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Viktiga funktioner {#key-features}

Användare av Campaign v8 har tillgång till både det nya webbgränssnittet för Campaign och v8-konsolen. Data och inställningar synkroniseras mellan miljöer. Alla data och inställningar som är tillgängliga i klientkonsolen visas i användargränssnittet för Campaign-webben, som du kommer åt via vänster navigering i Utforskaren. [Läs mer](../get-started/user-interface.md#user-interface-explorer)

Användargränssnittet för Campaign-webben är utformat för att marknadsförare enkelt ska kunna skapa och samordna kampanjer. Viktiga funktioner i webbgränssnittet Campaign v8 är bland annat:

* **Modern, vänlig och enhetlig upplevelse**. [Läs mer](../get-started/connect-to-campaign.md).
* **Nya kraftfulla funktioner och smidiga processer**. [Läs mer](../get-started/user-interface.md).
* **Förenklad och intuitiv frågemodellerare**. [Läs mer](../query/query-modeler-overview.md).
* **Inbyggda funktioner för kanalövergripande kampanjhantering**. [Läs mer](../msg/gs-messages.md).
* **Omdesignade kampanjarbetsflödesaktiviteter**. [Läs mer](../workflows/gs-workflows.md).
* **Skapa och hantera profiler enkelt**. [Läs mer](../audience/about-recipients.md).
* **Fördefinierade filter**. [Läs mer](../get-started/predefined-filters.md).
* **HTML Converter för e-postdesign**. [Läs mer](../email/existing-content.md).
* **SMS med erbjudanden**. [Läs mer](../msg/offers.md).

Campaign-klientkonsolen är utformad för administratörer och utvecklare för att konfigurera och anpassa sin miljö. De nyckelfunktioner som är tillgängliga i Campaign-klientkonsolen beskrivs i [den här dokumentationen](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Lär dig mer om funktioner som stöds och som inte stöds, och interoperabilitet mellan användargränssnittet för Campaign-webben och klientkonsolen [i Campaign på den här sidan](../get-started/capability-matrix.md).

## Terminologi {#terminology}

De flesta koncept är lika i Campaign v8 och Campaign Standard. Det finns dock några terminologiska skillnader. Exempel:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Specifika funktioner {#new-features}

För att övergången till Campaign v8 ska bli så smidig som möjligt har viktiga Campaign Standard-funktioner lagts till i Campaign v8. Dessa funktioner beskrivs i [den här dokumentationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=sv-SE){target=_blank} och är endast tillgängliga för användare som går över från Campaign Standard.

* **Dynamisk rapportering**: Dynamisk rapportering tillhandahåller anpassningsbara realtidsrapporter för att mäta effekten av marknadsföringsaktiviteter. Det innefattar tillgång till profildata för demografiska analyser utifrån dimensioner som kön, stad och ålder, tillsammans med funktionella e-postkampanjdata som öppningar och klick. [Läs mer](../reporting/dynamic-reporting/get-started-reporting.md).

* **Centraliserad varumärkesprofilering**: Med Adobe Campaign kan företag definiera riktlinjer för varumärkets visuella och tekniska egenskaper. Användarna kan presentera ett konsekvent varumärke för kunderna, från logotyper till tekniska aspekter som e-postavsändare, URL-adress eller domäner. [Läs mer](../administration/branding/branding-gs.md).

* **REST API:er**: Campaign Standard migrerade användare kan använda REST API:er för att skapa integreringar för Adobe Campaign och skapa ekosystem genom att interagera Adobe Campaign med andra tekniker. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target="_blank"}.

* **Landningssidor**: Startsidor för Campaign v8 innehåller förbättringar för att säkerställa funktionsparitet med Campaign Standard. Läs mer i [versionsinformationen](../rn/release-notes.md#new-24-4) och [dokumentationen](../landing-pages/get-started-lp.md) på landningssidan.

* **Visuella fragment**: Visuella fragment är återanvändbara visuella komponenter som refereras i en eller flera e-postleveranser eller innehållsmallar. När du ändrar ett fragment uppdateras allt innehåll som använder det. Med den här funktionen kan marknadsföringsanvändare förskapa flera anpassade innehållsblock för snabb meddelandesammanställning i en förbättrad designprocess. [Läs mer](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->