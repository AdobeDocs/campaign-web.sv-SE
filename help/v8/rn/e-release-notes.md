---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: a1bc0459c093389104768c4eabc825b551ffba3f
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 6%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

## Versionsinformation {#24-5-release}

**Releasedatum**: 21 maj 2024

Följande funktioner och förbättringar är tillgängliga för alla användare från och med majversionen.

### Granskningskedja  {#24-5-1}

Den nya **Granskningsspår** funktionen ger en detaljerad och kronologisk redovisning av alla åtgärder och händelser som har utförts i din Adobe Campaign-instans i realtid. Den erbjuder en praktisk metod för att spåra alla ändringar av era Campaign-data, till exempel frågor som status för arbetsflöden, de senaste personerna att ändra dem eller aktiviteter som utförs av användare i instansen. [Läs mer](../reporting/audit-trail.md)

### Anpassade fält {#24-5-2}

**Anpassade fält** är ytterligare attribut som läggs till i färdiga scheman via Adobe Campaign-konsolen. I webbgränssnittet för Campaign är dessa anpassade fält nu synliga på olika skärmar, till exempel information om en profil eller en testprofil. I webbanvändargränssnittet kan du inte skapa anpassade fält, men du kan nu ändra hur de visas. [Läs mer](../administration/custom-fields.md)

### Skapa länkar mellan tabeller {#24-5-3}

