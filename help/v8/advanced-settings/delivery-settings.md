---
audience: end-user
title: Leveransinställningar
description: Läs mer om leveransinställningar på Campaign Web
feature: Email
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '2295'
ht-degree: 4%

---


# Inställningar för e-postleverans {#email-del-settings}

Inställningar för e-postleverans **tekniska leveransparametrar** som definieras i e-postmallen. De kan laddas över för varje leverans.

De här inställningarna är tillgängliga i **Inställningar** som är tillgängliga när du redigerar en e-postleveransmall eller en e-postleveransmall.

## Inställningar för e-postleverans {#email-delivery-settings}

>[!CAUTION]
>
>Dessa inställningar beskrivs endast i informationssyfte. Vissa av dem beror på din konfiguration och dina behörigheter. De får inte ändras i den här versionen av produkten.

## Typologiinställningar {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologi"
>abstract="Typologiregler gör att marknadsförare kan standardisera affärspraxis för alla leveranser. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Profiler som matchar kriterier inom en typologiregel tas inte med i leveransgrupperna under beredningsfasen. Typologier och typologiregler skapas i Campaign-klientkonsolen."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Typologiinställningar för leverans"
>abstract="Typologiregler gör att marknadsförare kan standardisera affärspraxis för alla leveranser. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Profiler som matchar kriterier inom en typologiregel tas inte med i leveransgrupperna under beredningsfasen. Typologier och typologiregler skapas i Campaign-klientkonsolen."


Typologier är uppsättningar av **typologiregler** som utförs under beredningsfasen för att enkelt tillämpa flera filterregler på en leverans samtidigt. De gör att marknadsförarna kan standardisera sina rutiner för alla leveranser när de kan styra, filtrera och prioritera leveransen.

När du associerar en typologi med en meddelande- eller meddelandemall körs de typologiregler som ingår i typologin för att kontrollera leveransgiltigheten under meddelandeförberedelsen. Profiler som matchar kriterier inom en typologiregel exkluderas sedan från leveransgrupperna.

Typologier gör att du kan se till att dina e-postmeddelanden alltid innehåller vissa element (t.ex. en länk för att avbryta prenumerationen eller en ämnesrad) eller filtreringsregler för att utesluta grupper från det avsedda målet (t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder).

![](assets/delivery-settings-typology.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>Typologier och typologiregler skapas i Campaign-klientkonsolen. Läs mer om tryckregler och hur du konfigurerar trötthetshantering i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html){target="_blank"}.

### Trycket {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Tryckparametrar för leveransen"
>abstract="Med leveransvikter kan ni identifiera leveranser med högsta prioritet inom ramen för trötthetshantering. Meddelanden med högst vikt har prioritet."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Leveransvikt"
>abstract="Med leveransvikter kan ni identifiera leveranser med högsta prioritet inom ramen för tryckhantering. Meddelanden med högst vikt har prioritet."

I det här avsnittet kan du definiera en **tröskelvärde** konfigurera regler för trötthetshantering, vilket är det maximala antalet meddelanden som kan skickas till en profil under en viss period.

När denna tröskel har uppnåtts kan inga fler leveranser göras förrän efter den beaktade perioden. Med den här processen kan du automatiskt utesluta en profil från en leverans om ett meddelande överskrider det angivna tröskelvärdet och på så sätt undvika för många begäranden.

Tröskelvärden kan vara antingen konstanta eller variabla. Detta innebär att tröskelvärdena för en viss period kan variera från en profil till en annan eller till och med för samma profil.

I **[!UICONTROL Weight type]** finns det tre alternativ:

* **[!UICONTROL Constant]**
* **[!UICONTROL Depends on the recipient]**
* **[!UICONTROL Defined in each rule]**

Använd **[!UICONTROL Delivery weight]** fält för att definiera leveransprioriteten. Varje leverans har en vikt som motsvarar dess prioritetsnivå. Som standard är vikten för en leverans inställd på 5. Med tryckregler kan du definiera vikten för de leveranser som de tillämpas på. Vikter kan antingen anges eller beräknas med en formel som passar mottagarna. Du kan till exempel definiera vikten för en leverans baserat på mottagarens intressen.

