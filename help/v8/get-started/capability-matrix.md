---
audience: end-user
title: Funktionsmatris för kampanjwebbgränssnitt/klientkonsol
description: Lista över funktioner som stöds i Campaign Web-gränssnittet
hide: true
hidefromtoc: true
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 3c011a8f0958b7d0875fc18ec59309ef4b1f4103
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 0%

---

# Funktionsmatris för kampanjwebbgränssnitt/klientkonsol {#capabilities-matrix}

De viktigaste Campaign-funktionerna finns i gränssnittet för Campaign-webben. Det här gränssnittet var primärt utformat för att marknadsförarna ska kunna planera, lansera och mäta sina marknadsföringskampanjer. Alla funktioner listas [på den här sidan](../rn/whats-new.md).

Anpassning av kampanjplattform baserat på affärs- och databehov, och anslutning till andra system hanteras i Campaign-klientkonsolen. Därför kan vissa inställningar och funktioner bara nås, skapas eller hanteras från Campaign Client Console. Vissa kommer att vara tillgängliga i en senare uppdatering av användargränssnittet i Campaign Web.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Campaign Management {#campaign-mgt-capabilities}

Med Campaign Web-gränssnittet kan ni skapa kampanjer i flera kanaler som detaljerade [i det här avsnittet](../campaigns/gs-campaigns.md). Följande funktioner är bara tillgängliga i Campaign-klientkonsolen. De är inte tillgängliga i gränssnittet för Campaign-webben, men vissa kan visas från [Utforskarmenyn](user-interface.md#user-interface-explorer).

Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och lär dig hur du använder dessa funktioner.

* Marknadskalender. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#campaign-calendar){target="_blank"}
* Program och planer. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#work-with-plan-and-program){target="_blank"}
* Leverantörer, budget och kostnadshantering. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html){target="_blank"}
* Distribuerad marknadsföring (Central/Local marketing). [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html){target="_blank"}
* Marknadsföringsresurshantering, mål, simuleringar och kostnadskontroll. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html){target="_blank"}
* Uppgiftshantering. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html){target="_blank"}

## Kommunikationskanaler {#channels-capabilities}

Med användargränssnittet i Campaign Web kan du skapa, utforma och skicka e-post, SMS och push-meddelanden och mäta deras effekt med hjälp av olika dedikerade rapporter, som detaljerade [i det här avsnittet](../msg/gs-messages.md). Följande kanaler är dock för närvarande inte tillgängliga.

Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om dessa kanaler.

* Direktreklam. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-direct-mail/about-direct-mail-channel.html){target="_blank"}
* LINE-meddelanden. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html){target="_blank"}
* Anropscenter och Egna kanaler. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html#other-channels){target="_blank"}
* Social marknadsföring med X (Twitter). [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html){target="_blank"}

## Landningssidor och webbprogram {#Webapps-capabilities}

Med Adobe Campaign kan du skapa, designa och dela landningssidor. landningssidornas upplevelse har omdesignats helt i det nya gränssnittet. Upptäck hur du skapar, utformar och publicerar landningssidor i Campaign Web-gränssnittet [i det här avsnittet](../landing-pages/get-started-lp.md).

I Campaign-klientkonsolen kan du därför inte redigera, uppdatera eller ändra en landningssida som skapats i webbgränssnittet - och omvänt. Följande typer av webbprogram är inte tillgängliga i gränssnittet för Campaign-webben. De visas dock i listan över landningssidor. Använd länkarna för att bläddra i dokumentationen för Campaign Classic v7 och läs mer om dessa webbprogram:

* Webbprogram. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html){target="_blank"}
* Webbformulär. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html){target="_blank"}
* Onlineundersökningar. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html){target="_blank"}


## Profiler, testprofiler och målgrupper {#profiles-audiences-capabilities}

Du kan skapa, hantera och uppdatera profiler och testprofiler i både Campaign-klientkonsolen och Campaign-webbgränssnittet. Alla ändringar som görs i det ena gränssnittet visas i det andra. Vissa specifika mottagarinställningar och avancerade parametrar kan saknas i det nya webbgränssnittet för Campaign. Observera att termen &quot;mottagare&quot; har ändrats till &quot;profil&quot; i det nya webbgränssnittet.

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Alla målgrupper som skapats i Campaign-klientkonsolen eller i Adobe Experience Platform finns tillgängliga i Campaign Web-gränssnittet.

