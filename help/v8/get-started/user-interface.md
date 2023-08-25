---
audience: end-user
title: Upptäck gränssnittet
description: Användargränssnittet Campaign v8 på webben
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alfa"
source-git-commit: bbe4ed0ce05048cf22a18a36967b9a4c0422d93f
workflow-type: tm+mt
source-wordcount: '2567'
ht-degree: 0%

---

# Upptäck gränssnittet {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Upptäck gränssnittet"
>abstract="Det nya webbgränssnittet Campaign v8 erbjuder en integrerad, intuitiv och enhetlig användarupplevelse."

Det nya webbgränssnittet Campaign v8 erbjuder en modern och intuitiv användarupplevelse som förenklar utformningen och leveransen av marknadsföringskampanjer. Det nya gränssnittet är integrerat med Adobe Experience Platform.


>[!NOTE]
>
>Den här dokumentationen uppdateras ofta för att återspegla de senaste ändringarna i produktanvändargränssnittet. Vissa skärmbilder kan dock skilja sig något från användargränssnittet.


## Navigeringsmeny till vänster {#user-interface-left-nav}

Bläddra bland länkarna till vänster för att få tillgång till webbfunktionerna i Campaign v8. Flera länkar visar listor med objekt som kan sorteras och filtreras. Du kan också konfigurera kolumner så att all information som du behöver visas. Se det här [section](#list-screens). Alla listskärmar är skrivskyddade, förutom leveranslistan för e-post. Det går inte att klicka på ett listobjekt för utgåva/visning i Alpha. Alla listor kan redigeras i framtida versioner. Vilka alternativ som visas på den vänstra navigeringsmenyn beror på dina användarbehörigheter.

![](assets/home.png)

### Startsida {#user-interface-home}

Skärmen innehåller länkar och resurser som gör att du snabbt kommer åt de viktigaste webbfunktionerna i Campaign v8.

The **Senaste** listan innehåller genvägar till de nyligen skapade och ändrade leveranserna. Den här listan visar deras kanal, status, ägare, datum för skapande och ändring.

The **Viktiga resultatindikatorer** gör att du kan kontrollera plattformens effektivitet med hjälp av gemensamma nyckeltal.

Få åtkomst till hjälpsidorna för webbnyckel v8 från **Utbildning** på startsidan.


### Viktiga resultatindikatorer {#user-interface-key-indicators}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="Skräppost-KPI"

Bläddra till startsidan för att kontrollera viktiga prestandaindikatorer för din plattform. Indikatorerna visar antalet meddelanden som levereras, öppnas, klickas, tas bort från prenumerationen och antalet fel.

Mätvärden beräknas som standard för leveranser som skickats under de senaste 7 dagarna. Du kan ändra perioden från listrutan i kortets övre högra del. Meddelanden som skickas till testprofiler exkluderas.

Du kan välja vilken kanal som ska visas. Som standard återspeglar dessa indikatorer mätvärden för e-postkanalen.

![](assets/kpi.png)

#### Meddelandet har levererats {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Levererat"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla meddelanden som har bearbetats och hur många meddelanden som har levererats med framgång jämfört med det totala antalet meddelanden som skickats."

Antalet meddelanden som levereras återspeglar din leveransgrad. Det kan aldrig vara 100 % av följande orsaker: vissa adresser eller telefonnummer kan vara fel, skräppostblockerare hos e-postleverantörer kan avvisa dina meddelanden eller leveransproblem kan inträffa.

The **Levererat** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet meddelanden som levererats med lyckat resultat jämfört med det totala antalet skickade meddelanden.

* Summan av alla meddelanden som har bearbetats utan fel.

I Adobe Campaign är regeln för att markera ett meddelande som&quot;Levererat&quot;:

Antal meddelanden för vilka fältet &quot;dirigeringsadress&quot; är lika med &quot;Nej&quot; och med statusen &quot;Som tagits med i beräkningen av tjänsteleverantören&quot; (för SMS) eller &quot;Skickat&quot; (för e-post) eller &quot;Mottaget på mobilen&quot; (för push-meddelanden).


#### Totalt antal öppningar {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Öppnar"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla meddelanden som öppnats och hur många meddelanden som öppnats i procent jämfört med det totala antalet meddelanden som levererats med framgång."

Totalt antal öppningar beräknas genom att spåra det totala antalet gånger ett meddelande öppnas, oavsett hur många enskilda mottagare som öppnas av. Den här indikatorn är bara tillgänglig för e-post.

The **Öppnar** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet meddelanden som öppnats jämfört med det totala antalet meddelanden som levererats med lyckat resultat.

* Summan av alla öppnade meddelanden, per kanal.

Adobe Campaign identifierar att ett meddelande öppnas när mottagaren hämtar bilderna i e-postmeddelandet. HTML och Multipart/Alternative emails innehåller en bild på 0 pixlar som gör att du kan identifiera meddelanden som har öppnats. Eftersom meddelanden i textformat inte innehåller några bilder går det inte att se om de har öppnats eller inte. Värden som beräknas baserat på det meddelande som öppnas är alltid uppskattningar på grund av den felmarginal som är länkad till bildvisningen.



#### Genomklickningsfrekvens {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Klickningar"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla URL-adresser som klickats i meddelanden och procentandelen klickningar jämfört med det totala antalet meddelanden som levererats utan fel."

Du kan lägga till URL:er i meddelandeinnehållet, som dirigerar om mottagarna till en viss sida. Klickfrekvensen mäter antalet och procentandelen mottagare som klickade på en länk i meddelandet.

The **Klickningar** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet klick jämfört med det totala antalet meddelanden som levererats med framgång.

* Antal distinkta personer som klickat minst en gång i en leverans. Länkar som inte längre används och länkar till e-postspegelsidan tas inte med.

Dessa mått baseras på den konsoliderade spårningstabellen (`nms:trackingStats`). Den här sammanställningstabellen används av prestandaskäl när rapporter visas, i stället för i loggtabellen för mottagarspårning (`nms:trackingLogRcp`) och beräknas inte i realtid. Tabellen genereras några minuter efter att spårningsloggarna har hämtats.


#### Avbryta prenumerationstaxor {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Avprenumerationer"
>abstract="I det här måttet visas, för den valda kanalen, summan av alla avbeställningar från en tjänst och procentandelen avbeställningar jämfört med det totala antalet meddelanden som levererats med framgång."

Mottagarna måste kunna avanmäla sig från e-post och SMS via en dedikerad avprenumerationslänk i e-postinnehållet eller genom att svara STOP på ett SMS.

The **Avbeställ** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet avbrutna prenumerationer jämfört med det totala antalet meddelanden som levererats utan framgång.

* Summan av alla klick på en länk för att avbryta prenumerationen, dvs. där en URL-kategori är lika med &quot;Avanmäl dig&quot;.


#### Felfrekvenser {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Fel"
>abstract="Totalt antal fel som ackumulerats under leveranser och automatisk avhoppsbearbetning. Den associerade frekvensen är förhållandet till antalet meddelanden som ska levereras."

Vissa meddelanden som skickas från din Adobe Campaign-plattform når kanske inte sina mål. Det kan hända när användaradressen eller telefonen har stavfel, om mottagaren har ändrat e-postadressen eller om postlådan är full. Om ett meddelande inte kan skickas till en profil skickar fjärrservern automatiskt ett felmeddelande till Adobe Campaign. Det här felet är kvalificerat för att avgöra om e-postadressen, telefonnumret eller enheten ska sättas i karantän.

Därför bör du alltid kontrollera och uppdatera databasen och se till att alla profiler är aktiva och riktiga. Leveransfel kan vara tillfälliga eller permanenta - mjuka eller hårda studsar - beroende på varför meddelandet inte levererades.

The **Fel** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet fel jämfört med det totala antalet meddelanden som ska levereras.

* Totalt antal fel som ackumulerats under leveranser och automatisk återinläsning.


### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="The **Explorer** På -menyn visas alla Campaign-komponenter och -objekt med samma mapphierarki som på klientkonsolen. Bläddra bland alla komponenter, mappar och scheman i Campaign v8 och skapa leveranser, arbetsflöden och kampanjer. Alla andra listor är skrivskyddade."

The **Explorer** I visas alla Campaign-resurser och -objekt med samma mapphierarki som i klientkonsolen. Bläddra bland alla komponenter, mappar och scheman i Campaign v8 och skapa leveranser, arbetsflöden och kampanjer. Alla andra listor är skrivskyddade.

Vilka objekt som visas i Utforskaren beror på dina användarbehörigheter.

Precis som i alla listskärmar kan du konfigurera kolumner så att de anpassas för visningen så att du kan se all information du behöver. Se det här [section](#list-screens).

Mer information om Campaign Explorer, mapphierarkin och resurser finns i [Kampanjdokumentation v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}.

### Campaign Management {#user-interface-campaign-management}

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Kampanjer"
>abstract="Det här är listan över era kampanjer. Du kan visa användbar information som start-/slutdatum/sista ändringsdatum samt status för dem. Du kan filtrera listan efter status eller start-/slutdatum. Klicka på knappen Skapa kampanj för att lägga till en ny kampanj. Välj en kampanj för att visa dess innehåll, leveranser och detaljer. Bläddra till fliken Mallar för att visa och skapa mallar."



I CAMPAIGN MANAGEMENT-delen får ni tillgång till marknadsföringskampanjer, leveranser och arbetsflöden.

* **Kampanjer** - Det här är listan över era kampanjer och kampanjmallar. Som standard kan du för varje kampanj visa datum för start/slut/skapande/senaste ändring, aktuell status och namnet på den kampanjoperator som skapade den. Du kan filtrera listan efter status, start-/slutdatum, mapp eller skapa ett avancerat filter för att definiera egna filtervillkor. Läs mer om kampanjer [i det här avsnittet](../campaigns/gs-campaigns.md).

* **Leveranser** - Bläddra i listan över leveranser. Som standard kan du visa deras status, senaste ändringsdatum och nyckeltal för nyckeltal. Du kan filtrera listan efter status, kontaktdatum eller kanal. Klicka på en e-postleverans för att öppna instrumentpanelen och få en översikt över leveransinformationen. Leveranser i andra kanaler är skrivskyddade. Läs mer om leveranser [i det här avsnittet](../msg/gs-messages.md).

  Använd **Fler åtgärder** för att ta bort eller duplicera en leverans.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Arbetsflöden** - På den här skärmen har du tillgång till den fullständiga listan över arbetsflöden och arbetsflödesmallar. Du kan kontrollera deras status, senaste/nästa körningsdatum och skapa ett nytt arbetsflöde eller en ny arbetsflödesmall. Du kan filtrera listan med samma villkor som för andra objekt. Dessutom kan du filtrera arbetsflöden som tillhör en kampanj eller inte. Läs mer om arbetsflöden [i det här avsnittet](../workflows/gs-workflows.md).


### Kundhantering {#user-interface-customer-management}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Mottagare"
>abstract="Få åtkomst till din mottagardatabas. Du kan visa användbar information som e-postadress, förnamn och efternamn. Den här listan är skrivskyddad."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Målgrupper"
>abstract="Det här är er lista över målgrupper. Du kan visa typ, ursprung, datum och etikett för senaste ändringsdatum och skapandedatum. Du kan filtrera listan efter ursprung. Den här listan är skrivskyddad."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Prenumerationslistor"
>abstract="Bläddra bland prenumerationslistorna. Du kan visa deras typ, läge och etikett. Den här listan är skrivskyddad."


I avsnittet KUNDHANTERING kan du visa dina mottagare, målgrupper och prenumerationer. De här listorna är skrivskyddade.

* **Mottagare** - Få åtkomst till din mottagardatabas. Som standard kan du visa deras e-postadress, förnamn och efternamn. Läs mer om mottagare i [Adobe Campaign v8-dokumentation (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/gs-audiences.html){target="_blank"}.
* **Målgrupper** - Det här är er lista över målgrupper. Som standard kan du visa deras typ, ursprung, datum och etikett för senaste ändring. Du kan filtrera listan efter ursprung. Läs mer om målgrupper och listor i [Adobe Campaign v8-dokumentation (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.
* **Prenumerationer** - Bläddra igenom prenumerationslistorna. Som standard kan du visa deras typ, läge och etikett. Lär dig hur du hanterar prenumerationer och avbeställningar i [Adobe Campaign v8-dokumentation (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}.

### Beslutshantering

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Erbjudanden"
>abstract="Bläddra igenom listan med interaktionserbjudanden. Som standard kan du visa deras status, start-/slutdatum och miljö. Du kan filtrera listan efter status och start-/slutdatum. Det finns även mallar för erbjudandet. De här listorna är skrivskyddade."

* **Erbjudanden** - Bläddra igenom listan med interaktionserbjudanden. Som standard kan du visa deras status, start-/slutdatum och miljö. Du kan filtrera listan efter status och start-/slutdatum. Det finns även mallar för erbjudandet. De här listorna är skrivskyddade.

Lär dig hur du skapar hanterade erbjudanden i [Adobe Campaign v8-dokumentation (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

## Övre fält

Använd gränssnittets övre fält för att:

* dela med dig av dina synpunkter som en alfakonstant
* växla mellan organisationer och instanser
* växla mellan olika Adobe Experience Cloud-program
* få tillgång till hjälpsidor, kontakta support och dela feedback. Du kan söka efter hjälpartiklar och videoklipp i sökfältet.

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Sammanhangsberoende hjälp {#contextual-help}

Det finns sammanhangsberoende hjälp i gränssnittet. Klicka på `?` om du vill visa hjälpinformation och relaterade dokumentationslänkar.

![](assets/context-help.png){width="40%" align="left"}

<!--An on-boarding guide is also available to help you get started with Campaign v8 Web. Click the icon in the bottom right corner, choose one of the available step-by-step scenarios, and simply follow the instructions.

![](assets/onboarding.png){width="70%" align="left"}-->

## Webbläsare som stöds {#browsers}

Campaign v8 Web är utformat för att fungera optimalt i den senaste versionen av Google Chrome, Safari och Microsoft Edge. Du kan ha problem med att använda vissa funktioner i äldre versioner eller i andra webbläsare.

## Språkinställningar {#language-pref}

Campaign v8 Web finns för närvarande på följande språk:

<table>
<tr>
<td>
<p>Engelska (USA) - EN-US</p>
<p>Franska - FR</p>
<p>Tyska - DE</p>
<p>Italienska - IT</p>
</td>
<td>
<p>Spanska - ES</p>
<p>Portugisiska (Brasilien) - PTBR</p>
<p>Japanska - JP</p>
</td>
<td>
<p>Koreanska - KR</p>
<p>Förenklad kinesiska - CHS</p>
<p>Traditionell kinesiska - CHT</p>
</td>
</tr>
</table>

Standardspråket för gränssnittet avgörs av det språk du föredrar i användarprofilen.

Så här byter du språk:

1. Klicka på din profilikon, längst upp till höger och välj sedan **Inställningar**.
1. Klicka sedan på den språklänk som visas under din e-postadress.
1. Välj önskat språk och klicka på **Spara**. Du kan välja ett andra språk om komponenten som du använder inte är lokaliserad på ditt första språk.


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
>id="acw_targetdata_personalization_enrichmentdata"
>title="Anrikningsdata"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Rapportering skickas"
>abstract="Se utskicksindikatorerna för kampanjrapporteringen."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Rapporteringsspårning"
>abstract="Se spårningsindikatorerna för kampanjrapporteringen."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Rapportöversikt"
>abstract="Viktiga mätvärden för leveransen."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Rapportera målstatistik"
>abstract="I det här avsnittet visas specifika mätvärden beroende på målgrupper."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="Aggregerad rapportering för leveranser"
>abstract="Välj minst två leveranser för att visa en sammanställd datarapport."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Dedupliceringsfält"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Inställningar för borttagning av dubbletter"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Dedupliceringskomplementet"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Komplementfärg till Dimension"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Behörighet krävs"
>abstract="Administratören måste ge dig behörighet innan du kan skapa ett segment."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Behörighet krävs"
>abstract="Administratören måste ge dig behörighet innan du kan skapa ett segment."


>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Den här kampanjen är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här kampanjen. Kontakta administratören om det behövs för att ge dig åtkomst."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="Leveransen är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här leveransen. Kontakta administratören om det behövs för att ge dig åtkomst."

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="Tjänsten är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här tjänsten. Kontakta administratören om det behövs för att ge dig åtkomst."

<!-- Workflows-->

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Arbetsflödeslista"
>abstract="Lista över tillgängliga arbetsflöden för kampanjen. Använd knappen Skapa arbetsflöde för att lägga till ett arbetsflöde i kampanjen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Avgående övergång för att spara"
>abstract="tbc"

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_activity"
>title="Spara en publik"
>abstract="Använd den här aktiviteten för att spara målgruppen i arbetsflödet."


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="Arbetsflödet är skrivskyddat"
>abstract="Du har inte behörighet att redigera det här arbetsflödet. Kontakta administratören om det behövs för att ge dig åtkomst."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Arbetsflödet är skrivskyddat"
>abstract="Du kan inte redigera det här arbetsflödet på grund av att arbetsytan inte stöds eller är inkompatibel."

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Giltighetsperiod"
>abstract="Det här alternativet anger hur länge spårningen ska aktiveras på URL-adresserna."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Leveransens varaktighet"
>abstract="I fältet Leveransvaraktighet kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Giltighetsgräns för resurser"
>abstract="Fältet Giltighetsgräns används för överförda resurser, t.ex. spegelsidan eller bilder. Resurserna är giltiga under en begränsad tid: när gränsen har nåtts är resurserna inte längre tillgängliga."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Godkännandeläge"
>abstract="Varje steg i en leverans kan godkännas för att säkerställa full övervakning och kontroll av de olika processerna."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Maximalt antal återförsök"
>abstract="Om ett meddelande misslyckas på grund av ett tillfälligt fel, utförs nya försök tills slutet av leveransens varaktighet är slut."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Mottagarens betydelse"
>abstract="Mottagarens betydelse är en formel som används för att avgöra vilka mottagare som behålls när reglerna för kapacitetstypologi överskrids."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Leveransvikt"
>abstract="Med leveransvikter kan ni identifiera leveranser med högsta prioritet inom ramen för tryckhantering. Meddelanden med högst vikt har prioritet."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Typologi"
>abstract="Med typologi kan du styra, filtrera och övervaka leveransen."

>[!CONTEXTUALHELP]
>id="acw_reporting_email_exportation"
>title="Exportera"
>abstract="Du kan bara exportera den markerade sidan."

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Leveranslista i en kampanj"
>abstract="Leveranslista i en kampanj"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Arbetsflödeslista i en kampanj"
>abstract="Arbetsflödeslista i en kampanj"

<!-- delivery settings-->

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Målgrupp för leveransinställningar"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Godkännande av leveransinställningar"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Testinställningar för leveransinställningar"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Webbanalys för leveransinställningar"
>abstract="TBC"
