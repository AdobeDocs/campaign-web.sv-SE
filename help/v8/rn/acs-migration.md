---
audience: end-user
title: Övergång från Campaign Standard till Adobe Campaign Web
description: Upptäck webbanvändargränssnittet för kampanj
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 448b002a284b05000da80fd165b300bc24178c78
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 3%

---

# Campaign Standard över till Campaign v8 {#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

Välkommen till Adobe Campaign Managed Cloud Services v8!

Vi är glada över att kunna meddela att Adobe Campaign Standard-användare nu har rätt att gå över till Adobe Campaign Managed Cloud Services v8. Den här övergången ger många fördelar:

* Robust IT-infrastruktur: Med hanterade Cloud Service v8 kan kunderna utnyttja en mer robust IT-infrastruktur och få bättre prestanda, tillförlitlighet och skalbarhet för sina kampanjer.
* Förbättrat stöd: Vårt team för hanterade Cloud Service är fast beslutna att tillhandahålla förstklassig hjälp för att säkerställa en smidig övergång och kontinuerlig övervakning av din plattform. Från felsökning till förebyggande underhåll - vi har det du behöver.
* Integrering med Adobe Experience Platform: Hanterade Cloud Service v8 kan smidigt kopplas samman med Adobe Experience Platform, vilket ger kunderna möjlighet att utnyttja sina data fullt ut och leverera personaliserade, slagkraftiga kampanjer i alla kanaler.
* Enhetligt användargränssnitt och enhetlig upplevelse: Säkerställ att övergången till hanterade Cloud Service v8 inte stör ditt arbetsflöde. Du kommer att fortsätta använda det välbekanta användargränssnittet och användarupplevelsen, vilket ger en minimal inlärningskurva för ditt team.

## Viktiga funktioner {#key-features}

Som Campaign v8-användare har du tillgång till både det nya webbgränssnittet för Campaign och v8-konsolen. Data och inställningar synkroniseras från en miljö till en annan. Alla data och inställningar som är tillgängliga i klientkonsolen visas i användargränssnittet för Campaign-webben, från vänster navigering i Utforskaren. [Läs mer](../get-started/user-interface.md#user-interface-explorer)

Kampanjens webbgränssnitt är utformat för att marknadsförarna enkelt ska kunna skapa och samordna sina kampanjer. Låt oss fördjupa oss i vilka nyckelfunktioner webbgränssnittet Campaign v8 kommer att erbjuda:

* Modern, vänlig och enhetlig upplevelse. [Läs mer](../get-started/connect-to-campaign.md).
* Nya kraftfulla funktioner och smidiga processer. [Läs mer](../get-started/user-interface.md)
* Ny förenklad och intuitiv frågemodellerare. [Läs mer](../query/query-modeler-overview.md)
* Inbyggda funktioner för kanalövergripande kampanjhantering. [Läs mer](../msg/gs-messages.md)
* Nya och omarbetade kampanjarbetsflödesaktiviteter. [Läs mer](../workflows/gs-workflows.md)
* Enkelt att skapa och hantera profiler. [Läs mer](../audience/about-recipients.md)
* Fördefinierade filter. [Läs mer](../get-started/predefined-filters.md)
* HTML Converter för e-postdesign. [Läs mer](../email/existing-content.md)
* SMS med erbjudanden. [Läs mer](../msg/offers.md)

Campaign-klientkonsolen är utformad för administratörer och utvecklare för att konfigurera och anpassa sin miljö. De nyckelfunktioner som är tillgängliga i Campaign-klientkonsolen beskrivs i [den här dokumentationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Läs mer om funktioner som stöds och som inte stöds samt interoperabilitet mellan användargränssnittet i Campaign på webben och klientkonsolen för Campaign [på den här sidan](../get-started/capability-matrix.md)
>

## Terminologi {#terminology}

De flesta koncept är lika mellan Campaign v8 och Campaign Standard. Det finns dock några skillnader. Här är några exempel på skillnader i terminologi mellan Campaign Standard och Campaign v8:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* Resurser och anpassade resurser är **Scheman** och **Anpassade scheman**
* Meddelanden kallas **Leveranser**
* Roller har konfigurerats med **namngivna rättigheter**
* Säkerhetsgrupperna är **Operatorgrupper**
* Organisationsenheter hanteras via **Mappbehörigheter**
* Produktanvändare är **Operatorer** i klientkonsolen
* Leveransförberedelsen är **leveransanalysen** i klientkonsolen

## Specifika funktioner {#new-features}

För att ni smidigt ska kunna gå över till Campaign v8 har de viktigaste funktionerna för Campaign Standard lagts till i Campaign v8. De beskrivs i [den här dokumentationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"} och är endast tillgängliga för användare som övergår från Campaign Standard.

* **Dynamisk rapportering**: Dynamisk rapportering ger helt anpassningsbara realtidsrapporter för att mäta effekten av dina marknadsföringsaktiviteter. Det ger åtkomst till profildata, vilket möjliggör demografiska analyser efter profildimensioner som kön, ort och ålder, utöver funktionella e-postkampanjdata som öppningar och klick. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html){target="_blank"}.

* **Centraliserad varumärkesprofilering**: Alla företag har grafiska och tekniska riktlinjer för varumärken. Med Adobe Campaign kan ni definiera en uppsättning specifikationer för att presentera ett konsekvent varumärke för era kunder, från logotyper till tekniska aspekter som e-postavsändare, URL-adress eller domäner. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Resterande API:er** - Som en migrerad användare av Campaign Stardard kan du använda Rest API:er för att skapa integreringar för Adobe Campaign och skapa ett eget ekosystem genom att interagera med Adobe Campaign med den panel med tekniker som du använder. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.

* **Landningssidor** - Vissa förbättringar har gjorts på landningssidor för Campaign v8 för att säkerställa funktionens paritet med Campaign Standard. Läs mer i [versionsinformationen](../rn/release-notes.md#new-24-4) och [dokumentationen](../landing-pages/get-started-lp.md) på landningssidan.

* **Visuella fragment** - Visuella fragment är återanvändbara visuella komponenter som kan refereras i en eller flera e-postleveranser eller i innehållsmallar. När du ändrar ett fragment uppdateras allt innehåll som använder det. Med den här funktionen kan man skapa flera anpassade innehållsblock som kan användas av marknadsföringsanvändare för att snabbt sammanställa meddelandeinnehåll i en förbättrad designprocess. [Läs mer](../content/use-visual-fragments.md)

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->
