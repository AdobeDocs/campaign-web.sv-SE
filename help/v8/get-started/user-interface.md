---
audience: end-user
title: Upptäck gränssnittet
description: Adobe Campaign webbgränssnitt
hidefromtoc: true
hide: true
robots: noindex
googlebot: noindex
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 93525fd1900c3a667051720205219ae5f9884736
workflow-type: tm+mt
source-wordcount: '1524'
ht-degree: 2%

---

# Upptäck gränssnittet {#user-interface}

Adobe Campaign nya webbgränssnitt är ett modernt och intuitivt gränssnitt som förenklar utformningen och leveransen av marknadsföringskampanjer. Gränssnittet kan integreras med Adobe Experience Cloud program och lösningar.

Lär dig hur du ansluter till Adobe Campaign och utforskar Experience Cloud grundläggande navigering [i den här artikeln](connect-to-campaign.md).

>[!NOTE]
>
>Dokumentationen uppdateras ofta för att återspegla de senaste ändringarna i produktanvändargränssnittet. Vissa skärmbilder kan dock skilja sig något från användargränssnittet.

## Startsida för kampanj {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Senaste"
>abstract="Listan **Senaste** innehåller genvägar till nyligen skapade och ändrade leveranser. Den här listan visar deras kanal, status, ägare, datum för skapande och ändring."

På startsidan för Campaign kan du snabbt och enkelt bläddra bland viktiga resurser, indikatorer och komponenter.

I den övre delen av startsidan visas information om de senaste uppdateringarna och nya funktioner som finns i produkten, med länkar till versionsinformation och detaljerad dokumentation. Använd vänsterpilen för att bläddra igenom funktionskort.

![Skärmbild som visar hemsidan med funktionskort och navigeringsalternativ](assets/home.png){zoomable="yes"}

Med avsnittet **Nyckeltal för prestandaindikatorer** kan du kontrollera plattformens effektivitet med hjälp av gemensamma nyckeltal. Läs mer om dessa KPI:er på [den här sidan](../reporting/kpis.md).

Listan **Senaste** innehåller genvägar till nyligen skapade och ändrade leveranser. Den här listan visar deras kanal, status, ägare, skapandedatum och ändringsdatum. Klicka på länken **Visa mer** om du vill läsa in ytterligare leveranser.

Dessutom kan du få åtkomst till hjälpsidor för Adobe Campaign webbnyckel från avsnittet **Om** på sidan.

### Länken Om {#user-interface-about}

>[!CONTEXTUALHELP]
>id="acw_about"
>title="Om sida"
>abstract="På sidan Om finns information om din Adobe Campaign-instans."

>[!CONTEXTUALHELP]
>id="acw_about_instance"
>title="Om instans"
>abstract="Instansavsnittet innehåller viktig information om konsolklienten, inklusive både version och tillhörande build-nummer."

>[!CONTEXTUALHELP]
>id="acw_about_web"
>title="Om webben"
>abstract="I webbavsnittet visas versionen av användargränssnittet för Campaign-webben, med det senaste uppdateringsdatumet, om tillgängligt."

>[!CONTEXTUALHELP]
>id="acw_about_packages"
>title="Om installerade paket"
>abstract="I avsnittet Installerade paket visas alla moduler, funktioner och integreringar som finns på din instans."

Längst ned på sidan finns länken **[!UICONTROL About]** med information om din Adobe Campaign-instans. Dessa uppgifter är skrivskyddade.

![Skärmbild som visar länken Om längst ned på sidan](assets/about-link.png){zoomable="yes"}

Avsnittet **Instans** innehåller viktig information om konsolklienten, inklusive både **version** och det associerade **build**-numret.

* **version** refererar till den officiella versionen som du använder.
* **build** refererar till en specifik upprepning av den versionen.

Både version- och build-nummer är viktiga för felsökning eftersom de hjälper dig att avgöra vilka funktioner och korrigeringar som finns i din miljö.

I avsnittet **Webb** visas versionen av användargränssnittet för Campaign-webben, tillsammans med det senaste uppdateringsdatumet, om det är tillgängligt. Detta hjälper till att spåra ändringar eller förbättringar som gjorts i användargränssnittet för Campaign-webben.

Avsnittet **Installerade paket** innehåller alla moduler, funktioner och integreringar som finns i din instans. Dessa paket utökar funktionaliteten i Adobe Campaign och möjliggör specialiserade uppgifter som integrering med andra Adobe-lösningar eller stöd för specifika arbetsflöden. Med tanke på det stora antalet paket kan du söka i det här avsnittet för att snabbt kontrollera om en viss modul är installerad på din instans.