Import-/exportjobb i ett enda foto enligt beskrivningen i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html#import-jobs){target="_blank"} är inte tillgängliga i Campaign Web-användargränssnittet. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## Transaktionsmeddelanden {#mc-capabilities}

Funktioner för transaktionsmeddelanden som ingår i produktpaketet Message Center är för närvarande inte tillgängliga i det nya användargränssnittet för Campaign-webben.

Sök i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} och läs mer om meddelandefunktioner i realtid, som:

* Redigering och körning av meddelanden i realtid via e-post, SMS och push
* Berikning och personalisering av meddelanden
* Utlösare (övergivna Adobe Analytics-varukorgar)
* Rapportering och övervakning av transaktionsmeddelanden

## Innehållsdesign {#content-capabilities}

Med det nya e-postdesignern som kommer med Adobe Campaign webbgränssnitt kan du enkelt skapa engagerande, individuellt anpassade e-postmeddelanden via ett intuitivt dra och släpp-gränssnitt. Oavsett om du börjar på en tom sida, importerar ett befintligt innehåll eller använder befintliga mallar kan du utforma och förfina allt innehåll för varje e-postmeddelande. [Läs mer](../email/edit-content.md)

Med det nya användargränssnittet kan du hantera synkronisering av e-postmallar från Adobe Experience Manager och integrera med Adobe Experience Manager as a Cloud Service.

Observera att följande funktioner för tillfället inte är tillgängliga i gränssnittet för Campaign-webben. Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om dessa funktioner.

* Skapa anpassade personaliseringsblock. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}
* Innehåll från anpassade formulär (modulen Innehållshantering). [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html){target="_blank"}
* AMP för e-post. [Läs mer i dokumentationen för Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Typologier och typologiregler {#rules-capabilities}

Typologier är uppsättningar typologiregler som utförs under förberedelsefasen för att enkelt tillämpa flera filtreringsregler på en leverans samtidigt. De gör att marknadsförarna kan standardisera sina rutiner för alla leveranser när de kan styra, filtrera och prioritera leveransen.

Typologiregler kan väljas för en leverans, eller en leveransmall, i webbgränssnittet för Campaign, som detaljerade [i det här avsnittet](../advanced-settings/delivery-settings.md#typology). Regler och typologiregler kan dock bara skapas, hanteras och anpassas i Campaign-klientkonsolen.

Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om typologiregler:

* Skapa kontrollregler. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
* Trötthet/tryckregler. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}
* Skapa filtreringsregler. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* Hantering av typologiregler. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
* Kampanjsimulering. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
* Javascript-kodning för framtagning av typologiregler. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}

## Arbetsflöden {#wf-capabilities}

Det nya gränssnittet Campaign Web ger ett nytt arbetsflödesgränssnitt där du kan utforma och hantera processer. Viktiga arbetsflödesaktiviteter är redan tillgängliga i den nya designen, andra kommer i en framtida uppdatering. Läs mer om arbetsflödets funktioner, inklusive säkerhetsutkast och begränsningar [i det här avsnittet](../get-started/guardrails.md).

Observera att följande funktioner endast är tillgängliga i Campaign-klientkonsolen:

* Skript i arbetsflöden
* ETL-aktiviteter: Export, Redigera schema, Datainläsning, Datainhämtning, SQL-kod

Läs mer om tillgängliga arbetsflödesaktiviteter i arbetsflödesdokumentationen för Adobe Campaign v8 (konsol) [här](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html){target="_blank"}.

## Erbjudandehantering {#offer-capabilities}

Med Adobe Campaign Web kan du skicka med leveranserbjudanden som har skapats i konsolen via **[!UICONTROL Interaction]** -modul. Erbjudandeutformning, regler för behörighet och erbjudandehantering är bara tillgängligt i Campaign-klientkonsolen. [Läs mer](../msg/offers.md)

Lär dig hur du hanterar en erbjudandekatalog i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

## Integrering med Adobe Experience Cloud lösningar {#exc-capabilities}

Det nya moderna gränssnittet för Campaign förenklar utformningen och leveransen av marknadsföringskampanjer och ger enhetlighet tillsammans med andra Adobe-lösningar, inklusive Adobe Experience Platform och Adobe Experience Manager.

Följande integreringar är tillgängliga från Adobe Campaign klientkonsol och är ännu inte tillgängliga i Campaign Web-gränssnittet. Använd länkarna för att bläddra i dokumentationen för Campaign v8 (klientkonsolen) och läs mer om dessa integreringar:

* Adobe Analytics dataanvändning och KPI-delning. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html){target="_blank"}
* Målgruppsdelning med Adobe Experience Cloud (Adobe Audience Manager). [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html){target="_blank"}
* Integrering med Adobe Target. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html){target="_blank"}
* Integrering med Adobe Experience Cloud Triggers. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html){target="_blank"}

