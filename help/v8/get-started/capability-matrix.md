---
audience: end-user
title: Funktionsmatris för kampanjwebbgränssnitt/klientkonsol
description: Lista över funktioner som stöds i Campaign Web-gränssnittet
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '2133'
ht-degree: 3%

---

# Campaign Web and Campaign Client Console {#capabilities-matrix}

De viktigaste Campaign-funktionerna finns i gränssnittet för Campaign-webben. Gränssnittet är främst utformat för att marknadsförarna ska kunna planera, lansera och mäta sina marknadsföringskampanjer. Alla funktioner visas [på den här sidan](../rn/whats-new.md).

Anpassning av kampanjplattform baserat på affärs- och databehov, och anslutning till andra system, hanteras i Campaign-klientkonsolen. Därför kan vissa inställningar och funktioner bara kommas åt, skapas eller hanteras från Campaign-klientkonsolen. Vissa kommer att vara tillgängliga i en senare uppdatering av användargränssnittet för Campaign-webben.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Kampanjhantering {#campaign-mgt-capabilities}

Med Campaigns webbgränssnitt kan du skapa kampanjer i flera kanaler, vilket beskrivs närmare i [det här avsnittet](../campaigns/gs-campaigns.md). Följande funktioner är bara tillgängliga i Campaign-klientkonsolen. De är inte tillgängliga i Campaign Web-användargränssnittet, men vissa kan visas på [Utforskarmenyn](user-interface.md#user-interface-explorer).

Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och lär dig hur du använder dessa funktioner.

* **Marknadskalender**. Kampanjkalendern visar alla program, planer, kampanjer och leveranser i en global tidslinje. Den här funktionen är bara tillgänglig i klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=sv-SE#campaign-calendar){target="_blank"}
* **Program och planer**. Varje kampanj tillhör ett program som tillhör en plan. I gränssnittet för Campaign-webben är alla kampanjer kopplade till en inbyggd standardplan och ett standardprogram. Du kan bara skapa och hantera planer och program i klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=sv-SE#work-with-plan-and-program){target="_blank"}
* **Providers, budget och kostnadshantering**. Ni kan konfigurera tjänsteleverantörer som deltar i de jobb som utförs inom era kampanjer, inklusive kostnadsstrukturer, och hantera budgeten inom varje program och kampanj. Den här funktionen är bara tillgänglig i klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=sv-SE){target="_blank"}
* **Distribuerad marknadsföring** (Central/lokal marknadsföring). Adobe Campaign erbjuder en app för distribuerad marknadsföring för att genomföra kampanjer mellan centrala enheter (huvudkontor, marknadsföringsavdelningar och andra) och lokala enheter (säljställen, regionala myndigheter och andra). Den här funktionen är bara tillgänglig i klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=sv-SE){target="_blank"}
* **Hantering av marknadsföringsresurser** (MRM), mål, simuleringar och kostnadskontroll. Adobe Campaign erbjuder en MRM-app (Marketing Resource Management) som gör att ni kan styra marknadsföringsåtgärder i ett samverkansbaserat läge genom att tillhandahålla fullständig hantering och realtidsspårning av de uppgifter, budgetar och marknadsföringsresurser som ingår. Den här funktionen är bara tillgänglig i klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=sv-SE){target="_blank"}
* **Aktivitetshantering**. Som en del av MRM-appen kan kampanjaktiviteter skapas, tilldelas, spåras och övervakas från kontrollpanelen för kampanjer. Den här funktionen är bara tillgänglig i klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=sv-SE){target="_blank"}

## Kommunikationskanaler {#channels-capabilities}

Med Campaigns webbgränssnitt kan du skapa, utforma och skicka **e-post**, **SMS**, **push-meddelanden**, **direktreklam** och mäta deras effekt med hjälp av olika dedikerade rapporter, vilket beskrivs närmare i [det här avsnittet](../msg/gs-messages.md). Följande kanaler är för närvarande **inte** tillgängliga: i appen, LINE, Call center/Custom channel, social marknadsföring med X (Twitter).

Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om dessa kanaler.

