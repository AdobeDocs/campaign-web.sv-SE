---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 36d2b7a67ef087d628151199a223ceee54f84180
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 9%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

Ändringar och förbättringar som är tillgängliga med tidigare versioner visas på sidorna [2024](release-notes-24.md) och [2025](release-notes-25.md) .

## 26 januari {#26-1-release}

_27 januari 2026_

### Nya funktioner {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Flerspråkiga leveransfunktioner (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Funktionen för flerspråkig leverans är nu tillgänglig för alla kunder (GA). Med den här funktionen kan du skicka flera meddelanden på olika språk i Adobe Campaign webbanvändargränssnitt. Du kan välja standardspråk för leveransen samt de olika språk som leveransen kan skickas på. Du kan även förhandsgranska leveransen på de språk du har valt. 
<p>Mer information finns i den <a href="../msg/multilingual.md">detaljerade dokumentationen</a>.</p>
<p>Följande förbättringar har gjorts i flerspråkiga push-meddelanden:</p>
<ul>
<li>Nu kan du snabbt fylla i alla språkvarianter genom att överföra en CSV-fil med ditt flerspråkiga innehåll. <a href="../msg/multilingual.md#csv-upload">Läs mer</a>
</li>
<li>Stöd för push-meddelanden.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Profilberikning i transaktionsmeddelanden (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Profilberikning i funktionen för transaktionsmeddelanden är nu tillgängligt för alla kunder (GA). Förutom e-post stöds nu även SMS- och push-meddelanden. Med den här funktionen kan du anpassa transaktionsmeddelanden genom att länka Adobe Campaign-databasfält till meddelandeinnehållet. Du kan välja målmappningar, berikningskolumner och en avstämningsnyckel för att säkerställa korrekt personalisering i realtid samtidigt som prestandatrösklar bibehålls.</p>
<p>Mer information finns i den <a href="../transactional-messaging/profile-enrichment.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager live- och språkversioner</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Tack vare integreringen av Adobe Experience Manager-innehåll får ni tillgång till alla språk- och Live-kopior som skapats i Adobe Experience Manager direkt i Campaign när ni bygger leveranser. Du kan uppdatera innehåll i realtid för att hämta de senaste Adobe Experience Manager-versionerna. Integreringen eliminerar manuell innehållssynkronisering mellan Adobe Experience Manager och Campaign och effektiviserar arbetsflödet för flerspråkiga kampanjer.</p>
<p>Mer information finns i den <a href="../integrations/aem-multilingual.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Innehållsexperiment - A/B-tester</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Med hjälp av innehållsexperiment på Adobe Campaign Web kan du definiera flera olika leveransvarianter för A/B-tester för att mäta vilka som fungerar bäst för målgruppen. Du kan variera leveransinnehåll, ämne eller avsändare för att testa olika versioner och avgöra vilken variant som ger bäst resultat. Du kan utföra A/B-tester på olika e-postelement som ämnesrad, avsändarnamn och e-postinnehåll.</p>
<p>Mer information finns i den <a href="../email/ab-testing.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Kontinuerlig leveransaktivitet</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Med aktiviteten Kontinuerlig leverans kan du lägga till nya mottagare till en befintlig leverans. Med den här leveranstypen slipper du skapa en ny leverans varje gång, vilket gör den mer effektiv för meddelanden med låg volym eller meddelanden som skickas efter behov. En kontinuerlig leverans skapar en enda leveransinstans. Alla leveransloggar (broadLog) och spårningsloggar refererar till denna enda leverans, vilket förenklar övervakning och rapportering.</p>
<p>Mer information finns i den <a href="../workflows/activities/continuous-delivery.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Hantering av kampanjgodkännande</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Godkännandeprocessen hjälper till att samordna flera intressenter och säkerställer kvalitetskontroll innan leveranser skickas. Använd godkännanden när organisationen kräver validering från olika team, till exempel marknadschefer som granskar innehåll eller dataanalytiker som validerar målgrupper.</p>
<p>Mer information finns i den <a href="../campaigns/campaign-approvals.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

### Förbättringar {#26-1-improvements}

* Dynamisk rapportering har nu stöd för push-meddelanden och SMS. [Läs mer](../reporting/dynamic-reporting/get-started-reporting.md)
* Fördefinierade filter - Med ett nytt&quot;delat filter&quot;-alternativ kan du göra ett fördefinierat filter tillgängligt för andra användare i organisationen. [Läs mer](../get-started/predefined-filters.md#share-filter)
* Anpassningsfält som har skapats i Adobe Experience Manager, t.ex. Namn, E-post, Datum och Adress, ingår nu och är tillgängliga när du använder innehållsmallen.
* Utvärderingen av innehållskvaliteten kontrollerar nu om det finns läsbarhet, enhetlighet och effektivitet oberoende av varumärkesriktlinjerna, vilket identifierar otydliga meddelanden, inkonsekventa toner eller strukturella luckor. [Läs mer](../content/brands-score.md)
