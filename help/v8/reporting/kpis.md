---
title: Viktiga prestandaindikatorer
description: Lär dig hur du förstår viktiga prestandaindikatorer
badge: label="Beta"
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: 41d426b97dc836f60f21e80ce149ce93aec77d69
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Viktiga prestandaindikatorer {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Viktiga resultatindikatorer"
>abstract="The **Viktiga resultatindikatorer** kan du kontrollera plattformens effektivitet med hjälp av gemensamma nyckeltal."

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="Skräppost-KPI"

Bläddra till startsidan för att kontrollera viktiga prestandaindikatorer för din plattform. Indikatorerna visar antalet meddelanden som levereras, öppnas, klickas, tas bort från prenumerationen och antalet fel.

Mätvärden beräknas som standard för leveranser som skickats under de senaste 7 dagarna. Du kan ändra perioden från listrutan i kortets övre högra del. Meddelanden som skickas till testprofiler exkluderas.

Du kan välja vilken kanal som ska visas. Som standard återspeglar dessa indikatorer mätvärden för e-postkanalen.

![](assets/kpi.png)

## Meddelandet har levererats {#ui-delivered-kpi}

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


## Totalt antal öppningar {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Öppnar"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla meddelanden som öppnats och hur många meddelanden som öppnats i procent jämfört med det totala antalet meddelanden som levererats med framgång."

Totalt antal öppningar beräknas genom att spåra det totala antalet gånger ett meddelande öppnas, oavsett hur många enskilda mottagare som öppnas av. Den här indikatorn är bara tillgänglig för e-post.

The **Öppnar** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet meddelanden som öppnats jämfört med det totala antalet meddelanden som levererats med lyckat resultat.

* Summan av alla öppnade meddelanden, per kanal.

Adobe Campaign identifierar att ett meddelande öppnas när mottagaren hämtar bilderna i e-postmeddelandet. HTML och Multipart/Alternative emails innehåller en bild på 0 pixlar som gör att du kan identifiera meddelanden som har öppnats. Eftersom meddelanden i textformat inte innehåller några bilder går det inte att se om de har öppnats eller inte. Värden som beräknas baserat på det meddelande som öppnas är alltid uppskattningar på grund av den felmarginal som är länkad till bildvisningen.



## Genomklickningsfrekvens {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Klickningar"
>abstract="Det här måttet visar, för den valda kanalen, summan av alla URL-adresser som klickats i meddelanden och procentandelen klickningar jämfört med det totala antalet meddelanden som levererats utan fel."

Du kan lägga till URL:er i meddelandeinnehållet, som dirigerar om mottagarna till en viss sida. Klickfrekvensen mäter antalet och procentandelen mottagare som klickade på en länk i meddelandet.

The **Klickningar** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet klick jämfört med det totala antalet meddelanden som levererats med framgång.

* Antal distinkta personer som klickat minst en gång i en leverans. Länkar som inte längre används och länkar till e-postspegelsidan tas inte med.

Dessa mått baseras på den konsoliderade spårningstabellen (`nms:trackingStats`). Den här sammanställningstabellen används av prestandaskäl när rapporter visas, i stället för i loggtabellen för mottagarspårning (`nms:trackingLogRcp`) och beräknas inte i realtid. Tabellen genereras några minuter efter att spårningsloggarna har hämtats.


## Avbryta prenumerationstaxor {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Avprenumerationer"
>abstract="I det här måttet visas, för den valda kanalen, summan av alla avbeställningar från en tjänst och procentandelen avbeställningar jämfört med det totala antalet meddelanden som levererats med framgång."

Mottagarna måste kunna avanmäla sig från e-post och SMS via en dedikerad avprenumerationslänk i e-postinnehållet eller genom att svara STOP på ett SMS.

The **Avbeställ** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet avbrutna prenumerationer jämfört med det totala antalet meddelanden som levererats utan framgång.

* Summan av alla klick på en länk för att avbryta prenumerationen, dvs. där en URL-kategori är lika med &quot;Avanmäl dig&quot;.


## Felfrekvenser {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Fel"
>abstract="Totalt antal fel som ackumulerats under leveranser och automatisk avhoppsbearbetning. Den associerade frekvensen är förhållandet till antalet meddelanden som ska levereras."

Vissa meddelanden som skickas från din Adobe Campaign-plattform når kanske inte sina mål. Det kan hända när användaradressen eller telefonen har stavfel, om mottagaren har ändrat e-postadressen eller om postlådan är full. Om ett meddelande inte kan skickas till en profil skickar fjärrservern automatiskt ett felmeddelande till Adobe Campaign. Det här felet är kvalificerat för att avgöra om e-postadressen, telefonnumret eller enheten ska sättas i karantän.

Därför bör du alltid kontrollera och uppdatera databasen och se till att alla profiler är aktiva och riktiga. Leveransfel kan vara tillfälliga eller permanenta - mjuka eller hårda studsar - beroende på varför meddelandet inte levererades.

The **Fel** Indikatorn visar följande KPI:er för varje kanal:

* Procentandel av antalet fel jämfört med det totala antalet meddelanden som ska levereras.

* Totalt antal fel som ackumulerats under leveranser och automatisk återinläsning.