Använd **[!UICONTROL Delivery mode]** för att välja målutvärderingsläge. Tre olika lägen finns tillgängliga:

* **[!UICONTROL Target estimation and message personalization]**
* **[!UICONTROL Estimation and approval of the provisional target]**
* **[!UICONTROL Target evaluation]**

>[!NOTE]
>
>Trötthetshantering har konfigurerats i Campaign-klientkonsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}.

### Kapacitetsinställningar {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Kapacitetsinställningar för leverans"
>abstract="Innan du skickar meddelanden ska du använda kapacitetsregler för att se till att din organisation kan behandla leveransen, de inkommande meddelanden som leveransen kan generera och antalet samtal som till exempel ska göras till kontaktprenumeranter. Kapacitetsregler definieras i Adobe Campaign v8-konsolen. På den här skärmen väljer du en regel som är kopplad till e-postkanalen."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Mottagarens betydelse"
>abstract="Mottagarens betydelse är en formel som används för att avgöra vilka mottagare som behålls när reglerna för kapacitetstypologi överskrids."


I det här avsnittet kan du välja en kapacitetsregel som definieras i Adobe Campaign v8-konsolen. Den här regeln är associerad med e-postkanalen.

The **[!UICONTROL Importance of the recipient]** fält är en formel som används för att bestämma vilka mottagare som ska behållas när reglerna för kapacitetstypologi överskrids.

>[!NOTE]
>
>Typologiregler konfigureras i Campaign Client-konsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.

## Målgruppsinställningar {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Målgruppsinställningar för leveransen"
>abstract="Välj en **målmappning** bland de tillgängliga. Målmappningar definieras i Adobe Campaign v8-konsolen. Du kan också ange undantagsparametrar för leveransen. "

I det här avsnittet kan du välja en **målmappning** bland de tillgängliga. Målmappningar definieras i Adobe Campaign v8-konsolen. Målmappningen är den typ av data som hanteras av en åtgärd. Det gör att du kan definiera målpopulationen: mottagare, avtalspliktiga mottagare, operatörer, prenumeranter osv.

Läs mer om målmappningar i [det här avsnittet](../audience/targeting-dimensions.md).

I **[!UICONTROL Exclusion]** kan du välja att exkludera mottagare som inte längre vill bli kontaktade eller som hamnar i karantän. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

## Leverans {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Leveransinställningar för leveransen"
>abstract="Leveransparametrar är tekniska inställningar som gäller för leveransen. Du kan ändra leverans- och rutinlägen, aktivera e-postkopia, skicka med hjälp av påfyllnader och även välja formatet för de e-postmeddelanden som skickas. Dessa alternativ är begränsade till expertanvändare."

**[!UICONTROL Delivery]** parametrar är tekniska inställningar som gäller för leveransen.

![](assets/delivery-settings-delivery.png){zoomable=&quot;yes&quot;}

Det integrerade e-postmeddelandet **[!UICONTROL Routing]** externt konto anges som standard. Den innehåller de tekniska parametrar som gör att programmet kan skicka e-post.

Du kan definiera **[!UICONTROL Sending]** inställningarna nedan.

* **[!UICONTROL Delivery priority]**: Använd det här alternativet om du vill ändra avsändarordningen för leveranser genom att ange prioritetsnivå: normal, hög eller låg.

* **[!UICONTROL Message batch quantity]**: Använd det här alternativet om du vill definiera antalet meddelanden som grupperas i samma XML-leveranspaket. Om parametern är inställd på 0 grupperas meddelandena automatiskt. Paketstorleken definieras av beräkningen `<delivery size>/1024`, med minst 8 och högst 256 meddelanden per paket.

  >[!IMPORTANT]
  >
  >När leveransen skapas genom duplicering av en befintlig, återställs den här parametern.

* **[!UICONTROL Test SMTP delivery]**: Det här alternativet används för att testa att skicka via SMTP. Leveransen behandlas upp till anslutning till SMTP-servern, men skickas inte: För varje mottagare av leveransen ansluter Campaign till SMTP-providerservern, kör SMTP RCPT TO-kommandot och stänger anslutningen före SMTP DATA-kommandot.

