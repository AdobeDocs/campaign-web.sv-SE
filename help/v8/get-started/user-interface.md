---
audience: end-user
title: Upptäck gränssnittet
description: Adobe Campaign webbgränssnitt
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 7b04c6a9b425054690209bc3d3d8d0c29e038e31
workflow-type: tm+mt
source-wordcount: '1650'
ht-degree: 1%

---

# Upptäck gränssnittet {#user-interface}

Adobe Campaign nya webbgränssnitt är ett modernt och intuitivt gränssnitt som förenklar utformningen och leveransen av marknadsföringskampanjer. Det nya gränssnittet är integrerat med Adobe Experience Cloud program och lösningar.

Lär dig hur du ansluter till Adobe Campaign och upptäck Experience Cloud navigeringsgrunder [i den här artikeln](connect-to-campaign.md).


>[!NOTE]
>
>Den här dokumentationen uppdateras ofta för att återspegla de senaste ändringarna i produktanvändargränssnittet. Vissa skärmbilder kan dock skilja sig något från användargränssnittet.

## Startsida för kampanj {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Senaste"
>abstract="The **Senaste** listan innehåller genvägar till de nyligen skapade och ändrade leveranserna. Den här listan visar deras kanal, status, ägare, datum för skapande och ändring."

På Campaigns startsida kan ni snabbt och enkelt bläddra bland viktiga resurser, indikatorer och komponenter.

I den övre delen av startsidan finns information om de senaste uppdateringarna och nya funktioner som är tillgängliga i produkten, med länkar till versionsinformation och detaljerad dokumentation. Använd vänsterpilen för att rulla funktionskort.

![](assets/home.png){zoomable=&quot;yes&quot;}

The **Viktiga resultatindikatorer** gör att du kan kontrollera plattformens effektivitet med hjälp av gemensamma nyckeltal. Läs mer om dessa KPI:er i [den här sidan](../reporting/kpis.md).

The **Senaste** listan innehåller genvägar till de nyligen skapade och ändrade leveranserna. Den här listan visar deras kanal, status, ägare, datum för skapande och ändring. Klicka på **Visa mer** för att ladda fler leveranser.

Dessutom kan du få åtkomst till hjälpsidorna för Adobe Campaign Web key via **Utbildning** på sidan.

## Navigeringsmeny till vänster {#user-interface-left-nav}

