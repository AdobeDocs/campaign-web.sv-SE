---
audience: end-user
title: Övergång från Campaign Standard till Adobe Campaign Web
description: Upptäck webbanvändargränssnittet för kampanj
source-git-commit: 4c1f68f0e89b2b84b8845b2759ef3b0dc9b12033
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 5%

---


# Campaign Standard över till Campaign v8{#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

Välkommen till Adobe Campaign Managed Cloud Services v8!

Vi är glada över att kunna meddela att Adobe Campaign Standard-användare nu har rätt att gå över till Adobe Campaign Managed Cloud Services v8. Den här övergången ger många fördelar:

* Robust IT-infrastruktur: Med hanterade Cloud Service v8 kan kunderna utnyttja en mer robust IT-infrastruktur och få bättre prestanda, tillförlitlighet och skalbarhet för sina kampanjer.
* Förbättrat stöd: Vårt team för hanterade Cloud Service är fast beslutna att tillhandahålla förstklassig hjälp för att säkerställa en smidig övergång och kontinuerlig övervakning av din plattform. Från felsökning till förebyggande underhåll - vi har det du behöver.
* Integrering med Adobe Experience Platform: Hanterade Cloud Service v8 kan smidigt kopplas samman med Adobe Experience Platform, vilket ger kunderna möjlighet att utnyttja sina data fullt ut och leverera personaliserade, slagkraftiga kampanjer i alla kanaler.
* Enhetligt användargränssnitt och enhetlig upplevelse: Säkerställ att övergången till hanterade Cloud Service v8 inte stör ditt arbetsflöde. Du kommer att fortsätta använda det välbekanta användargränssnittet och användarupplevelsen, vilket ger en minimal inlärningskurva för ditt team.

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Viktiga funktioner {#key-features}

Låt oss fördjupa oss i vilka nyckelfunktioner Campaign v8 kan erbjuda er:

* Modern, vänlig och enhetlig upplevelse. [Läs mer](../get-started/connect-to-campaign.md).
* Nya kraftfulla funktioner och smidiga processer. [Läs mer](../get-started/user-interface.md)
* Ny förenklad och intuitiv frågemodellerare. [Läs mer](../query/query-modeler-overview.md)
* Inbyggda funktioner för kanalövergripande kampanjhantering. [Läs mer](../msg/gs-messages.md)
* Nya och omarbetade kampanjarbetsflödesaktiviteter. [Läs mer](../workflows/gs-workflows.md)
* Målgrupp med frågemodelleraren. [Läs mer](../query/query-modeler-overview.md)
* Enkelt att skapa och hantera profiler. [Läs mer](../audience/about-recipients.md)
* AI-baserad sammanhangsbaserad hjälp. [Läs mer](../get-started/using-ai.md)
* Fördefinierade filter. [Läs mer](../get-started/predefined-filters.md)
* HTML Converter för e-postdesign. [Läs mer](../email/existing-content.md)
* SMS med erbjudanden. [Läs mer](../msg/offers.md)

## Konsol och webbgränssnitt {#console}

Som Campaign v8-användare har du tillgång till både det nya webbgränssnittet för Campaign och v8-konsolen. Data och inställningar synkroniseras från en miljö till en annan. Alla data och inställningar som är tillgängliga i klientkonsolen visas i användargränssnittet för Campaign-webben, från vänster navigering i Utforskaren. [Läs mer](../get-started/user-interface.md#user-interface-explorer)

Funktioner som stöds och som inte stöds samt interoperabilitet mellan användargränssnittet i Campaign på webben och klientkonsolen i Campaign [på den här sidan](../get-started/capability-matrix.md)

## Terminologi {#terminology}

De flesta koncept är desamma för Campaign-webbgränssnittet och -Campaign Standarden. Det finns dock några skillnader. Här är några exempel på skillnader i terminologi mellan Campaign Standard och Campaign-webbgränssnittet:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* Anpassade resurser är **Scheman** i Campaign-webbgränssnittet.
* Marknadsföringsaktiviteter finns inte längre.
* Meddelandena är **Leveranser**.
* Operatorerna är **Användare**.
* Namngivna rättigheter är **Roller**.
* Operatorgrupper är **Säkerhetsgrupper**.
* Mappbehörigheter är **Organisationsenheter**

## Nya funktioner {#new-features}

För att du ska kunna gå över har vi lagt till [nyckelfunktioner](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html) från Campaign Standard till v8:

* **Dynamisk rapportering**: Dynamic Reporting tillhandahåller fullt anpassningsbara realtidsrapporter för att mäta effekten av era marknadsföringsaktiviteter. Det ger åtkomst till profildata, vilket möjliggör demografiska analyser efter profildimensioner som kön, ort och ålder, utöver funktionella e-postkampanjdata som öppningar och klick. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Centraliserad branding**: Varje företag har grafiska och tekniska riktlinjer för varumärken. Med Adobe Campaign kan ni definiera en uppsättning specifikationer för att presentera ett konsekvent varumärke för era kunder, från logotyper till tekniska aspekter som e-postavsändare, URL-adress eller domäner. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Övriga API:er** - Som migrerad användare av Campaign Stardard kan ni använda Rest API:er för att skapa integreringar för Adobe Campaign och bygga ett eget ekosystem genom att interagera med Adobe Campaign med den panel med tekniker som ni använder. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Landningssidor** - Många förbättringar har gjorts i Campaign v8 för att säkerställa att ni inte förlorar någon kapacitet. Läs mer i [versionsinformation](../rn/release-notes.md#new-24-4) och landningssidan [dokumentation](../landing-pages/get-started-lp.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->