Nu kan du skapa länkar med en annan tabell i **Berikning** arbetsflödesaktivitet. Använd den nya **Länkdefinition** i aktivitetsparametrarna för att skapa en länk mellan arbetstabelldata och Adobe Campaign-databasen. Om du till exempel läser in data från en fil som innehåller mottagarnas kontonummer, land och e-postadress, kan du nu skapa en länk till landstabellen för att uppdatera informationen i deras profiler. [Läs mer](../workflows/activities/enrichment.md#create-links)

<!--
### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.-->


### Allmänna förbättringar {#improvements-24-5}

* **Direktreklam** - Du kan nu använda uttrycksredigeraren för att välja vilka attribut som ska visas i extraheringsfiler för direktreklam. [Läs mer](../direct-mail/content-direct-mail.md)

* **Mapphantering** - Du kan nu skapa en undermapp av en annan typ än den överordnade mappen. [Läs mer](../get-started/permissions.md#folders)


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

* **Globalisering** - Som en del av vårt pågående arbete med att leverera en enhetlig användarupplevelse harmoniserar vi terminologin som används i Adobe Experience Cloud produkter och appar. Det här påverkar den tyska termen &quot;Titel&quot; som ändras till &quot;Label&quot; när det gäller namnet på ett objekt. Ändringarna införs stegvis i användargränssnittet och dokumentationen.


## Versionsinformation, april {#april-24-4-release}

**Releasedatum**: 2 maj 2024

### Nya funktioner {#new-24-4}

Följande funktioner är tillgängliga för alla användare från och med aprilversionen.

**Nya arbetsflödesaktiviteter**

* **Uppdatera data** - Använd den här aktiviteten för att utföra massuppdateringar på fält i databasen. Flera alternativ gör att du kan anpassa datauppdateringen. [Läs mer](../workflows/activities/update-data.md)
* **Prenumerationstjänster** - Använd den här aktiviteten om du vill prenumerera eller avbryta prenumeration på flera profiler till/från en tjänst i en enda åtgärd. [Läs mer](../workflows/activities/subscription-services.md)
* **Extrahera fil** - Använd den här aktiviteten om du vill exportera data från Adobe Campaign till ett annat system som en extern fil. [Läs mer](../workflows/activities/extract-file.md)
* **Överföringsfil** - Använd den här aktiviteten om du vill ta emot eller skicka filer, testa om det finns filer eller lista med filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll. [Läs mer](../workflows/activities/transfer-file.md)
* **Testa** - Använd den här aktiviteten för att aktivera övergångar baserat på angivna villkor. [Läs mer](../workflows/activities/test.md)
* **JavaScript-kod** - Använd den här aktiviteten för att köra ett JavaScript-kodfragment i ett arbetsflödes sammanhang. [Läs mer](../workflows/activities/javascript-code.md)
* **Extern signal** - Använd den här aktiviteten för att utlösa körningen av ett arbetsflöde från ett annat arbetsflöde eller ett API-anrop. [Läs mer](../workflows/activities/external-signal.md)
* **Inkrementell fråga** - Använd den här aktiviteten för att fråga databasen på schemalagd basis. Varje gång den här aktiviteten körs utesluts resultaten från tidigare körningar. På så sätt kan du bara rikta in dig på nya element. [Läs mer](../workflows/activities/incremental-query.md)

**Mallar för push-meddelanden**

Nu kan du skicka omfattande push-meddelanden via Android. Rich push notification är en förbättrad form av mobilmeddelanden som går utöver enkla textmeddelanden genom att införliva multimediaelement som bilder, interaktiva knappar eller annat multimediematerial. [Läs mer](../push/rich-push.md)

Observera att den här funktionen är **Begränsad tillgänglighet** (LA).


### Nya funktioner i begränsad tillgänglighet {#acs-24-4}

>[!AVAILABILITY]
>
>Följande funktioner är i Begränsad tillgänglighet (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.
>
>Se följande dokumentationssidor: [Campaign Standard över till Campaign v8](../rn/acs-migration.md) och [Funktioner för Campaign Standarder](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Varumärke** - Som en Campaign Standard migrerad användare kan era tekniska administratörer nu definiera ett eller flera varumärken för att centralisera de parametrar som påverkar ett varumärkes identitet. Detta inkluderar logotypen, domänen för landningssidans åtkomst-URL eller inställningar för meddelandespårning. Du kan skapa dessa varumärken och länka dem till meddelanden eller landningssidor. Den här konfigurationen hanteras i mallar. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Övriga API:er** - Som användare med migrerad Campaign Standard kan du använda de övriga API:erna för att skapa integreringar för Adobe Campaign och bygga ett eget ekosystem genom att interagera med Adobe Campaign med den tekniska panel som du använder. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Dynamisk rapportering** - Som användare med migrerad Campaign Standard har ni tillgång till Dynamic Reporting, som tillhandahåller fullt anpassningsbara realtidsrapporter för att mäta effekten av era marknadsföringsaktiviteter. Det ger åtkomst till profildata, vilket möjliggör demografiska analyser efter profildimensioner som kön, ort och ålder, utöver funktionella e-postkampanjdata som öppningar och klick. [Läs mer](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Landningssidor** - Följande förbättringar av landningssidor är endast tillgängliga för användare som går över från Campaign Standard:

   * Du kan nu hänvisa till en standardstartsida för prenumeration/avprenumeration när du konfigurerar en tjänst. När du utformar ett e-postmeddelande och definierar en länk till den landningssidan, prenumererar användare som skickar landningssidans formulär automatiskt på eller avbryter prenumerationen på den här tjänsten. [Läs mer](../audience/manage-services.md#create-service)
   * Ett nytt alternativ i landningssidans konfiguration gör att anonyma besökare kan komma åt landningssidan. Om du avmarkerar det här alternativet kan endast identifierade användare få åtkomst till och skicka formuläret. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Ett nytt alternativ i landningssidans konfiguration gör det möjligt att lagra ytterligare interna data när landningssidan skickas. [Läs mer](../landing-pages/create-lp.md#create-landing-page)
   * Med ett nytt alternativ kan du använda en landningssida för flera tjänster, vilket gör den dynamisk. När du lägger till en länk till ett e-postmeddelande kan du välja vilken tjänst som helst om du väljer en dynamisk landningssida. Om du väljer en landningssida som har en specifik tjänst kopplad till, kommer den här tjänsten att användas automatiskt (du kan inte välja en annan). [Läs mer](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Villkorligt innehåll stöds nu på landningssidor. [Läs mer](../landing-pages/lp-content.md)

### Allmänna förbättringar {#improvements-24-4}

Förbättringarna nedan är tillgängliga för alla kunder från och med aprilversionen.
<!--**Workflow - Copy/Paste into another tab**: -->

* The **Läs in fil** -aktiviteten har förbättrats med flera avsnitt som gör att du kan överföra en exempelfil, hantera fel och ignorera samt ta bort överförda filer när aktiviteten har körts. [Läs mer](../workflows/activities/load-file.md)


* Nu kan du **kopiera/klistra in aktiviteter** från ett arbetsflöde till ett annat arbetsflöde från en annan webbläsarflik. [Läs mer](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Nu kan du hantera alla arbetsflödesaktiviteter **körningsalternativ**. På så sätt kan du definiera aktivitetens körningsläge och beteende vid fel. [Läs mer](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* Alternativet&quot;Aktivera inte övergången om populationen är tom&quot; i **Delad aktivitet** Med kan du välja om arbetsflödet ska övergå till nästa aktivitet när segmentresultatet är tomt. [Läs mer](../workflows/activities/split.md)



## Versionsinformation om mars {#24-3-release}

>[!AVAILABILITY]
>
>Den här versionen är tillgänglig för alla användare som startar [Campaign (konsol) version 8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html). Läs mer om Adobe Campaign kundkonsoluppdateringar och uppgraderingar i [Kampanjdokumentation v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html){target="_blank"}.

**Releasedatum**: 19-20 mars 2024

### Direktreklam, kanal {#24-3-dm}

**Direktreklam** kanalen kan nu användas i arbetsflöden och som fristående leveranser. Direktreklam är en offlinekanal som gör att du kan skapa, anpassa och generera extraheringsfiler och dela dem med direktreklamleverantörer för att skicka e-post till kunderna.

### Ny arbetsflödesaktivitet för Ändra datakälla {#24-3-change-data-source}

The **Ändra datakälla** målaktiviteter gör att du kan ändra datakällan som används i arbetsflödets arbetsregister. Den här aktiviteten ger större flexibilitet genom att du kan hantera data i olika databaser och förbättra prestandan.

### Förbättring av delad arbetsflödesaktivitet {#24-3-split}

Nu kan du använda **Generera alla delmängder i samma tabell** i **Dela** arbetsflödesaktivitet för att gruppera alla delmängder i en enda utdataövergång.

### Frågemodelleraren {#24-3-query-modeler}

* Frågemodelleraren kan nu användas i e-postdesignern. Du kan skapa villkor när du skapar villkorsstyrt innehåll.
* Fördefinierade värden är nu tillgängliga för datumtypsattribut när du skapar ett anpassat villkor.
* Det går inte längre att lägga till operatorer för en ny övergång i diagrammet. De kan bara läggas till i en befintlig övergång innan komponenterna filtreras för att gruppera dem.