Bläddra bland länkarna till vänster för att få tillgång till Adobe Campaign webbfunktioner. Flera länkar visar listor med objekt som kan sorteras och filtreras. Du kan också konfigurera kolumner så att all information som du behöver visas. Se det här [section](#list-screens). Vissa listskärmar är skrivskyddade. Vilka alternativ som visas på den vänstra navigeringsmenyn och i listorna beror på dina användarbehörigheter. Läs mer om behörigheter i [det här avsnittet](permissions.md).


### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="The **Explorer** På -menyn visas alla Campaign-komponenter och -objekt med samma mapphierarki som på klientkonsolen. Bläddra bland alla komponenter, mappar och scheman i Campaign v8, kontrollera tillhörande behörigheter och skapa mappar och undermappar på den här menyn."

The **Explorer** I visas alla Campaign-resurser och -objekt med samma mapphierarki som i klientkonsolen. Bläddra bland alla komponenter, mappar och scheman i Campaign v8 och skapa leveranser, arbetsflöden och kampanjer.

Objekten som visas i **Explorer** beroende på dina användarbehörigheter. Du kan också lägga till mappar och undermappar om du har rätt behörighet. Läs mer om behörigheter i [det här avsnittet](permissions.md).

Du kan konfigurera kolumner för att anpassa visningen så att all information du behöver visas. Se det här [section](#list-screens). Du kan också lägga till mappar och undermappar, enligt informationen i [det här avsnittet](permissions.md#folders).

Mer information om Campaign Explorer, mapphierarkin och resurser finns i [Kampanjdokumentation v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}.

### Campaign Management {#user-interface-campaign-management}

I CAMPAIGN MANAGEMENT-delen får ni tillgång till marknadsföringskampanjer, leveranser och arbetsflöden.

* **Kampanjer** - Det här är listan över era kampanjer och kampanjmallar. Som standard kan du för varje kampanj visa datum för start/slut/skapande/senaste ändring, aktuell status och namnet på den kampanjoperator som skapade den. Du kan filtrera listan efter status, start-/slutdatum, mapp eller skapa ett avancerat filter för att definiera egna filtervillkor. Läs mer om kampanjer [i det här avsnittet](../campaigns/gs-campaigns.md).

* **Leveranser** - Bläddra i listan över leveranser. Som standard kan du visa deras status, senaste ändringsdatum och nyckeltal för nyckeltal. Du kan filtrera listan efter status, kontaktdatum eller kanal. Klicka på en e-postleverans för att öppna instrumentpanelen och få en översikt över leveransinformationen. Leveranser i andra kanaler är skrivskyddade. Läs mer om leveranser [i det här avsnittet](../msg/gs-messages.md).

  Använd **Fler åtgärder** för att ta bort eller duplicera en leverans.

  ![](assets/more-actions.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

* **Arbetsflöden** - På den här skärmen har du tillgång till den fullständiga listan över arbetsflöden och arbetsflödesmallar. Du kan kontrollera deras status, senaste/nästa körningsdatum och skapa ett nytt arbetsflöde eller en ny arbetsflödesmall. Du kan filtrera listan med samma villkor som för andra objekt. Dessutom kan du filtrera arbetsflöden som tillhör en kampanj eller inte. Läs mer om arbetsflöden [i det här avsnittet](../workflows/gs-workflows.md).


### Innehållshantering {#user-interface-content-management}

I avsnittet CONTENT MANAGEMENT kan du visa dina innehållsmallar och fragment.

* **Innehållsmallar** - För en snabbare och förbättrad designprocess kan du skapa fristående mallar för att enkelt återanvända anpassat innehåll i [!DNL Adobe Campaign]. Den här funktionen är endast tillgänglig för e-post och gör att innehållsorienterade användare kan arbeta med fristående mallar så att marknadsföringsanvändare kan återanvända och anpassa dem i sina egna e-postkampanjer. Läs mer i [det här avsnittet](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Kundhantering {#user-interface-customer-management}

I avsnittet KUNDHANTERING kan du visa dina profiler, målgrupper och prenumerationer. De här listorna är skrivskyddade.

* **Profiler** - Skapa och hantera profiler och få tillgång till mottagardatabasen. Som standard kan du visa deras e-postadress, förnamn och efternamn. Läs mer om profiler i [det här avsnittet](../audience/about-recipients.md).
* **Målgrupper** - Det här är er lista över målgrupper. Som standard kan du visa deras typ, ursprung, datum och etikett för senaste ändring. Du kan filtrera listan efter ursprung. Läs mer om målgrupper och listor i [det här avsnittet](../audience/about-recipients.md).
* **Prenumerationstjänster** - Bläddra igenom prenumerationslistorna. Som standard kan du visa deras typ, läge och etikett. Lär dig hur du hanterar prenumerationer och avbeställningar i [Adobe Campaign v8-dokumentation (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}.
* **Fördefinierade filter** - Fördefinierade filter är anpassade filter som skapas och sparas för framtida bruk. De kan användas som genvägar under alla filtreringsåtgärder med frågemodelleraren, t.ex. när en lista med data filtreras eller när målgruppen för en leverans skapas. Läs mer i [det här avsnittet](predefined-filters.md).


### Beslutshantering {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Erbjudanden"
>abstract="Bläddra igenom listorna med erbjudanden och erbjudandemallar som har skapats i konsolen med **Interaktion** -modul. De här listorna är skrivskyddade."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html" text="Lägg till erbjudanden till en leverans"

I avsnittet BESLUTSHANTERING kan du visa erbjudandemallar. De här listorna är skrivskyddade.

* **Erbjudanden** - Bläddra igenom listan över erbjudanden och erbjudandemallar som har skapats i konsolen med **Interaktion** -modul. Som standard kan du visa deras status, start-/slutdatum och miljö. Du kan filtrera listan efter status och start-/slutdatum. Det finns även mallar för erbjudandet.

Lär dig hur du skapar och skickar erbjudanden i e-postmeddelanden och SMS i [det här avsnittet](../msg/offers.md).

### Rapportering {#left-nav-reporting}

* **Rapporter** - **Rapport** ger en samlad sammanfattning av trafik- och interaktionsstatistik för varje kanal i Campaign-miljön. Rapporterna består av olika widgetar, som var och en har ett distinkt perspektiv på kampanjen eller leveransresultatet. Läs mer i [det här avsnittet](../reporting/global-reports.md).

<!--
## Contextual Help {#user-interface-help} 

A contextual help is available in the interface. When available, click on the `?` icon to display help information and related documentation links. 

![](assets/do-not-localize/context-help.png){zoomable="yes"}{width="40%" align="left"}

Currently released as a Beta version within the new Campaign Web user interface, the **AI-powered Knowledge Assistant** embedded within contextual help revolutionizes documentation searching and answering how-to questions with effortlessly sifting through vast documentation repositories, instantly pinpointing the precise information you need.

Thanks to Campaign Gen AI's capabilities, this assistant transforms your experience, making information retrieval and problem-solving a breeze. Whether you're seeking guidance in a complex task or navigating extensive documents, our AI-powered Knowledge Assistant is your ultimate companion, providing unmatched efficiency and accuracy in every interaction.

Learn more in [this section](using-ai.md).

-->

## Läs mer {#learn-more}

Lär dig hur du bläddrar bland, söker efter och filtrerar listor som finns i Campaign-miljön [på den här sidan](list-filters.md).



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Behörighet krävs"
>abstract="Administratören måste ge dig behörighet innan du kan skapa ett segment."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Behörighet krävs"
>abstract="Administratören måste ge dig behörighet innan du kan skapa ett segment."

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Globala rapporter skickar"
>abstract="Mätvärden för spårningsrapportering visas på den här skärmen"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Spårning av globala rapporter"
>abstract="Mätvärden för spårningsrapportering visas på den här skärmen"


<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->


<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Översikt över mottagarkort"
>abstract="Översikt över mottagarkort"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Mottagarens kontaktytor"
>abstract="Mottagarens kontaktytor"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Val av mottagarprenumerationer"
>abstract="Val av mottagarprenumerationer"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Mottagarna erbjuder en lista över berättigade"
>abstract="Mottagarna erbjuder en lista över berättigade"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Mottagarna erbjuder förhandsgranskning"
>abstract="Mottagarna erbjuder förhandsgranskning"





>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Filtret Spara villkorligt innehåll"
>abstract="Filtret Spara villkorligt innehåll"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Filter för val av villkorligt innehåll"
>abstract="Filter för val av villkorligt innehåll"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Villkorligt innehåll på ämnesraden"
>abstract="Villkorligt innehåll på ämnesraden"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Villkorligt villkor för subjektiv"
>abstract="Villkorligt villkor för subjektiv"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Simulera testprofiler"
>abstract="Simulera testprofiler"

<!--ML: not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Simulera valet av testprofiler"
>abstract="Simulera valet av testprofiler"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Simulera testprofiler som skickar"
>abstract="Simulera testprofiler som skickar"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="Simulera e-postlogg"
>abstract="Simulera e-postlogg"

<!-- ML: beta wiki page - not visible in UI-->

<!-- FOR POST-GA -->

<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="Uppdatera data"
>abstract="The **Uppdatera data** aktiviteten utför en massuppdatering av fälten i databasen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="Välj hur data ska uppdateras"
>abstract="The **Åtgärdstyp** kan du välja vilken process som ska utföras på data i databasen. Välj det första alternativet för att lägga till data eller uppdatera (om det redan har lagts till). Du kan också bara lägga till data, bara uppdatera data eller ta bort data. Välj **Uppdatera och sammanfoga samlingar** för att markera en primär post att länka dubbletter till och ta bort dessa dubbletter på ett säkert sätt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="Registrerings-ID"
>abstract="Ange hur posterna i databasen ska identifieras: Om data relaterar till en befintlig måldimension väljer du **Använda målgruppsdimensionen** och välj den måldimension och de fält som ska uppdateras. I annat fall anger du en eller flera anpassade länkar för att identifiera data i databasen eller direkt användning av avstämningsnycklar."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="Välj fält som ska uppdateras"
>abstract="Markera fälten som ska uppdateras och avstämningsinställningarna. Du kan använda **Automatisk mappning** för att automatiskt identifiera de fält som ska uppdateras."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="Avancerade alternativ för att uppdatera data"
>abstract="The **Avancerade alternativ** kan du ange ytterligare inställningar för att hantera data och dubbletter."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="Generera en utgående övergång"
>abstract="Växla **Generera en utgående övergång** möjlighet att lägga till en utgående övergång som aktiveras när körningen av **Uppdatera data** aktivitet. Uppdateringen markerar vanligtvis slutet av ett målarbetsflöde och därför är alternativet inte aktiverat som standard."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="Generera en utgående övergång för avvisade."
>abstract="Växla **Generera en utgående övergång för projekt** alternativ för att lägga till en utgående övergång som innehåller poster som inte har bearbetats korrekt efter uppdateringen (till exempel om det finns en dubblett). Uppdateringen markerar vanligtvis slutet av ett målarbetsflöde och därför är alternativet inte aktiverat som standard."

<!-- Workflow settings -->

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initscript"
>title="Initieringsskript"
>abstract="Initieringsskript"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_properties"
>title="Körningsegenskaper"
>abstract="Körningsegenskaper"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_error"
>title="Körningsfel"
>abstract="Körningsfel"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_initscript"
>title="Körningsinitieringsskript"
>abstract="Körningsinitieringsskript"

<!-- Delivery alerting -->

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Kontrollpanel för leveransaviseringskriterier"
>abstract="Kontrollpanel för leveransaviseringskriterier"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Kontrollpanel för leveransvarningar"
>abstract="Kontrollpanel för leveransvarningar"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Skapa leveransaviseringskriterier"
>abstract="Skapa leveransaviseringskriterier"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indikatorer att lägga till i aviseringar"
>abstract="Indikatorer att lägga till i aviseringar"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Aviseringstyp"
>abstract="Aviseringstyp"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Villkorsfrekvens"
>abstract="Villkorsfrekvens"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Villkor för leveransvarning"
>abstract="Villkor för leveransvarning"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Allmänna parametrar för leveransvarningar"
>abstract="Leveransvarningar"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Standardstartsida"
>abstract="Välj den standardstartsida som är kopplad till den här prenumerationstjänsten."
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Parametrar för leveransvarningsvillkor"
>abstract="Leveransvarningar"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Leveransmeddelanden har skickats"
>abstract="Leveransmeddelanden har skickats"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Historik för leveransaviseringar"
>abstract="Historik för leveransaviseringar"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_create"
>title="Skapa kontrollpanel för leveransvarningar"
>abstract="Skapa kontrollpanel för leveransvarningar"

<!-- IDs -->


>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields"
>title="Redigera anpassade attribut"
>abstract="Redigera anpassade attribut"
