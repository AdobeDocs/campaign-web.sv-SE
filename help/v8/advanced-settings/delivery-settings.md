---
audience: end-user
title: Inställningar för e-postleverans
description: Webbdokumentation för Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: ed814fbb9d3f9daeb725f44a7a1929217d1d48d2
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 11%

---

# Inställningar för e-postleverans {#email-del-settings}

![](../assets/do-not-localize/badge.png)

Dessa inställningar **tekniska leveransparametrar** som definieras i e-postmallen.

## Inställningar för e-postleverans {#email-delivery-settings}

>[!CAUTION]
>
> Dessa inställningar beskrivs endast i informationssyfte. Vissa av dem beror på din konfiguration och dina behörigheter. De får inte ändras i den här versionen av produkten.

## Typologi {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologi"
>abstract="Med typologi kan du styra, filtrera och övervaka leveransen."

Typologier är uppsättningar av **typologiregler** som körs under fasen för analys av meddelande. Med dem kan du se till att dina e-postmeddelanden alltid innehåller vissa element (t.ex. en länk för att avbryta prenumerationen eller en ämnesrad) eller filtreringsregler som utesluter grupper från det avsedda målet (t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder).

När du associerar en typologi med en meddelande- eller meddelandemall körs de typologiregler som ingår i typologin för att kontrollera meddelandets giltighet under meddelandeförberedelsen.

![](assets/delivery-settings-1.png)


### Tryckparametrar {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Leveransvikt"
>abstract="Med leveransvikter kan ni identifiera leveranser med högsta prioritet inom ramen för tryckhantering. Meddelanden med högst vikt har prioritet."

I det här avsnittet kan du definiera en **tröskelvärde**. Det här är det maximala antalet meddelanden som kan skickas till en profil under en viss period. När denna tröskel har uppnåtts kan inga fler leveranser göras förrän efter den beaktade perioden. Med den här processen kan du automatiskt utesluta en profil från en leverans om ett meddelande överskrider det angivna tröskelvärdet och på så sätt undvika för många begäranden.

Tröskelvärden kan vara antingen konstanta eller variabla. Detta innebär att tröskelvärdena för en viss period kan variera från en profil till en annan eller till och med för samma profil.

I **Breddtyp** finns det tre alternativ:

* **Konstant**
* **Beroende på mottagaren**
* **Definieras i varje regel**

Använd **Leveransvikt** fält för att definiera leveransprioriteten. Varje leverans har en vikt som motsvarar dess prioritetsnivå. Som standard är vikten för en leverans inställd på 5. Med tryckregler kan du definiera vikten för de leveranser som de ska tillämpas på. Vikter kan antingen anges eller beräknas med en formel som passar mottagarna. Du kan till exempel definiera vikten för en leverans baserat på mottagarens intressen.


Använd **Leveransläge** för att välja målutvärderingsläge. Tre olika lägen finns tillgängliga:

* **Målberäkning och meddelandepersonalisering**
* **Uppskattning och godkännande av det preliminära målet**
* **Målutvärdering**

Trötthetshanteringen följer med **Kampanjoptimering** tillägg. Läs mer om tryckregler och hur du konfigurerar trötthetshantering i [Kampanjdokumentation v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}.

### Kapacitetsinställningar {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Mottagarens betydelse"
>abstract="Mottagarens betydelse är en formel som används för att avgöra vilka mottagare som behålls när reglerna för kapacitetstypologi överskrids."

I det här avsnittet kan du välja en kapacitetsregel som definieras i Adobe Campaign v8-konsolen. Den här regeln är kopplad till e-postkanalen.

The **mottagarens vikt** fält är en formel som används för att bestämma vilka mottagare som ska behållas när reglerna för kapacitetstypologi överskrids.

