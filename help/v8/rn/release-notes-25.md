---
title: Versionsinformation om webbanvändargränssnittet i Campaign v8
description: 2025 Campaign Web User Interface-versioner
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: ec994efb6f88b729fe2dc9d7ba118e9ada10be9a
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 9%

---

# Versionsinformation 2025 {#2025-release}

På den här sidan visas alla ändringar och förbättringar som är tillgängliga i **2025-utgåvor**. De senaste versionskommentarerna är tillgängliga på [den här sidan](release-notes.md).

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
<p>Nu kan du skapa typologier och typologiregler i Adobe Campaign webbgränssnitt. Med typologier kan ni styra, filtrera och prioritera utskick av leveranser. Typologier används för att validera att leveranser alltid innehåller obligatoriska komponenter (t.ex. en länk för att avbryta prenumerationen eller en ämnesrad) eller filtreringsregler som utesluter grupper från målgruppen (t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder).</p>
<img src="assets/do-not-localize/typology.gif">
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
<p>Nu kan du skapa målmappningar i Campaign Web User Interface. Målmappningar definierar hur olika leveranskanaler (e-post, SMS, push-meddelanden) länkar till datafälten i ett schema. Med målmappningen kan du definiera målgruppen: profiler, kontraktsanställda, operatorer, prenumeranter, potentiella kunder osv.</p>
<img src="assets/do-not-localize/target-mapping.gif">
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
<p>Nu kan du komma åt information om ett schema genom att markera dess namn i listan. Utgåvan av anpassade fält är nu tillgänglig från knappen <b>Redigera anpassade fält</b> som finns i schemainformationen.</p>
<img src="assets/do-not-localize/schemas.gif">
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
<img src="assets/do-not-localize/visual-fragment.gif">
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
<img src="assets/do-not-localize/external-delivery.gif">
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
<p>Nu kan du skapa uppräkningar direkt via Adobe Campaign webbanvändargränssnitt. En uppräkning är en lista med värden som föreslås av systemet för att fylla i fält. Använd uppräkningar för att standardisera värdena för dessa fält, hjälp med inmatning av data eller användning inom frågor.</p>
<img src="assets/do-not-localize/enumerations.gif">
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
<img src="assets/do-not-localize/options.gif">
<p>Mer information finns i den <a href="../administration/options.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Definiera och anropa Javascript-koder</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skapa JavaScript-koder i Adobe Campaign webbanvändargränssnitt. På så sätt kan du skapa återanvändbara funktioner som kan användas i olika arbetsflöden, ungefär som i ett bibliotek.</p>
<img src="assets/do-not-localize/javascript.gif">
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
<img src="assets/do-not-localize/ai-lp.gif">
<p>Mer information om AI Assistant finns i <a href="../email/generative-lp.md">detaljerad dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>


### Förbättringar {#25-1-improvements}

* Anpassa visningen av anpassade fält i gränssnittet:

   * Nu kan du välja ytterligare anpassade fält som ska visas i gränssnittet
   * Du kan nu ange regler för hur anpassade fält av länktyp ska visas, t.ex. att begränsa listvärden baserat på indata från ett annat fält
   * Nu kan du ordna fälten i gränssnittet på ett flexiblare sätt: fälten kan spänna över en enda kolumn eller grupperas i underavsnitt för bättre sortering
   * Du kan nu ange specifika fält som skrivskyddade

* Senaste filter och favoritfilter: Om du snabbt vill återanvända attribut som används ofta kan du nu lägga till dem i favoriter. Detta gör att de är lättillgängliga för framtida uppgifter. Förutom favoriter kan du även visa och använda de senast markerade attributen.

* Externa konton: Den nya typen **[!UICONTROL Routing]** är tillgänglig för val när du skapar ett nytt externt konto. Med det kan du konfigurera ett specifikt externt konto för användning i externa leveranser. [Läs mer](../administration/external-account.md#routing)
