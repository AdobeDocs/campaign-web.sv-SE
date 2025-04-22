---
title: Versionsinformation om webbanvändargränssnittet i Campaign v8
description: 2024 Campaign Web User Interface-versioner
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '2501'
ht-degree: 7%

---

# Versionsinformation 2024 {#2024-release}

På den här sidan visas alla ändringar och förbättringar som är tillgängliga i **2024-utgåvor**. De senaste versionskommentarerna är tillgängliga på [den här sidan](release-notes.md).


## 24 oktober {#24-10-release}

**Releasedatum**: 29 okt 2024

Följande funktioner och förbättringar är tillgängliga från och med oktober.

### Funktioner

<table>
<thead>
<tr>
<th><strong>Externa konton</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du konfigurera och hantera externa konton direkt via Adobe Campaign webbanvändargränssnitt. Den här nya funktionen gör det enkelt att konfigurera olika typer av externa konton, till exempel studentmeddelanden (POP3) eller exekveringsinstanser.</p>
<p>Mer information finns i den <a href="../administration/external-account.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transaktionsmeddelanden</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Transactional Messaging (Message Center) är nu tillgängligt i webbgränssnittet för Campaign. Det här tillägget är utformat för att utlösa meddelanden som genereras från händelser som utlöses från informationssystem, och kan vara: faktura, orderbekräftelse, leveransbekräftelse, lösenordsändring, meddelande om produkttillgänglighet, kontobesked, skapande av webbkonto osv.</p>
<p>Mer information finns i den <a href="../transactional-messaging/transactional.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>


### Förbättringar