Läs mer om konsekvens och kapacitetsregler och hur du konfigurerar dem i [Kampanjdokumentation v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Målgrupp {#audience}

I det här avsnittet kan du välja en **målmappning** bland de tillgängliga. Målmappningar definieras i Adobe Campaign v8-konsolen.

Läs mer om målmappningar i [Kampanjdokumentation v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Leverans {#delivery}

Leveransparametrar är tekniska inställningar som gäller för leveransen.

* **Routning**: det integrerade externa kontot för e-postroutning anges som standard. Den innehåller de tekniska parametrar som gör att programmet kan skicka e-post.

* **Testa SMTP-leverans**: det här alternativet används för att testa att skicka via SMTP. Leveransen behandlas upp till anslutningen till SMTP-servern men skickas inte: för varje mottagare av leveransen ansluter Campaign till SMTP-providerservern, kör SMTP RCPT TO-kommandot och stänger anslutningen före SMTP DATA-kommandot.

* **BCC för e-post**: Det här alternativet används för att lagra e-post på ett externt system via BCC genom att lägga till en e-postadress för hemlig kopia till meddelandemålet. Läs mer om e-postkopia i [Kampanjdokumentation v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### Återförsök {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximalt antal återförsök"
>abstract="Om ett meddelande misslyckas på grund av ett tillfälligt fel, kommer nya försök att utföras under leveransens varaktighet."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Läs mer om hantering av nya försök i [Kampanjdokumentation v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Godkännande {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Godkännandeläge"
>abstract="Varje steg i en leverans kan godkännas för att säkerställa full övervakning och kontroll av de olika processerna."

Om varningar genereras under leveransförberedelsen kan du konfigurera leveransen för att definiera om den fortfarande ska köras eller inte. Som standard måste användaren bekräfta att meddelanden skickas i slutet av analysfasen: det här är **manuell** validering.

Du kan välja ett annat godkännandeläge i lämpligt fält. Tillgängliga lägen är:

* **Manuell**: I slutet av analysfasen måste användaren bekräfta leveransen för att kunna börja skicka.

* **Halvautomatisk**: Skicka börjar automatiskt om analysfasen inte genererar några varningsmeddelanden.

* **Automatisk**: Sändningen börjar automatiskt i slutet av analysfasen, oavsett resultatet.


## Giltighet {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Leveransens varaktighet"
>abstract="I fältet Leveransvaraktighet kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Giltighetsgräns för resurser"
>abstract="Fältet Giltighetsgräns används för överförda resurser, huvudsakligen för spegelsidan och bilder. Resurserna på den här sidan är giltiga under en begränsad tid."


The **Leveransens varaktighet** kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås.

Du kan också välja att ange datum. Välj **Ange giltighetsdatum explicit**. I det här fallet kan du även ange datum för leveransdatum och giltighetsgräns. Den aktuella tiden används som standard, men du kan ändra den direkt i indatafältet.

**Resurser - Giltighetsgräns** används för överförda resurser, huvudsakligen för spegelsidan och bilder. Resurserna på den här sidan är giltiga under en begränsad tid (för att spara diskutrymme).

![](assets/delivery-settings-2.png)


Läs mer om giltighetsperioden för leverans i [Kampanjdokumentation v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Hantering av spegelsidor {#mirror}

Spegelsidan är en HTML-sida som är tillgänglig online via en webbläsare. Innehållet är identiskt med e-postmeddelandet. Spegelsidan genereras som standard om länken infogas i postens innehåll.

Förutom standardläget är följande alternativ också tillgängliga:

* **[!UICONTROL Force the generation of the mirror page]**: även om ingen länk till spegelsidan infogas i leveransen, skapas spegelsidan.
* **[!UICONTROL Do not generate the mirror page]**: ingen spegelsida genereras, även om länken finns i leveransen.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: Med det här alternativet kan du komma åt spegelsidans innehåll, med anpassningsinformation, i leveransloggfönstret. Det gör du genom att klicka på **[!UICONTROL Delivery]** och väljer den rad för mottagaren vars spegelsida du vill visa. Klicka på länken **[!UICONTROL Display the mirror page for this message...]**.


### Spåra {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Giltighetsperiod"
>abstract="Det här alternativet anger hur länge spårningen ska aktiveras på URL-adresserna."

Spårningsparametrar definieras i det relaterade avsnittet. Möjliga alternativ är:

**Giltighetsgräns för spårning**: Använd det här alternativet om du vill ändra hur länge spårningen ska aktiveras på URL-adresserna.

**Ersättnings-URL för utgångna URL:er**: Använd det här alternativet om du vill ange en URL till en reservwebbsida: den visas när spårningen har upphört att gälla.

## Testinställningar {#test-setttings}

Du kan ange undantagsparametrar i det här avsnittet. Tillgängliga alternativ är:

* **Håll ihop** Med kan du auktorisera flera leveranser till mottagare som uppfyller flera målinriktningskriterier.

* **Behåll blocklist adresser** Med kan du hålla profiler som inte längre används av leveransen, t.ex. efter en avanmälan (avanmälan), kvar från målet.

* **Behåll adresser i karantän** gör att du kan hålla profiler med en adress som inte svarar från målet.

Du kan också anpassa namnet på korrekturet.

Använd **Behåll leveranskoden för korrekturet** associera till beviset med samma leveranskod som den som är definierad för den leverans som det hör till.

Som standard anges korrekturens ämne med&quot;PROOF #&quot;, där # är bevisets nummer. Du kan ändra det här prefixet i **Etikettprefix** fält.