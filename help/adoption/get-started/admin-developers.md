---
title: Kom igång med Adobe Campaign v8 för administratörer och utvecklare.
description: Den här självstudiekursen ger en översikt över de viktigaste administrativa funktionerna och datahanteringsfunktionerna i Campaign v8. Det riktar sig till administratörer och den tekniska marknadsföraren som migrerar från Campaign Standard till Campaign v8.
role: Admin, Developer
level: Beginner, Experienced
source-git-commit: a1c16a9ba5e5ca844eaf82ed3b587f4f7a0b0873
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Kom igång för administratörer och utvecklare {#acs-gs-admin}

Den här sidan ger en översikt över de viktigaste administrativa funktionerna och datahanteringsfunktionerna i Campaign v8. Det är till för administratörer och teknikmarknadsförare som går över från Campaign Standard till Campaign v8.

Den största förändringen för dig är introduktionen av klientkonsolen, det inbyggda programmet som kommunicerar med Adobe Campaign programserver.

Campaign-klientkonsolen centraliserar alla funktioner och inställningar. Den förblir synkroniserad med användargränssnittet i Campaign Web, vilket ger enhetlighet i båda miljöerna.

![](assets/client_console.png){zoomable="yes"}

[Läs mer om användargränssnittet i klientkonsolen i Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"} .

## Kampanjarkitektur v8 {#acs-gs-admi-archi}

Kampanjarkitekturen beskrivs i dokumentationen för Campaign v8 (konsol). Lär dig grunderna på [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"}.

Länk som du kan använda för att starta:

* Adobe Campaign-komponenter och global arkitektur beskrivs på [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"}.

* Se [Kom igång med Campaign-arkitekturen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} för att förstå Campaign-arkitekturen innan du börjar strukturera instansen.

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* Transactional messaging (Message Center) är modulen Campaign v8 som är utformad för att hantera utlösta meddelanden. Den bygger på en specifik arkitekturmodell som beskrivs i [det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"}.

## Kampanjklientkonsol {#acs-gs-console}

### Installera klientkonsolen {#acs-gs-admin-console}

Administration och konfigurering utförs i klientkonsolen. Det första steget är att konfigurera miljön.

Campaign-klientkonsolen är ett systemspecifikt program som kommunicerar med Adobe Campaign-programservern via standardInternetprotokoll, som SOAP och HTTP. Campaign-klientkonsolen centraliserar alla funktioner och inställningar och kräver minimal bandbredd eftersom den är beroende av ett lokalt cacheminne. Kampanjklientkonsolen är utformad för enkel driftsättning och kan distribueras från en webbläsare, uppdateras automatiskt och kräver ingen specifik nätverkskonfiguration eftersom den bara genererar HTTP(S)-trafik.

I följande video förklaras hur du hämtar och installerar Adobe Campaign Client Console och hanterar anslutningen till din instans.

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

Mer information finns i [Ansluta till kampanj med klientkonsolen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect){target="_blank"}.

Observera att klientkonsolen måste installeras i en miljö som stöds. Läs mer i [Kompatibilitetsmatrisen för Campaign v8 (konsol)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"}.

### Upptäck klientkonsolens gränssnitt  {#acs-gs-ui}

Lär dig mer om användargränssnittet i Adobe Campaign V8 och hur du navigerar bland huvudfunktionerna i den här självstudiekursen.

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

Mer information finns i [Arbeta med klientkonsolen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"}.

## Administrera miljön {#acs-gs-admin-env}

När klientkonsolen har installerats följer du stegen i den här dokumentationen för att skapa anslutningen till programservern: [Anslutning till programserverns dokumentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}.

Säkerhetsrutinerna är djupt integrerade i vår interna programutveckling och våra processer och verktyg för drift och följs noggrant av våra funktionsövergripande team för att förebygga, upptäcka och hantera incidenter på ett snabbt sätt. Läs mer i [Bästa praxis för kampanjsäkerhet](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security){target="_blank"}.

### Behörigheter och behörigheter {#acs-gs-admin-rights}

Med Adobe Campaign kan du definiera och hantera de behörigheter som tilldelats användare. Dessa behörigheter definieras genom att användargruppbehörigheter, namngivna rättigheter och behörigheter kombineras i mappar.

Som Campaign Standard-användare som går över till Campaign v8 har du samma behörigheter och åtkomsträttigheter. Säkerhetsgrupper har flyttats av Adobe till Campaign v8-operatorgrupperna och dina behörigheter per organisationsenhet har ändrats till mappbehörigheter. Kampanjanvändare   använda deras Adobe ID för att ansluta till Campaign v8 och sedan använda samma inloggning och lösenord som i Campaign Standarden.

Campaign [folders](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"} är noder i utforskarträdet i klientkonsolen. Beroende på vilken typ de har innehåller de vissa typer av data. Program materialiseras av mappar i Campaign v8. Du kan skapa mappar och hantera behörigheter för dem för att begränsa åtkomsten. [Läs mer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Läs mer i [dokumentationen om användarbehörigheter](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.


### Kontrollpanelen i Campaign {#acs-gs-admin-cp}

På samma sätt som för Campaign Standard kan du använda Kontrollpanelen för att administrera din miljö. Observera att för v8 har kontrollpanelen ytterligare funktioner.

Med Campaign Control Panel kan ni effektivisera arbetet som produktadministratör för Adobe Campaign genom att hantera inställningar och spåra användningen för var och en av instanserna. Det intuitiva gränssnittet låter dig enkelt övervaka användningen av nyckelresurser och utföra administrativa uppgifter såsom att lägga till IP-adresser i tillåtelselistan, övervaka SFTP-lagring, hantera nycklar och mycket annat.

Läs mer i [Kontrollpanelens självstudiekurser](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} och [dokumentationen på kontrollpanelen](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=sv){target="_blank"}.

* **Lägg till IP-adresser** - Med Campaign-kontrollpanelen kan du konfigurera nya anslutningar till dina instanser genom att lägga till IP-adressintervall i tillåtelselista. Läs mer i [Listdokumentationen för IP-tillåtna](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}

* **Underdomänskonfiguration** - Du kan konfigurera ett underavsnitt av din domän (tekniskt en &quot;DNS-zon&quot;) för användning med Adobe Campaign.
Läs mer i [dokumentationen om delegering av underdomäner](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}

* **Hantera SFTP-servrar** - På Kontrollpanelen kan du interagera med alla SFTP-servrar som är anslutna till Campaign-instanser som du har åtkomst till. Läs mer i [dokumentationen för SFTP-hantering](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}


### Granskningskedja {#acs-gs-admin-audit-trail}

Som redan finns i Campaign Standarden kan granskningsspåret användas i Campaign v8 för att få tillgång till hela historiken för ändringar som gjorts i instansen.

I Adobe Campaign webbanvändargränssnitt ger funktionen Granskningsspårning användarna full insyn i alla ändringar som görs i viktiga enheter i instansen, vanligtvis sådana som påverkar instansens smidiga funktion rejält. Läs mer i [Granskningsspårningsdokumentationen](../../v8/reporting/audit-trail.md)

### Datapaket {#acs-gs-admin-audit-packages}

På samma sätt som i Campaign Standard kan administratörer definiera paket för utbyte av resurser mellan olika Adobe Campaign-instanser via strukturerade XML-filer. Dessa kan vara konfigurationsparametrar eller data.

Du kan använda datapaket för att exportera och importera anpassade plattformsinställningar och data. Ett paket kan innehålla olika typer av konfigurationer och komponenter, filtrerade eller inte. Lär dig hur du arbetar med datapaket i Campaign v8 i [den här dokumentationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/packages){target="_blank"}.

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### Anpassa användargränssnittet {#acs-gs-admin-ui}

Det finns flera alternativ som du kan använda för att anpassa användargränssnittet i klientkonsolen, som:

* **Lista och datavisning** - Riktlinjer för hantering av användargränssnittsinställningar som listor, enheter och datavisning finns i det här dokumentet: [Dokumentation för användargränssnittsinställningar](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **Mapphantering** - Mappar är objekt i Adobe Campaign som gör att du kan ordna dina komponenter och data. De används också för att hantera behörigheter. Lär dig [arbeta med mappar](../../v8/get-started/work-with-folders.md).

* **Anpassade fält** - Anpassade fält är ytterligare attribut som läggs till i scheman som är klara att användas via Adobe Campaign-konsolen. Dessa anpassade fält visas på olika skärmar, till exempel information om en profil eller en testprofil. Läs mer i [dokumentationen för konfiguration av anpassade fält](../../v8/administration/custom-fields.md).

## Konfigurera varumärket {#acs-gs-admin-branding}

Alla företag har varumärkesriktlinjer som definierar både visuella element och tekniska detaljer. När det gäller Adobe Campaign Standard hjälper Adobe Campaign v8 er att hantera dessa riktlinjer centralt, så att ni kan presentera en enhetlig varumärkesbild för era kunder i allt ni gör, från logotyper i e-postmeddelanden till URL:er och domäner som används i era kampanjer. Som teknisk administratör kan du skapa och hantera flera varumärken inom Adobe Campaign.

Läs mer i [varumärkesdokumentationen](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}

## Förstå skapande av datamodell {#acs-gs-admin-data-model-creation}

På samma sätt som för Campaign Standard har Adobe Campaign v8 en fördefinierad datamodell. Adobe Campaign förlitar sig på en molndatabas som innehåller tabeller som är länkade tillsammans. Läs mer i [Datamodelldokumentationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}.

Ett schema är ett XML-dokument som är associerat med en databastabell. Den definierar datastrukturen och beskriver tabellens SQL-definition. Se [dokumentationen för att skapa scheman](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

Lär dig hur du skapar ett schema och hur du utökar ett befintligt schema i Campaign v8 i den här videon:

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

På samma sätt som i Campaign Standard kan du skapa anpassade resurser. I Campaign v8 är anpassade eller utökade **scheman** anpassade resurser.

* Lär dig hur du arbetar med schema på [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

* Lär dig hur du utökar ett befintligt schema på [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"}.

* Lär dig hur du skapar ett nytt schema på [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"}.

* När du skapar eller utökar ett schema måste du skapa eller ändra de associerade indataformulären för att göra ändringarna synliga för slutanvändarna. Med ett inmatningsformulär kan du redigera en instans som är associerad med ett dataschema från Adobe Campaign klientkonsol. Formuläret identifieras av dess namn och namnutrymme. Se [Skapa inmatningsdokumentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}.

## Arbetsflöden och datahantering {#acs-gs-admin-data-management}

På samma sätt som med Adobe Campaign Standard innehåller Adobe Campaign v8 en arbetsflödesmodul som gör det möjligt att samordna alla processer och uppgifter i olika moduler på programservern. I den omfattande grafiska miljön kan du utforma processer såsom segmentering, kampanjkörning, filhantering och mänskligt deltagande osv. Arbetsflödesmotorn kör och spårar dessa processer. Lär dig hur du börjar med arbetsflöden i Campaign v8 i [den här dokumentationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"}.

Se länkar till andra användbara resurser nedan:

* Läs om vilka målgruppsmått och arbetsregister som är och hur Adobe Campaign hanterar data från olika datakällor i den här videon:

  >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* Med Campaign kan du lägga till kontakter i molndatabasen. Du kan läsa in en fil, schemalägga och automatisera flera kontaktuppdateringar, samla in data på webben eller ange profilinformation direkt i mottagartabellen.  Läs mer i [Importera data (konsol) ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"}.

* Du kan enkelt exportera dina olika rapporter till PDF eller CSV-format så att du kan dela, ändra och skriva ut dem. Läs mer i [dokumentationen om dataexport](../../v8/reporting/export-reports.md).

## REST API:er {#acs-gs-admin-apis}

Campaign REST API:er är avsedda att göra det möjligt att skapa integreringar för Adobe Campaign och bygga ett eget ekosystem genom att interagera med Adobe Campaign med den panel med tekniker som ni använder.

Som Campaign Standard-användare som går över till Campaign v8 är REST API:er tillgängliga.

Läs mer i dokumentationen för [Rest API](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"}.

Observera att vissa rekommendationer och begränsningar gäller för REST API:er vid övergång från Campaign Standard till Campaign v8. De listas på [den här sidan](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"}. Specifika begränsningar gäller också vid övergång till Campaign v8 enligt listan i Tillgänglighetsmeddelandet nedan:

>[!AVAILABILITY]
>
>* PKEY-värdena ändras mellan den befintliga Campaign Standarden och den migrerade Campaign v8-instansen. Om PKEY:er lagras i en extern databas måste implementeringen ändras på ett sätt som de måste anropa Adobe Campaign v8-API:er, som tillhandahåller nycklar/hrefs-länkar med PKEY:er och efterföljande API-anrop måste formateras dynamiskt genom att nycklarna/hrefs från tidigare API-anrop används &#x200B;
>
>* I Campaign v8, för samma kropp där fordonet är länkat till profilen, &#x200B; ett fel skulle uppstå när egenskapen firstName inte är giltig för `cusVehicle`, men en begärandebrödtext med bara attributen utan länk fungerar bra. `{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* Tidszonen visas för användaren som en del av `profileAndServicesExt/profile` REST API-anrop och inte `profileAndServices/profile` REST API-anrop eftersom den läggs till i ett utökat schema som en del av datamigreringen. &#x200B;
>
>* `ccpaOptOut` visas bara för användaren som en del av `profileAndServicesExt/profile` REST API-anrop och inte `profileAndServices/profile` REST API-anrop eftersom det läggs till i ett utökat schema som en del av datamigreringen.
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## Prenumerationstjänster {#acs-gs-admin-sub}

Som administratör kan du som Campaign Standard skapa prenumerationstjänster och marknadsförare kan skicka meddelanden till sina prenumeranter. Viktiga koncept och implementeringssteg är anpassade efter Campaign Standard. Här finns användbara länkar och video.

Lär dig hur du konfigurerar och hanterar prenumerationer samt riktar dig till prenumeranter.

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

* Se prenumerationstjänsterna [Dokumentation för webbanvändargränssnittet](../../v8/audience/manage-subscribers.md).

* Se även dokumentationen för att ange prenumerationstjänster i klientkonsolen i [det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"}.

## Meddelanden och leveranser{#acs-gs-msg}

### Konfigurera leveranskanaler {#acs-gs-admin-channels}

Som Campaign Standard kan Adobe Campaign v8 hjälpa er att skicka flerkanalskampanjer, inklusive e-post, SMS, push-meddelanden och direktreklam, och mäta hur effektiva de är med hjälp av olika dedikerade rapporter. Dessa meddelanden är utformade och skickas genom leveranser och kan anpassas för varje mottagare. De viktigaste funktionerna är målinriktning, definition och personalisering av meddelanden, genomförande av kommunikation och tillhörande verksamhetsrapporter. Den huvudsakliga funktionella åtkomstpunkten är leveransassistenten. Den här åtkomstpunkten leder till flera funktioner som täcks av Adobe Campaign.

Som administratör måste du definiera kanalkonfigurationer. Läs mer på länkarna nedan.

* **E-post** - E-postinställningarna finns på [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"}.
* **SMS** - Lär dig hur du konfigurerar din SMS-kanal i [den här dokumentationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.
* **Push-meddelanden** - Steg för att konfigurera push-meddelandekanalen finns detaljerade [i det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
* **Transactional messaging** - Steg för att konfigurera [Transactional messaging](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"} i Campaign v8 beskrivs [i det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings)

### Externa konton {#acs-gs-ext-accounts}

Som administratör ansvarar du för att konfigurera och underhålla externa konton för Campaign. Som i Campaign Standard används externa konton av tekniska processer som tekniska arbetsflöden eller kampanjarbetsflöden.

Övergången till Campaign v8 tar hand om era befintliga Campaign Standarders externa konton: de är nu tillgängliga i klientkonsolen.

Läs mer om konfigurationen för [externt konto](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts){target="_blank"}.


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### Dynamiskt innehåll {#acs-gs-dyn-content}

Använd Campaign för att skapa dynamiskt innehåll och skicka personaliserade meddelanden. Personalization funktioner kan kombineras för att förbättra era budskap och skapa en anpassad användarupplevelse.

Med Campaign v8 som administratör kan du definiera dynamiska innehållsblock och hur de används för att anpassa innehållet i e-postleveransen i den här videon:

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

Länkar:

* [Kom igång med personalisering](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [Använd personaliseringsblock](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [Skapa villkorligt innehåll](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [Personalization-datakällor](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### Leveransmallar {#acs-gs-templates}

Att använda leveransmallar är ett krav i Campaign v8, som i Campaign Standard.

För en snabbare och förbättrad designprocess kan du skapa leveransmallar som enkelt återanvänder anpassat innehåll och anpassade inställningar för alla era kampanjer. Med den här funktionen kan ni standardisera den kreativa utseendet och känslan för att kunna genomföra och lansera kampanjer snabbare. Lär dig hur du skapar leveransmallar i [Webbanvändargränssnittet för kampanj](../../v8/msg/delivery-template.md). Se även hur du skapar leveransmallar i klientkonsolen i [det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/create-templates){target="_blank"}.

### Typologiregler {#acs-gs-admin-rules}

Som administratör ansvarar du för att skapa och underhålla typologiregler för leveranser. Precis som i Adobe Campaign Standard, i Campaign v8, är typologiregler affärsregler som gör att du kan kontrollera och filtrera meddelandet innan du skickar det.

När ni går över till Campaign v8 från en Campaign Standard-miljö flyttas era typologiregler till Campaign v8.

I Campaign v8 levereras typologiregler med en specifik Campaign Optimization ass-on. Med den här modulen kan du styra, filtrera och övervaka leveransen. För att undvika konflikter mellan kampanjer kan Adobe Campaign testa olika kombinationer genom att tillämpa särskilda begränsningsregler. Detta garanterar att de skickade meddelandena uppfyller kundernas behov och förväntningar och företagets kommunikationspolicy. Läs mer i [dokumentationen om typologiregler](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}.

### Karantänhantering {#acs-gs-admin-quarantine}

Alla karantänadresser och karantänregler har migrerats från er Campaign Standard-miljö till Campaign v8. Ingen specifik åtgärd krävs för karantänhantering.

Som administratör kan du bekanta dig med karantänhantering i Campaign v8 från [den här sidan](../../v8/audience/quarantine.md). Se även detaljerad dokumentation om karantänhantering i klientkonsolen i [det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"}.


## Hantera Adobe Campaign-integreringar {#acs-gs-integrations}

Ni kan koppla samman er Campaign-instans med Adobe Experience Cloud lösningar för att kombinera funktioner. Adobe Campaign har flera kopplingar som gör att du kan kommunicera med externa program, ansluta till databasmotorer, dela och synkronisera data. Lär dig hur du kombinerar dina lösningar i [den här dokumentationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/integration){target="_blank"}.

Som Campaign Standard-användare som migrerar till Campaign v8 gäller följande för dig:

* Om du använde dessa integreringar med Campaign Standard har konfigurationerna och data för **Adobe Analytics** och **Audience Manager** migrerats av Adobe.
* Om din e-postmiljö är integrerad med **Adobe Experience Manager** rekommenderar Adobe att du går över till **Adobe Experience Manager as a Cloud Service** så att du kan använda den här funktionen när du utformar e-postmeddelanden i webbgränssnittet för Campaign och underlättar en smidig hantering av e-postleveransinnehåll och -formulär direkt i din Adobe Experience Manager-Campaign Standard. Läs mer på [den här sidan](../../v8/integrations/aem-content.md).
Observera att Campaign också kan integreras med Adobe Experience Manager 6.5. Mer information om hur du konfigurerar den här integreringen finns i [den här dokumentationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}.
* Om din Campaign Standard-miljö är integrerad med **Utlösare** måste du konfigurera och konfigurera den här integreringen i Campaign v8 så som beskrivs i [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}.
* Om din Campaign Standard är integrerad med **Adobe Target** måste du konfigurera och konfigurera den här integreringen i Campaign v8 så som beskrivs i [den här sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}.