* **Arbetsflödesaktiviteter** - Du kan nu flytta en aktivitet och alla dess underordnade noder från en övergång till en annan i ett arbetsflöde. En dedikerad **Flytta**-knapp är tillgänglig i aktivitetens egenskapspanel för att utföra detta. [Läs mer](../workflows/orchestrate-activities.md#move)

* **Aktivitet för arbetsflödesberikning**

   * Du kan nu definiera ett alias och en etikett när du skapar ett nytt fält i aktiviteten **Enrichment**. [Läs mer](../workflows/activities/enrichment.md#collection-settings)
   * Nu kan du lägga till erbjudanden för varje profil i aktiviteten **Enrichment**. [Läs mer](../workflows/activities/enrichment.md##add-offers)

* **Distribution av värden** - Vid åtkomst till listan med fält för anpassning kan du nu kontrollera hur värden distribueras för varje fält. Ett dedikerat popup-fönster visar antalet och procentandelen för varje värde. [Läs mer](../query/build-query.md#distribution-values-query)

* **Version- och systeminformation** - Nu kan du komma åt information om dina instansversioner, både för klientkonsolen och webbanvändargränssnittet. I det nya avsnittet visas även alla inbyggda paket som är installerade i din miljö. [Läs mer](../get-started/user-interface.md#user-interface-about)

* **Listor** - Nu kan du enkelt ändra ordningen på värdena i en lista. [Läs mer](../get-started/work-with-folders.md)

* **Leverans** - Leveransvariabeln är nu tillgänglig från personaliseringsfält. [Läs mer](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## September-uppdateringar {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI Assistant</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>När du har skapat och skräddarsytt ditt budskap går du ett steg längre med AI Assistant på Adobe Campaign Web. Med det här kraftfulla verktyget kan du optimera effekten av ditt innehåll genom att generera en mängd engagerande text, huvudtitlar och visuellt tilltalande bilder.</p>
<p>Fördjupa dig i en praktisk upplevelse med <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">vår förhandsvisning av aktiva funktioner</a>, som är utformad för att du först ska kunna utforska dess funktioner och till fullo förstå dess funktioner.</a>.</p>
<p>Mer information finns i den <a href="../email/generative-gs.md">detaljerade dokumentationen</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Tillgänglighetsdatum: 12 sept</p>
</td>
</tr>
</tbody>
</table>

## Augustiversion {#24-8-release}

**Releasedatum**: 3 september 2024

Följande funktioner och förbättringar är tillgängliga från och med augusti.

* **SMTP-parametrar** - SMTP-inställningar är nu tillgängliga i inställningarna för e-postleverans. [Läs mer](../advanced-settings/delivery-settings.md#smtp)

* **Globala variabler** - Nu kan du definiera globala variabler för att definiera värden för leveranser. [Läs mer](../advanced-settings/delivery-settings.md#variables-delivery)

### Nya funktioner i begränsad tillgänglighet {#acs-24-8}

>[!AVAILABILITY]
>
>Följande funktioner är i Begränsad tillgänglighet (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.
>
>Se följande dokumentationssidor: [Campaign Standard övergång till Campaign v8](../rn/acs-migration.md) och [Funktioner för Campaign Standard-användare](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}.

* **Varumärkning för direktreklam** - Tekniska administratörer kan nu definiera ett eller flera varumärken för att centralisera parametrarna som påverkar ett varumärkes identitet. Detta inkluderar logotypen, domänen för landningssidans åtkomst-URL eller inställningar för meddelandespårning. Nu kan du skapa dessa varumärken och länka dem till meddelanden eller landningssidor. Den här konfigurationen hanteras i mallar. [Läs mer](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Prenumerationer med landningssidor** - Nu kan du länka en landningssida till en tjänst och skicka ett bekräftelsemeddelande när användare validerar den. [Läs mer](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visuella fragment** - Nu kan du arkivera visuella innehållsfragment. [Läs mer](../content/create-fragment.md#archive)

* **Captcha på landningssidor** - Nu kan du lägga till captcha för att skydda din landningssida från skräppost och missbruk som orsakas av bottnar. Detta är icke-störande för kunderna eftersom det inte kräver någon interaktion från dem och baseras på interaktioner med webbplatsen. [Läs mer](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->


## Versionsinformation juli {#24-7-release}

**Releasedatum**: 30-31 juli 2024

Följande funktioner och förbättringar är tillgängliga från och med juliversionen.

### Innehållsfragment {#24-7-1}

Nu kan du skapa och använda innehållsfragment. Ett innehållsfragment är en återanvändbar komponent som kan refereras i ett eller flera meddelanden. När du ändrar ett fragment uppdateras allt innehåll som använder det. Med den här funktionen kan man skapa flera anpassade innehållsblock som kan användas av marknadsföringsanvändare för att snabbt sammanställa meddelandeinnehåll i en förbättrad designprocess.

Det finns två typer av fragment:

* **Uttrycksfragment** är fördefinierade uttryck som är tillgängliga från en dedikerad post i uttrycksredigeraren.
* **Visuella fragment** är fördefinierade visuella block som du kan återanvända i flera e-postleveranser eller i innehållsmallar. [Läs mer](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**Visuella fragment** har begränsad tillgänglighet (LA). Den här funktionen är begränsad till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

### Svällningsgrupp {#24-7-2}

En **svällningsgrupp** är en lista med dirigerade adresser. Det används för att inkludera specifika adresser i leveranser och sedan målprofiler som inte matchar de definierade målvillkoren. På så sätt kan mottagare som inte är leveranskänsliga ta emot leveransen på samma sätt som andra målmottagare. Du kan använda dirigerade adresser när du skickar korrektur eller för att skydda din e-postlista. [Läs mer](../audience/trap-group.md)

### Multipla mallar för push-meddelanden {#24-7-3}

Nu kan du skicka omfattande push-meddelanden. Ett omfattande push-meddelande är en förbättrad form av mobilmeddelanden som går längre än enkla textmeddelanden genom att infoga multimediaelement som bilder, interaktiva knappar eller annat multimediematerial. I den här versionen finns det nu en uppsättning mallar för push-meddelanden för dina iOS- och Android-appar.

[Läs mer](../push/rich-push.md)

>[!AVAILABILITY]
>
>Den här funktionen kräver en uppdatering av Campaign v8.6.3 <!--or v8.7.2-->. Läs mer i Versionsinformation för Campaign v8-klientkonsolen [på Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes){target="_blank"}.

### Förbättringar {#improvements-24-7}

**Mapphantering** - Nu kan du hantera behörigheter och begränsningar för mappar.

## Versionsinformation för juni {#24-6-release}

**Releasedatum**: 18-19 juni 2024

Följande funktioner och förbättringar är tillgängliga för alla användare från och med juni.

### Leveransvarningar {#24-6-3}

Funktionen för leveransvarning är ett varningssystem som gör att en grupp användare automatiskt kan ta emot meddelanden som innehåller information om hur leveransen utförs. [Läs mer](../msg/delivery-alerting.md)

### Planer och program {#24-6-4}

Nu kan ni skapa planer och program för att ordna era kampanjer. Genom att definiera en mapphierarki kan ni ordna era kampanjer i program och era program i planer. [Läs mer](../administration/plans-programs.md)

### Förbättringar {#improvements-24-6}

* **Avstämning i anrikningsaktivitet**: Aktiviteten **Anrikning** kan nu användas för att stämma av data från Campaign-databasschemat med data från ett annat schema, eller med data från ett temporärt schema, till exempel data som överförts med en Läs in filaktivitet. Du kan till exempel använda det här alternativet för att stämma av en profils land, som anges i en överförd fil, med något av de länder som är tillgängliga i den dedikerade tabellen i Campaign-databasen. [Läs mer](../workflows/activities/enrichment.md)

## Versionsinformation {#24-5-release}

**Releasedatum**: 21 maj 2024

Följande funktioner och förbättringar är tillgängliga för alla användare från och med majversionen.

### Granskningskedja  {#24-5-1}

Den nya funktionen **Granskningsspår** ger en detaljerad och kronologisk registrering av alla åtgärder och händelser som har utförts i din Adobe Campaign-instans i realtid. Den erbjuder en praktisk metod för att spåra alla ändringar av era Campaign-data, till exempel frågor som status för arbetsflöden, de senaste personerna att ändra dem eller aktiviteter som utförs av användare i instansen. [Läs mer](../reporting/audit-trail.md)

### Anpassade fält {#24-5-2}

**Anpassade fält** är ytterligare attribut som läggs till i scheman som är klara att användas via Adobe Campaign-konsolen. I webbgränssnittet för Campaign är dessa anpassade fält nu synliga på olika skärmar, till exempel information om en profil eller en testprofil. I webbanvändargränssnittet kan du inte skapa anpassade fält, men du kan nu ändra hur de visas. [Läs mer](../administration/custom-fields.md)

### Skapa länkar mellan tabeller {#24-5-3}

Nu kan du skapa länkar med en annan tabell i arbetsflödesaktiviteten **Berikning**. Använd det nya avsnittet **Länkdefinition** i aktivitetsparametrarna för att skapa en länk mellan arbetstabelldata och Adobe Campaign-databasen. Om du till exempel läser in data från en fil som innehåller mottagarnas kontonummer, land och e-postadress, kan du nu skapa en länk till landstabellen för att uppdatera informationen i deras profiler. [Läs mer](../workflows/activities/enrichment.md#create-links)

### Allmänna förbättringar {#improvements-24-5}

* **Direktutskick** - Nu kan du använda uttrycksredigeraren för att välja vilka attribut som ska visas i extraheringsfiler för direktutskick. [Läs mer](../direct-mail/content-direct-mail.md)

* **Mapphantering** - Nu kan du skapa en undermapp av en annan typ än den överordnade mappen. [Läs mer](../get-started/permissions.md#folders)

* **Globalisering** - Som en del av vår pågående strävan att leverera en enhetlig användarupplevelse harmoniserar vi terminologin som används i Adobe Experience Cloud-produkter och -appar. Det här påverkar den tyska termen &quot;Titel&quot; som ändras till &quot;Label&quot; när det gäller namnet på ett objekt. Ändringarna införs stegvis i användargränssnittet och dokumentationen.


## Versionsinformation, april {#april-24-4-release}

**Releasedatum**: 2 maj 2024

### Nya funktioner {#new-24-4}

Följande funktioner är tillgängliga för alla användare från och med aprilversionen.

**Nya arbetsflödesaktiviteter**

* **Uppdatera data** - Använd den här aktiviteten för att utföra massuppdateringar på fält i databasen. Flera alternativ gör att du kan anpassa datauppdateringen. [Läs mer](../workflows/activities/update-data.md)
* **Prenumerationstjänster** - Använd den här aktiviteten om du vill prenumerera på eller avbryta prenumeration på flera profiler till/från en tjänst i en enda åtgärd. [Läs mer](../workflows/activities/subscription-services.md)
* **Extrahera fil** - Använd den här aktiviteten om du vill exportera data från Adobe Campaign till ett annat system som en extern fil. [Läs mer](../workflows/activities/extract-file.md)
* **Överför fil** - Använd den här aktiviteten om du vill ta emot eller skicka filer, testa om det finns filer eller lista över filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll. [Läs mer](../workflows/activities/transfer-file.md)
* **Test** - Använd den här aktiviteten för att aktivera övergångar baserat på angivna villkor. [Läs mer](../workflows/activities/test.md)
* **JavaScript-kod** - Använd den här aktiviteten för att köra ett JavaScript-kodfragment i ett arbetsflödes sammanhang. [Läs mer](../workflows/activities/javascript-code.md)
* **Extern signal** - Använd den här aktiviteten för att utlösa ett arbetsflödes körning från ett annat arbetsflöde eller ett API-anrop. [Läs mer](../workflows/activities/external-signal.md)
* **Inkrementell fråga** - Använd den här aktiviteten för att fråga databasen på schemalagd basis. Varje gång den här aktiviteten körs utesluts resultaten från tidigare körningar. På så sätt kan du bara rikta in dig på nya element. [Läs mer](../workflows/activities/incremental-query.md)

**Mallar för avancerade push-meddelanden**

Nu kan du skicka omfattande push-meddelanden via Android. Rich push notification är en förbättrad form av mobilmeddelanden som går utöver enkla textmeddelanden genom att införliva multimediaelement som bilder, interaktiva knappar eller annat multimediematerial. [Läs mer](../push/rich-push.md)

Observera att den här funktionen är i **begränsad tillgänglighet** (LA).


### Nya funktioner i begränsad tillgänglighet {#acs-24-4}

>[!AVAILABILITY]
>
>Följande funktioner är i Begränsad tillgänglighet (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.
>
>Se följande dokumentationssidor: [Campaign Standard övergång till Campaign v8](../rn/acs-migration.md) och [Funktioner för Campaign Standard-användare](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Varumärke** - Som en migrerad Campaign Standard-användare kan teknikadministratörer nu definiera ett eller flera varumärken för att centralisera parametrarna som påverkar ett varumärkes identitet. Detta inkluderar logotypen, domänen för landningssidans åtkomst-URL eller inställningar för meddelandespårning. Du kan skapa dessa varumärken och länka dem till meddelanden eller landningssidor. Den här konfigurationen hanteras i mallar. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Övriga API:er** - Som en Campaign Standard-migrerad användare kan du använda Rest API:er för att skapa integreringar för Adobe Campaign och skapa ett eget ekosystem genom att interagera med Adobe Campaign med den panel med tekniker som du använder. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Dynamisk rapportering** - Som migrerad Campaign Standard-användare har du tillgång till Dynamic Reporting som tillhandahåller fullt anpassningsbara realtidsrapporter för att mäta effekten av dina marknadsföringsaktiviteter. Det ger åtkomst till profildata, vilket möjliggör demografiska analyser efter profildimensioner som kön, ort och ålder, utöver funktionella e-postkampanjdata som öppningar och klick. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Landningssidor** - Följande förbättringar av landningssidor är bara tillgängliga för användare som övergår från Campaign Standard:

   * Du kan nu hänvisa till en standardstartsida för prenumeration/avprenumeration när du konfigurerar en tjänst. När du utformar ett e-postmeddelande och definierar en länk till den landningssidan, prenumererar användare som skickar landningssidans formulär automatiskt på eller avbryter prenumerationen på den här tjänsten. [Läs mer](../audience/manage-services.md#create-service)
   * Ett nytt alternativ i landningssidans konfiguration gör att anonyma besökare kan komma åt landningssidan. Om du avmarkerar det här alternativet kan endast identifierade användare få åtkomst till och skicka formuläret. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Ett nytt alternativ i landningssidans konfiguration gör det möjligt att lagra ytterligare interna data när landningssidan skickas. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Med ett nytt alternativ kan du använda en landningssida för flera tjänster, vilket gör den dynamisk. När du lägger till en länk till ett e-postmeddelande kan du välja vilken tjänst som helst om du väljer en dynamisk landningssida. Om du väljer en landningssida som har en specifik tjänst kopplad till, kommer den här tjänsten att användas automatiskt (du kan inte välja en annan). [Läs mer](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Villkorligt innehåll stöds nu på landningssidor. [Läs mer](../landing-pages/lp-content.md)

### Allmänna förbättringar {#improvements-24-4}

Förbättringarna nedan är tillgängliga för alla kunder från och med aprilversionen.

* Aktiviteten **Läs in fil** har förbättrats med flera avsnitt som gör att du kan överföra en exempelfil, hantera fel och avvisa samt ta bort överförda filer när aktiviteten har körts. [Läs mer](../workflows/activities/load-file.md)


* Du kan nu **kopiera/klistra in aktiviteter** från ett arbetsflöde till ett annat arbetsflöde från en annan webbläsarflik. [Läs mer](../workflows/orchestrate-activities.md#copy-activities-copy)

* Alla arbetsflödesaktiviteter tillåter nu att du hanterar deras **körningsalternativ**. På så sätt kan du definiera aktivitetens körningsläge och beteende vid fel. [Läs mer](../workflows/orchestrate-activities.md#execution-options-execution)

* Alternativet&quot;Aktivera inte övergången om populationen är tom&quot; i **Delad aktivitet** gör att du kan välja om arbetsflödet ska övergå till nästa aktivitet när segmentresultatet är tomt. [Läs mer](../workflows/activities/split.md)

## Versionsinformation om mars {#24-3-release}

>[!AVAILABILITY]
>
>Den här versionen är tillgänglig för alla användare som startar [Campaign (konsol) version 8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html). Läs mer om Adobe Campaign klientkonsolversioner och uppgraderingar i [dokumentationen för Campaign v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html){target="_blank"}.

**Releasedatum**: 19-20 mars 2024

### Direktreklam, kanal {#24-3-dm}

Kanalen **Direktreklam** är nu tillgänglig för användning i arbetsflöden och som fristående leveranser. Direktreklam är en offlinekanal som gör att du kan skapa, anpassa och generera extraheringsfiler och dela dem med direktreklamleverantörer för att skicka e-post till kunderna.

### Ny arbetsflödesaktivitet för Ändra datakälla {#24-3-change-data-source}

Med målaktiviteten **Ändra datakälla** kan du ändra datakällan som används i arbetsflödets arbetsregister. Den här aktiviteten ger större flexibilitet genom att du kan hantera data i olika databaser och förbättra prestandan.

### Förbättring av delad arbetsflödesaktivitet {#24-3-split}

Nu kan du använda alternativet **Generera alla delmängder i samma tabell** i arbetsflödesaktiviteten **Dela** för att gruppera alla delmängder i en enda utdataövergång.

### Frågemodelleraren {#24-3-query-modeler}

* Frågemodelleraren är nu tillgänglig för användning i e-post-Designer. Du kan skapa villkor när du skapar villkorsstyrt innehåll.
* Fördefinierade värden är nu tillgängliga för datumtypsattribut när du skapar ett anpassat villkor.
* Det går inte längre att lägga till operatorer för en ny övergång i diagrammet. De kan bara läggas till i en befintlig övergång innan komponenterna filtreras för att gruppera dem.