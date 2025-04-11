---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 8%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web-gränssnittsreleaser fungerar enligt en kontinuerlig leveransmodell, vilket möjliggör en skalbar, stegvis lösning för driftsättning av funktioner. Versionsinformationen uppdateras därför flera gånger i månaden. Kontrollera dem regelbundet.

Ändringar och förbättringar som är tillgängliga i tidigare versioner visas [på den här sidan](release-notes-24.md).

## 25 februari {#25-2-release}

**Releasedatum**: 18 feb 2025

Följande funktioner och förbättringar är tillgängliga från och med februari.

### Funktioner {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Skapa affärsregler (typologiregler)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skapa typologier och typologiregler i Adobe Campaign webbgränssnitt. Typologier styr, filtrerar och prioriterar sändning av leveranser. Typologier validerar att leveranser alltid innehåller obligatoriska komponenter (till exempel en länk för att avbryta prenumerationen eller en ämnesrad) eller filtreringsregler som utesluter grupper från målgruppen (till exempel prenumeranter, konkurrenter eller icke-lojalitetskunder).</p>
<img src="assets/do-not-localize/typology.gif" alt="Illustration av typologiregler i Adobe Campaign webbgränssnitt">
<p>Mer information finns i den <a href="../administration/typologies.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Målmappningar</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skapa målmappningar i Campaign Web User Interface. Målmappningar definierar hur olika leveranskanaler (e-post, SMS, push-meddelanden) länkar till datafälten i ett schema. Målmappningen definierar målgruppen: profiler, kontraktsanställda, operatörer, prenumeranter, potentiella kunder och andra.</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="Illustration of target mappings creation in Adobe Campaign Web User Interface">
<p>Mer information finns i den <a href="../administration/target-mappings.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Schemainformation</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du komma åt information om ett schema genom att markera dess namn i listan. Redigering av anpassade fält är nu tillgängligt från knappen <b>Redigera anpassade fält</b> som finns i schemainformationen.</p>
<img src="assets/do-not-localize/schemas.gif" alt="Illustration of schema details and custom fields editing in Adobe Campaign Web User Interface">
<p>Mer information finns i den <a href="../administration/schemas.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

## 25 januari {#25-1-release}

**Releasedatum**: 5 feb 2025

Följande funktioner och förbättringar är tillgängliga från och med januari.

### Funktioner {#25-1-features}

<table>
<thead>
<tr>
<th><strong>Skapa och använda visuella fragment</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Visuella fragment är fördefinierade visuella block som du kan återanvända i flera e-postleveranser eller i innehållsmallar. Den här funktionen är nu tillgänglig för alla kunder som kör serverbygget 8.6.4 och senare.</p>
<img src="assets/do-not-localize/visual-fragment.gif" alt="Illustration av hur man skapar och använder fragment i Adobe Campaign webbgränssnitt">
<p>Mer information finns i den <a href="../content/use-visual-fragments.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Använd ett tredjepartssystem för att skicka leveranser</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du definiera externa leveranser och externa leveransmallar i webbgränssnittet för Campaign. I det här läget kompileras meddelanden till en utdatafil som kan delas med din externa leverantör. Som standard används det externa leveransläget för direktmeddelandekanalen.</p>
<img src="assets/do-not-localize/external-delivery.gif" alt="Illustration av externa leveransinställningar i Adobe Campaign webbgränssnitt">
<p>Mer information finns i den <a href="../msg/send-external-deliveries.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Hantera dina uppräkningar</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skapa uppräkningar direkt via Adobe Campaign webbanvändargränssnitt. En uppräkning är en lista med värden som föreslås av systemet för att fylla i fält. Använd uppräkningar för att standardisera värdena i dessa fält, bistå med datainmatning eller använd inom frågor.</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Illustration av uppräkningshantering i Adobe Campaign webbgränssnitt">
<p>Mer information finns i den <a href="../administration/enumerations.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Skapa anpassade alternativ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du använda de tekniska funktionerna i Adobe Campaign webbgränssnitt och skapa egna anpassade alternativ som passar dina behov. Detta är särskilt användbart när du arbetar med arbetsflödesaktiviteter i JavaScript för att lagra mellanliggande data.</p>
<img src="assets/do-not-localize/options.gif" alt="Illustration of custom options creation in Adobe Campaign Web User Interface">
<p>Mer information finns i den <a href="../administration/options.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Definiera och anropa JavaScript-koder</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skapa JavaScript-koder i Adobe Campaign webbanvändargränssnitt. På så sätt kan du skapa återanvändbara funktioner som kan användas i olika arbetsflöden, ungefär som i ett bibliotek.</p>
<img src="assets/do-not-localize/javascript.gif" alt="Illustration av JavaScript-kod i Adobe Campaign webbgränssnitt">
<p>Mer information finns i den <a href="../administration/javascript-codes.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Skapa landningssidor med AI Assistant</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>AI Assistant finns nu för leverans av landningssidor, vilket gör att du kan generera text, bilder eller hela sidlayouter.</p>
<img src="assets/do-not-localize/ai-lp.gif" alt="Illustration av hur AI Assistant används för att generera landningssidor i Adobe Campaign webbanvändargränssnitt">
<p>Mer information om AI Assistant finns i <a href="../email/generative-lp.md">detaljerad dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Förbättringar {#25-1-improvements}

* Anpassa visningen av anpassade fält i gränssnittet:
   * Välj ytterligare anpassade fält som ska visas i gränssnittet.
   * Ange regler för visning av anpassade fält av länktyp, t.ex. begränsningar av listvärden som baseras på indata från ett annat fält.
   * Ordna fälten i gränssnittet på ett flexiblare sätt: fälten kan spänna över en enda kolumn eller grupperas i underavsnitt för bättre sortering.
   * Ange specifika fält som skrivskyddade.

* Filtren Senaste och Favoriter: Lägg till attribut som används ofta till favoriter för snabb åtkomst. Förutom favoriter kan du visa och använda de senast valda attributen.

* Externa konton: Den nya typen **[!UICONTROL Routing]** är tillgänglig för val när du skapar ett nytt externt konto. Med det kan du konfigurera ett specifikt externt konto för användning i externa leveranser. [Läs mer](../administration/external-account.md#routing).