## Rapportering {#reporting-capabilities}

Det nya gränssnittet för Campaign-webben innehåller en uppsättning nya rapporter och nyckeltal för alla kanaler: leveransrapporter, kampanjrapporter och globala rapporter. Läs mer [i det här avsnittet](../reporting/gs-reports.md)

Vissa funktioner är bara tillgängliga från klientkonsolen. Bläddra bland länkarna för att bläddra bland [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=sv){target="_blank"} och lär dig mer.

* Inbyggd leveransrapport och inkorgsåtergivning. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html){target="_blank"}
* Anpassa rapporter. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html){target="_blank"}
* Beskrivande analys. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html){target="_blank"}
* Kampanjanalys/kubrapporter. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html){target="_blank"}
* Rapportera delning enligt schema som PDF och CSV, eller länk. [Läs mer](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html){target="_blank"}

## Datamodellering och datainmatning {#data-capabilities}

Kampanjwebbgränssnittet har inte följande funktioner. De är bara tillgängliga i klientkonsolen.

Bläddra bland länkarna i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=sv){target="_blank"} och lär dig mer.

* Externa konton. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html){target="_blank"}
* Skapande och tillägg av schema. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html){target="_blank"}
* Arbetsflödesaktiviteter för datahantering: Datainläsning, extrahering (fil), Uppdatera data, Redigera schema, Tekniska arbetsflöden för import/export. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#data-management){target="_blank"}
* Kampanjkonfiguration och anslutning till externa system. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html){target="_blank"}

## Godkännanden {#approvals-capabilities}

Användargränssnittet för Campaign-webben hanterar inte godkännande av innehåll, leveranser, arbetsflöden, kampanjer och mål. De är bara tillgängliga i klientkonsolen.

Lär dig hur du hanterar godkännanden i arbetsflöden i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html){target="_blank"}.


Lär dig hantera leverans, innehåll och målgodkännanden i kampanjer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html){target="_blank"}.


## Behörigheter {#permissions-capabilities}

Kampanjanvändare har bara åtkomst till gränssnittet i Campaign-webben via Adobe ID via Adobe Identity Management System (IMS). Behörigheter som ges till användare gäller även i användargränssnittet för Campaign-webben.

Behörigheterna definieras i Adobe Admin Console och Adobe Campaign klientkonsol som detaljerade [i det här avsnittet](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html). Behörighetsåtgärder kan inte utföras via Adobe Campaign webbgränssnitt.


## Övervakning {#monitoring-capabilities}

Övervakningskapaciteten för Campaign-plattformen är bara tillgänglig i klientkonsolen och på Campaign-kontrollpanelen. De visas inte i gränssnittet för Campaign-webben.

Bläddra bland länkarna till dokumentationen för Campaign v8 (klientkonsolen) och kontrollpanelen om du vill veta mer.

* [Arbetsflödesövervakning](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html){target="_blank"}
* [Värmekarta för arbetsflöde](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html){target="_blank"}
* [Prestandaövervakning](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=sv){target="_blank"}
* [Övervakning av leveransen](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html){target="_blank"}