* **LINJESMEDDELANDE**. LINE är ett program för kostnadsfria snabbmeddelanden, röst- och videosamtal som finns på alla mobila enheter och på datorn. I Adobe Campaign kan du endast skicka LINE-meddelanden från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=sv-SE){target="_blank"}
* **Anropscenter och anpassade kanaler**. Call center och andra anpassade kanaler kan implementeras i er Campaign-miljö. Dessa kanaler är bara tillgängliga i klientkonsolen. [Läs mer i Campaign Classic v7-dokumentationen](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=sv-SE#other-channels){target="_blank"}
* **Social marknadsföring** med X (Twitter). Ni interagerar med era kunder via X (Twitter) genom att skicka meddelanden och direktmeddelanden. Den här funktionen, som kommer med tillägget Social Marketing, är bara tillgänglig från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=sv-SE){target="_blank"}

## Landningssidor och webbprogram {#Webapps-capabilities}

Med Adobe Campaign kan du skapa, designa och dela landningssidor. landningssidornas upplevelse har omdesignats helt i det nya gränssnittet. Upptäck hur du skapar, utformar och publicerar landningssidor i gränssnittet [för Campaign-webben i det här avsnittet](../landing-pages/get-started-lp.md).

I klientkonsolen för Campaign kan du alltså inte redigera, uppdatera eller ändra en landningssida som skapats i webbgränssnittet, och vice versa. Följande typer av webbprogram är inte tillgängliga i Campaign Web-användargränssnittet. De visas dock i listan över landningssidor. Använd länkarna för att bläddra i dokumentationen för Campaign Classic v7 och läs mer om dessa webbprogram:

* **Webbprogram**. Med Adobe Campaign kan du skapa och publicera dynamiska och interaktiva webbapplikationer med förinlästa data från databasen och innehåll som är anpassat efter den anslutna användarens rättigheter. Den här funktionen är bara tillgänglig i klientkonsolen. [Läs mer i Campaign Classic v7-dokumentationen](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=sv-SE){target="_blank"}
* **Webbformulär**. Webb- och landningssidor som är utformade i klientkonsolen visas i gränssnittet för webbkampanjen, men kan inte redigeras eller ändras. Vissa alternativ kan skilja sig åt mellan klientkonsolens webbsidesigner och landningssidans designer som kommer med gränssnittet för webben i Campaign. [Läs mer i Campaign Classic v7-dokumentationen](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=sv-SE){target="_blank"}
* **Onlineundersökningar**. Du kan endast skapa onlinesenkäter och samla in svar från klientkonsolen. Den här funktionen är inte tillgänglig i gränssnittet för Campaign-webben. [Läs mer i Campaign Classic v7-dokumentationen](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=sv-SE){target="_blank"}

## Profiler, testprofiler och målgrupper {#profiles-audiences-capabilities}

Du kan skapa, hantera och uppdatera profiler och testprofiler i både Campaign-klientkonsolen och Campaign-webbgränssnittet. Alla ändringar som görs i det ena gränssnittet visas i det andra. Vissa specifika mottagarinställningar och avancerade parametrar kanske saknas i det nya webbgränssnittet för Campaign.

Observera att termen &quot;mottagare&quot; har ändrats till &quot;profil&quot; i det nya webbgränssnittet, och &quot;dirigerade adresser&quot; är nu &quot;Testa profiler&quot;.

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Alla målgrupper som skapats i Campaign-klientkonsolen eller i Adobe Experience Platform är tillgängliga i Campaign Web-användargränssnittet.

Import-/exportjobb med en bild, som beskrivs i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=sv-SE#import-jobs){target="_blank"}, är inte tillgängliga i webbgränssnittet för Campaign. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html?lang=sv-SE){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## Innehållsdesign {#content-capabilities}

Med det nya e-postgränssnittet i Designer som medföljer Adobe Campaign webbgränssnitt kan du enkelt skapa engagerande, individuellt anpassade e-postmeddelanden via ett intuitivt dra och släpp-gränssnitt. Oavsett om du börjar på en tom sida, importerar befintligt innehåll eller använder befintliga mallar kan du utforma och förfina allt innehåll för varje e-postmeddelande. [Läs mer](../email/edit-content.md)

Med det nya användargränssnittet kan du hantera synkronisering av e-postmallar från Adobe Experience Manager och integrera med Adobe Experience Manager as a Cloud Service.

Observera att följande funktioner för tillfället inte är tillgängliga i gränssnittet för Campaign-webben. Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om dessa funktioner.

