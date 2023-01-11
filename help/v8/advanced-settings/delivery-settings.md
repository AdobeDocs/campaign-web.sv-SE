---
audience: end-user
title: Avancerade inställningar
description: Webbdokumentation för Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 96d5ee712131ba314ef25736e421efe436d5170a
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 17%

---

# Avancerade inställningar {#advanced-settings}

![](../assets/do-not-localize/badge.png)

>[!NOTE]
>
>Dokumentationen håller på att byggas och uppdateras ofta. Den slutliga versionen av detta innehåll är klar i januari 2023.

Dessa inställningar **tekniska leveransparametrar** som definieras i e-postmallen. Om du vill ändra någon av dem för en viss leverans, ska du vara försiktig.

## Inställningar för e-postleverans {#email-delivery-settings}

>[!NOTE]
>
> Ändra bara inställningarna, inga nya alternativ tillåts. Beror på åtkomsträttigheter.

## Typologi {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologi"
>abstract="Med typologi kan du styra, filtrera och övervaka leveransen."

Typologier är uppsättningar av **typologiregler** som körs under fasen för analys av meddelande. Med dem kan du se till att dina e-postmeddelanden alltid innehåller vissa element (t.ex. en länk för att avbryta prenumerationen eller en ämnesrad) eller filtreringsregler som utesluter grupper från det avsedda målet (t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder).

När du associerar en typologi med ett meddelande eller en meddelandemall kommer de typologiregler som ingår i typologin att köras för att kontrollera meddelandets giltighet.

### Tryckparametrar {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Leveransvikt"
>abstract="Med leveransvikter kan ni identifiera leveranser med högsta prioritet inom ramen för tryckhantering. Meddelanden med högst vikt har prioritet."

I det här avsnittet kan du definiera en **tröskelvärde**. Det här är det maximala antalet meddelanden som kan skickas till en profil under en viss period. När denna tröskel har uppnåtts kan inga fler leveranser göras förrän efter den beaktade perioden. Med den här processen kan du automatiskt utesluta en profil från en leverans om ett meddelande överskrider det angivna tröskelvärdet och på så sätt undvika för många begäranden.

Tröskelvärden kan vara antingen konstanta eller variabla. Detta innebär att tröskelvärdena för en viss period kan variera från en profil till en annan eller till och med för samma profil.

I **Breddtyp** finns det tre alternativ: (formeln saknas beroende på alternativ..)

* **Konstant**
* **Beroende på mottagaren**
* **Definieras i varje regel**

The **Leveransvikt** fält: Varje leverans har en vikt som motsvarar dess prioritetsnivå. Som standard är vikten för en leverans inställd på 5. Med tryckregler kan du definiera vikten för de leveranser som de ska tillämpas på. Vikter kan antingen anges eller beräknas med en formel som passar mottagarna. Du kan till exempel definiera vikten för en leverans baserat på mottagarens intressen.

The **Leveransläge** fält.. ?

* **Målberäkning och meddelandepersonalisering**
* **Uppskattning och godkännande av det preliminära målet**
* **Målutvärdering**

### Kapacitetsinställningar {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Mottagarens betydelse"
>abstract="Mottagarens betydelse är en formel som används för att avgöra vilka mottagare som behålls när reglerna för kapacitetstypologi överskrids."

I det här avsnittet kan du välja en kapacitetsregel som definieras i Adobe Campaign v8-konsolen. Den här regeln är kopplad till e-postkanalen.

The **mottagarens vikt** fält är en formel som används för att bestämma vilka mottagare som ska behållas när reglerna för kapacitetstypologi överskrids.

## Målgrupp {#audience}

I det här avsnittet kan du välja en **målmappning** definieras i Adobe Campaign v8-konsolen. Målmappning måste skapas om du använder en annan mottagartabell än den som finns i Adobe Campaign.

## Leverans {#delivery}

**Routning** markering: Det externa kontot för integrerad e-postroutning tillhandahålls som standard. Den innehåller de tekniska parametrar som gör att programmet kan skicka e-post.

**Testa SMTP-leverans**: Använd det här alternativet om du vill testa att skicka via SMTP. Leveransen behandlas upp till anslutningen till SMTP-servern men skickas inte: för varje mottagare av leveransen ansluter Campaign till SMTP-providerservern, kör SMTP RCPT TO-kommandot och stänger anslutningen före SMTP DATA-kommandot.

**BCC för e-post**: Använd det här alternativet om du vill lagra e-post på ett externt system via BCC genom att lägga till en e-postadress för hemlig kopia till meddelandemålet.

### Återförsök {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximalt antal återförsök"
>abstract="Om ett meddelande misslyckas på grund av ett tillfälligt fel, kommer nya försök att utföras under leveransens varaktighet."

Meddelanden som inte har levererats tillfälligt på grund av ett mjukt eller ignorerat fel kan återförsökas automatiskt. Som standard schemaläggs fem återförsök till leveransdagens första dag med ett minsta intervall på en timme som sprids ut över dagens 24 timmar. Ett nytt försök per dag programmeras efter detta och fram till leveransdatumet, som definieras på fliken Giltighet.

## Godkännande {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Godkännandeläge"
>abstract="Varje steg i en leverans kan godkännas för att säkerställa full övervakning och kontroll av de olika processerna."

**Manuell**: I slutet av analysfasen måste användaren bekräfta leveransen för att kunna börja skicka.

**Halvautomatisk**: Skicka börjar automatiskt om analysfasen inte genererar några varningsmeddelanden.

**Automatisk**: Sändningen börjar automatiskt i slutet av analysfasen, oavsett resultatet.


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

### Hantering av spegelsidor {#mirror}

**Hantering av spegelsidor** innehåller fyra alternativ:

* **Generera spegelsidan om en spegellänk visas i e-postinnehållet**: spegelsidan genereras om länken infogas i postinnehållet.
* **Framtvinga generering av spegelsidan**: Spegelsidan skapas även om ingen länk till spegelsidan infogas i meddelandena.
* **Generera inte spegelsidan**: Ingen spegelsida genereras, även om länken finns i meddelandena.
* **Skapar en spegelsida som bara är tillgänglig med meddelandets identifierare**: Med det här alternativet kan du komma åt spegelsidans innehåll, med anpassningsinformation, i leveransloggfönstret.


### Spåra {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Giltighetsperiod"
>abstract="Det här alternativet anger hur länge spårningen ska aktiveras på URL-adresserna."

**Giltighetsgräns för spårning**: Det här alternativet anger hur länge spårningen ska aktiveras på URL-adresserna.

**Ersättnings-URL för utgångna URL:er**: Använd det här alternativet om du vill ange en URL till en reservwebbsida: den visas när spårningen har upphört att gälla.


## Testinställningar {#test-setttings}

**Håll ihop** Med kan du auktorisera flera leveranser till mottagare som uppfyller flera målinriktningskriterier.

**Behåll blocklist adresser** Med kan du hålla profiler som inte längre används av leveransen, t.ex. efter en avanmälan (avanmälan), kvar från målet.

**Behåll adresser i karantän** gör att du kan hålla profiler med en adress som inte svarar från målet.

**Behåll leveranskoden för korrekturet** Med kan du ge beviset samma leveranskod som den som är definierad för den leverans som det hör till.

Som standard anges korrekturens ämne med&quot;Korrekturnr&quot;, där # är numret på beviset. Du kan ändra det här prefixet i **Etikettprefix** fält.