* **[!UICONTROL Email BCC]**: Det här alternativet används för att lagra e-post på ett externt system via BCC genom att lägga till en e-postadress för hemlig kopia till meddelandemålet. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

I **[!UICONTROL Wave definition]** väljer du **[!UICONTROL Send using multiple waves]** möjlighet att stegvis öka volymen som skickas med vågor. På så sätt undviker du att meddelanden markeras som skräppost eller när du vill begränsa antalet meddelanden per dag. Med vågor kan du dela upp leveranser i flera grupper i stället för att skicka stora mängder meddelanden samtidigt. [Läs mer](send-using-waves.md)

Du kan också ändra **[!UICONTROL Mail formats]** av de e-postmeddelanden som skickats enligt nedan.

* **[!UICONTROL Use recipient preferences]** (standardläge)

  Meddelandeformatet definieras enligt de data som lagras i mottagarprofilen. Om en mottagare vill ta emot meddelanden i ett visst format är detta det format som skickas. Om fältet inte är ifyllt skickas ett multipart-alternativt meddelande (se nedan).

* **[!UICONTROL Let recipient mail client choose the most appropriate format]**

  Meddelandet innehåller båda formaten: text och HTML. Formatet som visas vid mottagning beror på konfigurationen av mottagarens e-postprogramvara (multipart-option).

  >[!IMPORTANT]
  >
  >Det här alternativet inkluderar båda versionerna av dokumentet. Det påverkar därför leveransgraden eftersom meddelandestorleken är större.

* **[!UICONTROL Send all messages in text format]**

  Meddelandet skickas i textformat. HTML-formatet skickas inte, utan används endast för spegelsidan när mottagaren klickar på meddelandet.

## Web Analytics {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Inställningar för webbanalys för leverans"
>abstract="Välj ett webbanalyskonto. Det här kontot är konfigurerat i Campaign Client-konsolen. Du kan också definiera de taggar som delas med analysverktyget som du använder."

I det här avsnittet kan du välja ett webbanalyskonto. Det här kontot är konfigurerat i Campaign-klientkonsolen.

Du kan också definiera de taggar som delas med analysverktyget som du använder.

>[!NOTE]
>
>Web Analytics-funktioner konfigureras i Campaign Client-konsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html#external-account-ac){target="_blank"}.

## Försök igen {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Maximalt antal återförsök"
>abstract="Om ett meddelande misslyckas på grund av ett tillfälligt fel, utförs nya försök tills slutet av leveransens varaktighet är slut."

<!--Currently not visible in UI > ??-->

Meddelanden som inte har levererats tillfälligt på grund av ett mjukt eller ignorerat fel kan återförsökas automatiskt. Som standard schemaläggs fem återförsök till den första dagen i leveransen med ett minsta intervall på en timme som sprids ut över dygnets 24 timmar.