* **Skapa anpassade anpassningsblock**. Förutom standardanpassningsblocken kan du skapa anpassade block från klientkonsolen. Den här funktionen är inte tillgänglig i gränssnittet för Campaign-webben. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=sv-SE#create-custom-personalization-blocks){target="_blank"}
* **Innehåll från anpassade formulär**. Med innehållshanteringsmodulen kan du skapa och hantera formulär som hjälper dina användare när de skapar innehåll i Campaign. Den här funktionen är bara tillgänglig med klientkonsolen. [Läs mer i Campaign Classic v7-dokumentationen](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=sv-SE){target="_blank"}
* **AMP för e-post**. Med AMP for Email-formatet kan du inkludera AMP-komponenter i dina meddelanden och förbättra e-postupplevelsen med avancerat och användbart innehåll. Den här funktionen är bara tillgänglig i klientkonsolen. [Läs mer i Campaign Classic v7-dokumentationen](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=sv-SE){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Typologier och typologiregler {#rules-capabilities}

Typologier är uppsättningar typologiregler som körs under förberedelsefasen för att enkelt tillämpa flera filtreringsregler på en leverans samtidigt. De gör det möjligt för marknadsförarna att standardisera affärspraxis för alla leveranser genom att styra, filtrera och prioritera utskick av leveranser.

Typologiregler kan väljas för en leverans eller en leveransmall i webbgränssnittet för Campaign, vilket beskrivs [i det här avsnittet](../advanced-settings/delivery-settings.md#typology). Regler och typologiregler kan dock bara skapas, hanteras och anpassas i Campaign-klientkonsolen.

Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om typologiregler:

<!--
* Control rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=sv-SE){target="_blank"}
-->
* Skapa trötthets-/tryckregler. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=sv-SE){target="_blank"}
<!--
* Filtering rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=sv-SE){target="_blank"}
* Typology rules management. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=sv-SE){target="_blank"}
-->
* Kampanjsimulering. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=sv-SE){target="_blank"}
<!--
* JavaScript coding for typology rules authoring. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=sv-SE#use-cases-on-pressure-rules){target="_blank"}
-->

## Arbetsflöden {#wf-capabilities}

Det nya gränssnittet Campaign Web ger ett nytt arbetsflödesgränssnitt där du kan utforma och hantera processer. Viktiga arbetsflödesaktiviteter är redan tillgängliga i deras nya design, och vissa kommer att ingå i en framtida uppdatering. Läs mer om arbetsflödesfunktioner, inklusive skyddsutkast och begränsningar, [i det här avsnittet](../get-started/guardrails.md).

Observera att följande funktioner endast är tillgängliga i Campaign-klientkonsolen:

<!--
* Scripting in workflows
-->

* ETL-aktiviteter: Export, Redigera schema, Datainläsning, Datainhämtning, SQL-kod

Läs mer om tillgängliga arbetsflödesaktiviteter i arbetsflödesdokumentationen för Adobe Campaign v8 (konsol) [här](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=sv-SE){target="_blank"}.

## Erbjudandehantering {#offer-capabilities}

Du kan skicka erbjudanden i leveranser som skapats i Adobe Campaign webbgränssnitt. Erbjudandena måste ha skapats i klientkonsolen med modulen **[!UICONTROL Interaction]**. Erbjudandeutformning, regler för behörighet och erbjudandehantering är endast tillgängliga i Campaign-klientkonsolen. [Läs mer](../msg/offers.md)

Lär dig hur du hanterar en erbjudandekatalog i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=sv-SE){target="_blank"}.

## Integrering med Adobe Experience Cloud lösningar {#exc-capabilities}

Det nya moderna gränssnittet Campaign förenklar utformningen och leveransen av marknadsföringskampanjer och ger enhetlighet tillsammans med andra Adobe-lösningar, inklusive Adobe Experience Platform och Adobe Experience Manager.

Följande integreringar är tillgängliga från Adobe Campaign klientkonsol och är ännu inte tillgängliga i Campaign Web-användargränssnittet. Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om dessa integreringar:

* Adobe Analytics dataanvändning och KPI-delning. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=sv-SE){target="_blank"}
* Målgruppsdelning med Adobe Experience Cloud (Adobe Audience Manager). [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=sv-SE){target="_blank"}
* Integrering med Adobe Target. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=sv-SE){target="_blank"}
* Integrering med Adobe Experience Cloud-utlösare. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=sv-SE){target="_blank"}

## Rapportering {#reporting-capabilities}

Det nya gränssnittet för Campaign-webben innehåller en uppsättning nya rapporter och nyckeltal för alla kanaler: leveransrapporter, kampanjrapporter och globala rapporter. Läs mer [i det här avsnittet](../reporting/gs-reports.md)

Vissa funktioner är bara tillgängliga från klientkonsolen. Bläddra bland länkarna till dokumentationen för [Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=sv){target="_blank"} och läs mer.

