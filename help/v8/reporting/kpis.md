---
title: Viktiga prestandaindikatorer
description: Lär dig hur du förstår viktiga prestandaindikatorer
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# Viktiga prestandaindikatorer {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Viktiga resultatindikatorer"
>abstract="Med avsnittet **Nyckeltal för prestandaindikatorer** kan du kontrollera plattformens effektivitet med hjälp av gemensamma nyckeltal."

<!-- à enlever? -->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="Skräppost-KPI"

Bläddra till startsidan för att kontrollera viktiga prestandaindikatorer för din plattform. Dessa indikatorer visar antalet meddelanden som levereras, öppnas, klickas, prenumerationen avbryts och antalet fel anges.

Mätvärden beräknas som standard för leveranser som skickas under de senaste sju dagarna. Du kan ändra perioden från listrutan i kortets övre högra del. Meddelanden som skickas till testprofiler exkluderas.

Du kan välja vilken kanal som ska visas. Som standard återspeglar dessa indikatorer mätvärden för e-postkanalen.

![Skärmbild som visar KPI-kortet med mått för e-postkanalen.](assets/kpi.png){zoomable="yes"}

## Meddelandet har levererats {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Levererat"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla meddelanden som har bearbetats och hur många meddelanden som har levererats med framgång jämfört med det totala antalet meddelanden som skickats."

Antalet meddelanden som levereras återspeglar din leveransgrad. Det kan aldrig vara 100 % av följande orsaker: vissa adresser eller telefonnummer kan vara fel, skräppostblockerare hos e-postleverantörer kan avvisa dina meddelanden eller leveransproblem kan inträffa.

Indikatorn **Levererad** visar följande KPI:er för varje kanal:

* Procentandel av antalet meddelanden som levererats med lyckat resultat jämfört med det totala antalet skickade meddelanden.

* Summan av alla meddelanden som har bearbetats utan fel.

I Adobe Campaign är regeln för att markera ett meddelande som&quot;Levererat&quot;:

Antal meddelanden för vilka fältet &quot;dirigeringsadress&quot; är lika med &quot;Nej&quot; och med statusen &quot;Som tagits med i beräkningen av tjänsteleverantören&quot; (för SMS), &quot;Skickat&quot; (för e-post) eller &quot;Mottaget på mobilen&quot; (för push-meddelanden).

## Totalt antal öppningar {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Öppnar"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla öppnade meddelanden och hur många meddelanden som öppnats i procent jämfört med det totala antalet meddelanden som levererats med framgång."

Totalt antal öppningar beräknas genom att spåra det totala antalet gånger ett meddelande öppnas, oavsett hur många enskilda mottagare som genererar dessa öppningar. Den här indikatorn är bara tillgänglig för e-post.

Indikatorn **Öppnar** visar följande KPI:er för varje kanal:

* Procentandel av antalet meddelanden som öppnats jämfört med det totala antalet meddelanden som levererats utan fel.

* Summan av alla öppnade meddelanden, per kanal.

Adobe Campaign identifierar att ett meddelande öppnas när mottagaren hämtar bilderna i e-postmeddelandet. HTML och Multipart/Alternative emails innehåller en bild på 0 pixlar som gör att du kan identifiera meddelanden som har öppnats. Eftersom meddelanden i textformat inte innehåller några bilder går det inte att identifiera om de har öppnats. Värden som beräknas baserat på det meddelande som öppnas är alltid uppskattningar på grund av den felmarginal som är länkad till bildvisningen.

## Genomklickningsfrekvens {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Klickningar"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla URL:er som klickats i meddelanden och procentandelen klickningar jämfört med det totala antalet meddelanden som levererats utan fel."

Lägg till URL:er i meddelandeinnehållet för att dirigera om mottagarna till en viss sida. Klickfrekvensen mäter antalet och procentandelen mottagare som klickade på en länk i meddelandet.

Indikatorn **Click** visar följande KPI:er för varje kanal:

* Procentandel av antalet klick jämfört med det totala antalet meddelanden som levererats med framgång.

* Antal distinkta personer som klickat minst en gång i en leverans. Länkar och länkar till e-postspegelsidan tas inte med.

Dessa mått baseras på den konsoliderade spårningstabellen (`nms:trackingStats`). Den här aggregerade tabellen används av prestandaskäl när rapporter visas, i stället för loggtabellen för mottagarspårning (`nms:trackingLogRcp`). Den beräknas inte i realtid. Tabellen genereras några minuter efter att spårningsloggarna har hämtats.