Läs mer om hantering av nya försök i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Godkännande {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Godkännandeläge för leverans"
>abstract="Välj godkännandeläge. Om varningar genereras under leveransförberedelsen kan du konfigurera leveransen för att definiera om den fortfarande ska köras eller inte."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Godkännandeläge för leveranser"
>abstract="Välj godkännandeläge för leveranser baserat på den här mallen. Om varningar genereras under leveransförberedelsen kan du konfigurera leveransen för att definiera om den fortfarande ska köras eller inte."

Om varningar genereras under leveransförberedelsen kan du konfigurera leveransen för att definiera om den fortfarande ska köras eller inte. Som standard måste användaren bekräfta att meddelanden skickas i slutet av analysfasen: det här är **manuell** validering.

Du kan välja ett annat godkännandeläge i lämpligt fält. Tillgängliga lägen är:

* ****[!UICONTROL Manual]****: I slutet av analysfasen måste användaren bekräfta leveransen för att kunna börja skicka.

* **[!UICONTROL Semi-Automatic]**: Sändningen börjar automatiskt om analysfasen inte genererar några varningsmeddelanden.

* **[!UICONTROL Automatic]**: Sändningen börjar automatiskt i slutet av analysfasen, oavsett resultatet.

## Giltighet {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Inställningsgiltighet"
>abstract="The **Leveransens varaktighet** kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås.<br>The **Giltighetsgräns för resurser** -fältet används för överförda resurser, t.ex. spegelsidor eller bilder. När gränsen har nåtts är resurserna inte längre tillgängliga."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Giltighetsgräns för resurser"
>abstract="The **Giltighetsgräns för resurser** -fältet används för överförda resurser, t.ex. spegelsidan eller bilder. Resurserna är giltiga under en begränsad tid: när gränsen har nåtts är resurserna inte längre tillgängliga."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Leveransens varaktighet"
>abstract="The **Leveransens varaktighet** kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### Giltighetsperiod {#validity-period}

The **[!UICONTROL Delivery duration]** kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås.

Du kan också välja att ange datum. Gör detta genom att välja **[!UICONTROL Explicitly set validity dates]**. I det här fallet kan du även ange datum för leveransdatum och giltighetsgräns. Den aktuella tiden används som standard, men du kan ändra den direkt i indatafältet.

**[!UICONTROL Resources validity limit]** används för överförda resurser, huvudsakligen för spegelsidan och bilder. Resurserna på den här sidan är giltiga under en begränsad tid (för att spara diskutrymme). Efter den här gränsen är resurserna inte längre tillgängliga.

![](assets/delivery-settings-validity.png){zoomable=&quot;yes&quot;}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

Läs mer om giltighetsperioden för leverans i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Hantering av spegelsidor {#mirror}

Spegelsidan är en HTML-sida som är tillgänglig online via en webbläsare. Innehållet är identiskt med e-postmeddelandet. Spegelsidan genereras som standard om länken infogas i postens innehåll.

Förutom standardläget är följande alternativ också tillgängliga:

* **[!UICONTROL Force the generation of the mirror page]**: Använd det här läget för att generera spegelsidan även om ingen länk till spegelsidan infogas i leveransen.
* **[!UICONTROL Do not generate the mirror page]**: Använd det här läget för att undvika att en spegelsida genereras, även om länken finns i leveransen.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: När spegelsidans länk inte finns i e-postinnehållet använder du det här alternativet för att aktivera åtkomst till spegelsidans innehåll från klientkonsolen i leveransloggfönstret.


### Spåra {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Giltighetsperiod"
>abstract="Giltighetsperioden anger den varaktighet som spårningen är aktiverad för i meddelande-URL:erna."

**[!UICONTROL Tracking]** parametrar definieras i det relaterade avsnittet. Möjliga alternativ är:

**[!UICONTROL Tracking validity limit]**: Använd det här alternativet om du vill ändra hur länge spårningen ska aktiveras på URL-adresserna.

**[!UICONTROL Substitution URL for expired URLs]**: Använd det här alternativet om du vill ange en URL till en reservwebbsida: den visas när spårningen har upphört att gälla.

## Korrekturinställningar {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Definiera korrekturinställningarna för leveransen"
>abstract="Välj undantagsparametrarna och anpassa etiketten för korrektur."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

Du kan ange undantagsparametrar i det här avsnittet. Tillgängliga alternativ är:

* ****[!UICONTROL Keep doubles]**** Med kan du auktorisera flera leveranser till mottagare som uppfyller flera målinriktningskriterier.

* **[!UICONTROL Keep denylisted addresses]** Med kan du hålla profiler som inte längre används av leveransen, t.ex. efter en avanmälan (avanmälan), kvar från målet.

* **[!UICONTROL Keep quarantined addresses]** gör att du kan hålla profiler med en adress som inte svarar från målet.

Du kan också anpassa etiketten för korrektur:

* Använd **[!UICONTROL Keep the delivery code for the proof]** associera till beviset med samma leveranskod som den som är definierad för den leverans som det hör till.

* Som standard anges korrekturens ämne med &quot;PROOF #&quot;, där # är korrekturets nummer. Du kan ändra det här prefixet i **[!UICONTROL Label prefix]** fält.