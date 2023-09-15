---
audience: end-user
title: Inställningar för e-postleverans
description: Läs mer om inställningar för e-postleverans i webbgränssnittet för Campaign
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Beta"
source-git-commit: 2afec0260566c2393c96063037adbf1902497289
workflow-type: tm+mt
source-wordcount: '1806'
ht-degree: 7%

---


# Inställningar för e-postleverans {#email-del-settings}

Dessa inställningar **tekniska leveransparametrar** som definieras i e-postmallen. De finns på **Konfigurera leveransinställningar** -ikoner som är tillgängliga när du redigerar e-postleveranser.

## Inställningar för e-postleverans {#email-delivery-settings}

>[!CAUTION]
>
> Dessa inställningar beskrivs endast i informationssyfte. Vissa av dem beror på din konfiguration och dina behörigheter. De får inte ändras i den här versionen av produkten.

## Typologiinställningar {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologi"
>abstract="Typologiregler gör att marknadsförare kan standardisera affärspraxis för alla leveranser. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Profiler som matchar kriterier inom en typologiregel tas inte med i leveransgrupperna under beredningsfasen."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Typologiinställningar för leverans"
>abstract="Typologiregler gör att marknadsförare kan standardisera affärspraxis för alla leveranser. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Profiler som matchar kriterier inom en typologiregel tas inte med i leveransgrupperna under beredningsfasen."


Typologier är uppsättningar av **typologiregler**, som utförs under beredningsfasen. Typologiregler gör att marknadsförare kan standardisera affärspraxis för alla leveranser. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Profiler som matchar kriterier inom en typologiregel exkluderas från leveransmålgrupperna vid leveransförberedelsefasen.  Med dem kan du se till att dina e-postmeddelanden alltid innehåller vissa element (t.ex. en länk för att avbryta prenumerationen eller en ämnesrad) eller filtreringsregler som utesluter grupper från det avsedda målet (t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder).

Typologiregler grupperas tillsammans inom en typologi för att enkelt kunna tillämpa flera filterregler på en leverans samtidigt.

När du associerar en typologi med en meddelande- eller meddelandemall körs de typologiregler som ingår i typologin för att kontrollera meddelandets giltighet under meddelandeförberedelsen.

![](assets/delivery-settings-1.png)




### Trycket {#pressure-parameters}


>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Tryckparametrar för leveransen"
>abstract="Med leveransvikter kan ni identifiera leveranser med högsta prioritet inom ramen för trötthetshantering. Meddelanden med högst vikt har prioritet."


I det här avsnittet kan du definiera en **tröskelvärde** fastställa regler för trötthetshantering. Det här är det maximala antalet meddelanden som kan skickas till en profil under en viss period. När denna tröskel har uppnåtts kan inga fler leveranser göras förrän efter den beaktade perioden. Med den här processen kan du automatiskt utesluta en profil från en leverans om ett meddelande överskrider det angivna tröskelvärdet och på så sätt undvika för många begäranden.

Tröskelvärden kan vara antingen konstanta eller variabla. Detta innebär att tröskelvärdena för en viss period kan variera från en profil till en annan eller till och med för samma profil.

I **Breddtyp** finns det tre alternativ:

* **Konstant**
* **Beroende på mottagaren**
* **Definieras i varje regel**

Använd **Leveransvikt** fält för att definiera leveransprioriteten. Varje leverans har en vikt som motsvarar dess prioritetsnivå. Som standard är vikten för en leverans inställd på 5. Med tryckregler kan du definiera vikten för de leveranser som de tillämpas på. Vikter kan antingen anges eller beräknas med en formel som passar mottagarna. Du kan till exempel definiera vikten för en leverans baserat på mottagarens intressen.


Använd **Leveransläge** för att välja målutvärderingsläge. Tre olika lägen finns tillgängliga:

* **Målberäkning och meddelandepersonalisering**
* **Uppskattning och godkännande av det preliminära målet**
* **Målutvärdering**

Trötthetshanteringen följer med **Kampanjoptimering** tillägg. Läs mer om tryckregler och hur du konfigurerar trötthetshantering i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}.

### Kapacitetsinställningar {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Kapacitetsinställningar för leverans"
>abstract="Innan du skickar meddelanden ska du använda kapacitetsregler för att se till att din organisation kan behandla leveransen, de inkommande meddelanden som leveransen kan generera och antalet samtal som till exempel ska göras till kontaktprenumeranter. Kapacitetsregler definieras i Adobe Campaign v8 Console. På den här skärmen väljer du en regel som är kopplad till e-postkanalen."

I det här avsnittet kan du välja en kapacitetsregel som definieras i Adobe Campaign v8-konsolen. Den här regeln är associerad med e-postkanalen.

The **mottagarens vikt** fält är en formel som används för att bestämma vilka mottagare som ska behållas när reglerna för kapacitetstypologi överskrids.