## Prenumerationstaxor {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Prenumerationer"
>abstract="I det här måttet visas, för den valda kanalen, summan av alla prenumerationer på en tjänst och procentandelen prenumerationer jämfört med det totala antalet meddelanden som levererats med framgång."

Mottagarna kan välja att använda e-post och SMS.

Indikatorn **Prenumerationer** visar följande KPI:er för varje kanal:

* Procentandel av antalet prenumerationer jämfört med det totala antalet meddelanden som levererats med framgång.

>[!NOTE]
>
> KPI:er för prenumeration och avprenumeration varierar beroende på tjänsttyp. E-postprenumerationer och avbeställningar omfattar till exempel alla e-postrelaterade tjänster, oavsett om de är en följd av manuella åtgärder eller webbformulär. Det är viktigt att särskilja detta tillvägagångssätt från leveransnivåmätvärdet för att avsluta prenumerationen, som spårar länkklick som inte är faktiska avabonnerade användare.

## Avbryta prenumerationstaxor {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Avprenumerationer"
>abstract="I det här måttet visas, för den valda kanalen, summan av alla avbeställningar från en tjänst och procentandelen avbeställningar jämfört med det totala antalet meddelanden som levererats med framgång."

Mottagarna måste kunna avanmäla sig från e-post och SMS via en dedikerad avprenumerationslänk i e-postinnehållet eller genom att svara STOP på ett SMS.

Indikatorn **Avbeställning** visar följande KPI:er för varje kanal:

* Procentandel av antalet avbrutna prenumerationer jämfört med det totala antalet meddelanden som levererats utan framgång.

* Summan av alla klickningar på en länk för att avbryta prenumerationen, vilket innebär att URL-kategorin är lika med&quot;Avanmäl dig&quot;.

>[!NOTE]
>
> KPI:er för prenumeration och avprenumeration varierar beroende på tjänsttyp. E-postprenumerationer och avbeställningar omfattar till exempel alla e-postrelaterade tjänster, oavsett om de är en följd av manuella åtgärder eller webbformulär. Det är viktigt att särskilja detta tillvägagångssätt från leveransnivåmätvärdet för att avsluta prenumerationen, som spårar länkklick som inte är faktiska avabonnerade användare.

## Felfrekvenser {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Fel"
>abstract="Totalt antal fel som ackumulerats under leveranser och automatisk avhoppsbearbetning. Den associerade frekvensen är förhållandet till antalet meddelanden som ska levereras."

Vissa meddelanden som skickas från din Adobe Campaign-plattform når kanske inte sina mål. Det kan hända när användaradressen eller telefonen har stavfel, om mottagaren har ändrat sin e-postadress eller om postlådan är full. Om ett meddelande inte kan skickas till en profil skickar fjärrservern automatiskt ett felmeddelande till Adobe Campaign. Det här felet är kvalificerat för att avgöra om e-postadressen, telefonnumret eller enheten ska sättas i karantän.

Kontrollera och uppdatera databasen regelbundet och se till att alla profiler är aktiva och riktiga. Leveransfel kan vara tillfälliga eller permanenta - mjuka eller hårda studsar - beroende på varför meddelandet inte levererades.

Indikatorn **Fel** visar följande KPI:er för varje kanal:

* Procentandel av antalet fel jämfört med det totala antalet meddelanden som ska levereras.

* Totalt antal fel som ackumulerats under leveranser och automatisk återinläsning.

## Meddelandet har skickats {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Skickat"
>abstract="Detta mätresultat visar, för direktpostkanalen, summan av alla skickade meddelanden och procentandelen meddelanden som skickats till leverantören, jämfört med det totala antalet meddelanden som förberetts under leveransförberedelsefasen."

Under beredningsfasen genereras extraheringsfilen för direktreklam, men informationen om mottagare (leveransloggar) uppdateras inte. Status för en leverans ändras från Väntande leverans till Skickat när Campaign-användaren bekräftar att leveransen har skickats. Därefter anges leveransen till Slutförd.

Det kan aldrig vara 100 % av de meddelanden som skickas jämfört med det totala antalet meddelanden som skickas, eftersom vissa adresser kan saknas eller vara ofullständiga.

Indikatorn **Skickat** visar följande nyckeltal för direktpostkanalen:

* Procentandel av antalet skickade meddelanden jämfört med det totala antalet förberedda meddelanden.

* Summan av alla skickade meddelanden.