![Skärmbild som visar avsnittet Installerade paket med sökfunktioner](assets/about.png){zoomable="yes"}

## Navigeringsmeny till vänster {#user-interface-left-nav}

Bläddra bland länkarna till vänster för att få tillgång till Adobe Campaign webbfunktioner. Flera länkar visar listor med objekt som kan sorteras och filtreras. Du kan också konfigurera kolumner så att all information som du behöver visas. Se [avsnittet](#list-screens). Vissa listskärmar är skrivskyddade. Vilka alternativ som visas på den vänstra navigeringsmenyn och i listorna beror på dina användarbehörigheter. Läs mer om behörigheter i [det här avsnittet](permissions.md).

### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="Menyn **Utforskaren** visar alla Campaign-komponenter och -objekt med samma mapphierarki som den i klientkonsolen. Bläddra bland alla komponenter, mappar och scheman i Campaign v8, kontrollera tillhörande behörigheter och skapa mappar och undermappar på den här menyn."

Menyn **Utforskaren** visar alla Campaign-resurser och -objekt med samma mapphierarki som den i klientkonsolen. Bläddra bland alla komponenter, mappar och scheman i Campaign v8 och skapa leveranser, arbetsflöden och kampanjer.

Vilka objekt som visas i **Utforskaren** beror på dina användarbehörigheter. Du kan också lägga till mappar och undermappar om du har rätt behörighet. Läs mer om behörigheter i [det här avsnittet](permissions.md).

Du kan konfigurera kolumner för att anpassa visningen så att all information du behöver visas. Se [avsnittet](#list-screens). Du kan också lägga till mappar och undermappar, vilket beskrivs i [det här avsnittet](permissions.md#folders).

Mer information om Campaign-utforskaren, mapphierarkin och resurser finns i den här [Campaign v8-dokumentationen (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=sv-SE#ac-explorer-ui){target="_blank"}.

### Kampanjhantering {#user-interface-campaign-management}

I avsnittet **Kampanjhantering** har du tillgång till marknadsföringskampanjer, leveranser och arbetsflöden.

* **Kampanjer** - Det här är listan över era kampanjer och kampanjmallar. Som standard kan du för varje kampanj visa start-, slut-, skapings- och senaste ändringsdatum, aktuell status och namnet på den kampanjoperator som skapade kampanjen. Du kan filtrera listan efter status, start-/slutdatum, mapp eller skapa ett avancerat filter för att definiera egna filtervillkor. Läs mer om kampanjer [i det här avsnittet](../campaigns/gs-campaigns.md).

* **Leveranser** - Bläddra i listan över leveranser. Som standard kan du visa deras status, senaste ändringsdatum och nyckeltal för nyckeltal. Du kan filtrera listan efter status, kontaktdatum eller kanal. Klicka på en e-postleverans för att öppna instrumentpanelen och få en översikt över leveransinformationen. Leveranser i andra kanaler är skrivskyddade. Läs mer om leveranser [i det här avsnittet](../msg/gs-messages.md).

  Använd knappen **Fler åtgärder** för att ta bort eller duplicera en leverans.

  ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"} [Skärmbild som visar knappen Fler åtgärder med alternativ för att ta bort eller duplicera en leverans.]

* **Arbetsflöden** - På den här skärmen kan du komma åt den fullständiga listan över arbetsflöden och arbetsflödesmallar. Du kan kontrollera deras status, senaste/nästa körningsdatum och skapa ett nytt arbetsflöde eller en ny arbetsflödesmall. Du kan filtrera listan med samma villkor som för andra objekt. Dessutom kan du filtrera arbetsflöden som tillhör en kampanj eller inte. Läs mer om arbetsflöden [i det här avsnittet](../workflows/gs-workflows.md).

### Innehållshantering {#user-interface-content-management}

I avsnittet **Innehållshantering** kan du visa dina innehållsmallar och fragment.

* **Innehållsmallar** - För en snabbare och förbättrad designprocess kan du skapa fristående mallar för att enkelt återanvända anpassat innehåll i hela [!DNL Adobe Campaign]. Den här funktionen är endast tillgänglig för e-post och gör att innehållsorienterade användare kan arbeta med fristående mallar så att marknadsföringsanvändare kan återanvända och anpassa dem i sina egna e-postkampanjer. Läs mer i [det här avsnittet](../content/create-email-templates.md).

* **Fragment** - Ett fragment är en återanvändbar komponent som kan refereras till i en eller flera leveranser mellan kampanjer. När du ändrar ett fragment uppdateras allt innehåll som använder det. [Lär dig arbeta med fragment](../content/fragments.md).

Med den här funktionen kan ni skapa flera anpassade innehållsblock som marknadsföringsanvändare kan använda för att snabbt sammanställa e-postinnehåll i en förbättrad designprocess.

### Kundhantering {#user-interface-customer-management}

I avsnittet **Kundhantering** kan du visa dina profiler, målgrupper och prenumerationer. De här listorna är skrivskyddade.

* **Profiler** - Skapa och hantera profiler och få åtkomst till mottagardatabasen. Som standard kan du visa deras e-postadress, förnamn och efternamn. Läs mer om profiler i [det här avsnittet](../audience/about-recipients.md).
* **Publiker** - Det här är din lista över målgrupper. Som standard kan du visa deras typ, ursprung, skapande, senaste ändringsdatum och etikett. Du kan filtrera listan efter ursprung. Läs mer om målgrupper och listor i [det här avsnittet](../audience/about-recipients.md).
* **Prenumerationstjänster** - Bläddra bland dina prenumerationslistor. Som standard kan du visa deras typ, läge och etikett. Lär dig hur du hanterar prenumerationer och avbeställningar i [Adobe Campaign v8-dokumentationen (konsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=sv-SE){target="_blank"}.
* **Fördefinierade filter** - Fördefinierade filter är anpassade filter som skapas och sparas för framtida bruk. De kan användas som genvägar under alla filtreringsåtgärder med frågemodelleraren, t.ex. när en lista med data filtreras eller målgruppen för en leverans skapas. Läs mer i [det här avsnittet](predefined-filters.md).

### Beslutshantering {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Erbjudanden"
>abstract="Bläddra igenom listorna med erbjudanden och erbjudandemallar som har skapats i konsolen med modulen **Interaktion** . De här listorna är skrivskyddade."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=sv-SE" text="Lägg till erbjudanden till en leverans"

I avsnittet **Beslutshantering** kan du visa erbjudanden och erbjudandemallar. De här listorna är skrivskyddade.

* **Erbjudanden** - Bläddra igenom listan med erbjudanden och erbjudandemallar som har skapats i konsolen med modulen **Interaktion**. Som standard kan du visa deras status, start-/slutdatum och miljö. Du kan filtrera listan efter status och start-/slutdatum. Det finns även mallar för erbjudandet.

Lär dig hur du skapar och skickar erbjudanden i e-postmeddelanden och SMS i [det här avsnittet](../msg/offers.md).

### Rapportering {#left-nav-reporting}

* **Rapporter** - Posten **Rapport** innehåller en samlad sammanfattning av trafik- och interaktionsstatistik för varje kanal i Campaign-miljön. Rapporterna består av olika widgetar, som var och en har ett distinkt perspektiv på kampanjen eller leveransresultatet. Läs mer i [det här avsnittet](../reporting/global-reports.md).

### Administration {#left-nav-admin}

* **Granskningsspårning** - Posten **Granskningsspårning** ger användarna fullständig synlighet för alla ändringar som görs i viktiga entiteter i instansen, vanligtvis de som påverkar instansens smidiga funktion avsevärt. [Läs mer](../reporting/audit-trail.md).

* **Externa konton** - Skapa nya externa konton med webbanvändargränssnittet för att uppfylla dina specifika behov och säkerställa sömlösa dataöverföringar. [Läs mer](../administration/external-account.md).

* **Scheman** - Anpassade fält är ytterligare attribut som har lagts till i scheman som är klara att användas via Adobe Campaign-konsolen. [Läs mer](../administration/custom-fields.md).

<!--* **Delivery Alerting** - Delivery Alerting is an alert management system that enables groups of users to automatically receive email notifications with information on their delivery executions. [Learn more](../msg/delivery-alerting.md).-->

## Läs mer {#learn-more}

Lär dig hur du bläddrar bland, söker efter och filtrerar listor som är tillgängliga i Campaign-miljön [på den här sidan](list-filters.md).



<!--CONTEXTUAL HELP TO DISPATCH IN DOCS ONCE FEATURE LIVE-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_notification"
>title="Kontinuerlig leverans"
>abstract="Kontinuerlig leverans"