* Inbyggd leveransrapport och inkorgsåtergivning. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=sv-SE){target="_blank"}
* Anpassa rapporter. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=sv-SE){target="_blank"}
* Beskrivande analys. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=sv-SE){target="_blank"}
* Kampanjanalys-/kubrapporter. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=sv-SE){target="_blank"}
* Rapportera delning enligt schema som PDF och CSV, eller länk. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=sv-SE){target="_blank"}

## Datamodellering och datainmatning {#data-capabilities}

Kampanjwebbgränssnittet har inte följande funktioner. De är bara tillgängliga i klientkonsolen:

### Externa konton {#external}

Adobe Campaign har en uppsättning fördefinierade externa konton som kan anslutas till externa system. Som systemadministratör för en kampanj kan du skapa och hantera externa konton. [Läs mer](../administration/external-account.md)

### Skapande och tillägg av schema {#schema}

Framtagning, ändring och tillägg av scheman är begränsade till avancerade användare. Dessa funktioner är bara tillgängliga från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=sv-SE){target="_blank"}

### Funktioner för datahantering i arbetsflöden {#data}

Datahantering kombinerar en uppsättning aktiviteter för att lösa komplexa problem med målinriktning genom att erbjuda mer effektiva och flexibla verktyg som datainläsning, extrahering (fil), uppdateringsdata, redigeringsschema eller tekniska arbetsflöden för import/export. [Upptäck datahanteringsfunktioner för arbetsflöden i klientkonsolen](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=sv-SE#data-management){target="_blank"}

>[!NOTE]
>
>Vissa av dessa aktiviteter är bara tillgängliga i klientkonsolen, men vissa är tillgängliga i Campaign-webbgränssnittet, till exempel **Enrichment**, **Load file**, **Change data source** eller **Change dimension** . [Läs mer om målgruppsanpassning och datahanteringsaktiviteter i användargränssnittet för Campaign på webben](../workflows/activities/about-activities.md#targeting)

### Konfiguration för federerad dataåtkomst {#fda}

Kampanjkonfiguration och anslutning till externa system är begränsade till avancerade användare och är endast tillgängliga från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=sv-SE){target="_blank"}

## Godkännanden {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="Godkännandehantering"
>abstract="Godkännandehantering är bara tillgängligt från klientkonsolen. "

Användargränssnittet för Campaign-webben hanterar inte godkännande av innehåll, leveranser, arbetsflöden, kampanjer och mål. De är bara tillgängliga i klientkonsolen.

Lär dig hur du hanterar godkännanden i arbetsflöden i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=sv-SE){target="_blank"}.

Lär dig hur du hanterar leverans, innehåll och målgodkännanden i kampanjer i dokumentationen för [Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=sv-SE){target="_blank"}.

## Behörigheter {#permissions-capabilities}

Kampanjanvändare har endast åtkomst till gränssnittet för Campaign-webben via sin Adobe ID via Adobe Identity Management System (IMS). Behörigheter som ges till användare gäller även i gränssnittet för webbkampanjen.

Behörigheter definieras i Adobe Admin Console- och Adobe Campaign-klientkonsolen, vilket beskrivs närmare i [det här avsnittet](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=sv-SE). Behörighetsåtgärder kan inte utföras via Adobe Campaign webbgränssnitt.

## Övervakning {#monitoring-capabilities}

Funktioner för övervakning av kampanjplattformar är bara tillgängliga i klientkonsolen och Campaign Control-panelen. De visas inte i gränssnittet för Campaign-webben.

Bläddra bland länkarna till dokumentationen för Campaign v8 (klientkonsolen) och kontrollpanelen om du vill veta mer.

* [Arbetsflödesövervakning](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=sv-SE){target="_blank"}
* [Värmekarta för arbetsflöde](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=sv-SE){target="_blank"}
* [Prestandaövervakning](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=sv){target="_blank"}
* [Övervaka levererbarhet](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=sv-SE){target="_blank"}

## Hantering av tidszoner {#timezone-management}

Adobe Campaign Web UI visar alla datum- och tidsvärden baserat på den **lokala tidszonen i användarens webbläsare**. Detta kan leda till skillnader när tidsstämplar jämförs mellan webbgränssnittet och klientkonsolen.

Mer information om skillnaderna mellan tidszonerna för [webbgränssnittet](../administration/timezone-management.md), **klientkonsolen** och **arbetsflödeskörning** finns på **sidan**.