Läs mer om konsekvens och kapacitetsregler och hur du konfigurerar dem i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Målgruppsinställningar {#audience}


>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Målgruppsinställningar för leveransen"
>abstract="Välj en **målmappning** bland de tillgängliga. Målmappningar definieras i Adobe Campaign v8-konsolen. Du kan också ange undantagsparametrar för leveransen. "


I det här avsnittet kan du välja en **målmappning** bland de tillgängliga. Målmappningar definieras i Adobe Campaign v8-konsolen.

Läs mer om målmappningar i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Leverans {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Leveransinställningar för leveransen"
>abstract="Leveransparametrar är tekniska inställningar som gäller för leveransen. Du kan aktivera BCC för leveransen och ändra leveranssätt och rutinlägen. Dessa alternativ är begränsade till expertanvändare."

Leveransparametrar är tekniska inställningar som gäller för leveransen.

* **Routning**: det integrerade externa kontot för e-postroutning anges som standard. Den innehåller de tekniska parametrar som gör att programmet kan skicka e-post.

* **Testa SMTP-leverans**: det här alternativet används för att testa att skicka via SMTP. Leveransen behandlas upp till anslutning till SMTP-servern men skickas inte: För varje mottagare av leveransen ansluter Campaign till SMTP-providerservern, kör SMTP RCPT TO-kommandot och stänger anslutningen före SMTP DATA-kommandot.

* **BCC för e-post**: det här alternativet används för att lagra e-post på ett externt system via BCC genom att lägga till en e-postadress för hemlig kopia till meddelandemålet. Läs mer om e-postkopia i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

### Webbanalys {#web-analytics}


>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Inställningar för webbanalys för leverans"
>abstract="Välj ett webbanalyskonto. Det här kontot är konfigurerat i Campaign-klientkonsolen. Du kan också definiera de taggar som delas med analysverktyget som du använder."

I det här avsnittet kan du välja ett webbanalyskonto. Det här kontot är konfigurerat i Campaign-klientkonsolen.

Du kan också definiera de taggar som delas med analysverktyget som du använder.

Läs mer om Web Analytics och Campaign i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.


### Återförsök {#retries}

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Läs mer om hantering av nya försök i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Godkännande {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Godkännandeläge för leverans"
>abstract="Välj godkännandeläge. Om varningar genereras under leveransförberedelsen kan du konfigurera leveransen för att definiera om den fortfarande ska köras eller inte. "

Om varningar genereras under leveransförberedelsen kan du konfigurera leveransen för att definiera om den fortfarande ska köras eller inte. Som standard måste användaren bekräfta att meddelanden skickas i slutet av analysfasen: det här är **manuell** validering.

Du kan välja ett annat godkännandeläge i lämpligt fält. Tillgängliga lägen är:

* **Manuell**: I slutet av analysfasen måste användaren bekräfta leveransen för att kunna börja skicka.

* **Halvautomatisk**: Sändningen börjar automatiskt om analysfasen inte genererar några varningsmeddelanden.

* **Automatisk**: Sändningen börjar automatiskt i slutet av analysfasen, oavsett resultatet.


## Giltighet {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Inställningsgiltighet"
>abstract="I fältet Leveransvaraktighet kan du ange gränsen för globala leveransförsök. Det innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, utförs regelbundna, konfigurerbara försök tills giltighetsgränsen har nåtts. Fältet Giltighetsgräns används för överförda resurser, t.ex. spegelsidan eller bilder. Resurserna är giltiga under en begränsad tid: när gränsen har nåtts är resurserna inte längre tillgängliga."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

The **Leveransens varaktighet** kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås.

Du kan också välja att ange datum. Gör detta genom att välja **Ange giltighetsdatum explicit**. I det här fallet kan du även ange datum för leveransdatum och giltighetsgräns. Den aktuella tiden används som standard, men du kan ändra den direkt i indatafältet.

**Resurser - Giltighetsgräns** används för överförda resurser, huvudsakligen för spegelsidan och bilder. Resurserna på den här sidan är giltiga under en begränsad tid (för att spara diskutrymme). Efter den här gränsen är resurserna inte längre tillgängliga.

![](assets/delivery-settings-2.png)


Läs mer om giltighetsperioden för leverans i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Hantering av spegelsidor {#mirror}

Spegelsidan är en HTML-sida som är tillgänglig online via en webbläsare. Innehållet är identiskt med e-postmeddelandet. Spegelsidan genereras som standard om länken infogas i postens innehåll.

Förutom standardläget är följande alternativ också tillgängliga:


* **[!UICONTROL Force the generation of the mirror page]**: använd det här läget för att generera spegelsidan även om ingen länk till spegelsidan infogas i leveransen.
* **[!UICONTROL Do not generate the mirror page]**: använd det här läget för att undvika att en spegelsida genereras, även om länken finns i leveransen.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: När spegelsidans länk inte finns i e-postinnehållet använder du det här alternativet för att aktivera åtkomst till spegelsidans innehåll från klientkonsolen i leveransloggfönstret.


### Spåra {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

Spårningsparametrar definieras i det relaterade avsnittet. Möjliga alternativ är:

**Giltighetsgräns för spårning**: använd det här alternativet om du vill ändra hur länge spårningen ska aktiveras på URL-adresserna.

**Ersättnings-URL för utgångna URL:er**: använd det här alternativet om du vill ange en URL till en reservwebbsida: den visas när spårningen har upphört att gälla.

## Testinställningar {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Testinställningar för leverans"
>abstract="Välj undantagsparametrar och anpassa etiketten för testmeddelandena."

Du kan ange undantagsparametrar i det här avsnittet. Tillgängliga alternativ är:

* **Behåll dubbla** Med kan du auktorisera flera leveranser till mottagare som uppfyller flera målinriktningskriterier.

* **Behåll blocklist adresser** Med kan du hålla profiler som inte längre används av leveransen, t.ex. efter en avanmälan (avanmälan), kvar från målet.

* **Behåll adresser i karantän** gör att du kan hålla profiler med en adress som inte svarar från målet.

Du kan också anpassa namnet på testmeddelandena.

Använd **Behåll leveranskoden för beviset** associera till testmeddelandet med samma leveranskod som den som är definierad för den leverans som det är relaterat till.

Ämnet i testmeddelandet har som standard prefixet&quot;PROOF #&quot;, där # är numret på testmeddelandet. Du kan ändra det här prefixet i **Etikettprefix** fält.