---
title: Tidiga versionsinformation om webbanvändargränssnittet i Campaign v8
description: Upptäck nya funktioner i nästa version av Campaign Web User Interface
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 1864f6c847e1720eb5e58a0572b110e7991fafb8
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 2%

---

# Tidig versionsinformation {#e-release}

Adobe Campaign webbanvändargränssnitt innehåller kontinuerligt nya funktioner, förbättringar av befintliga funktioner och felkorrigeringar. Alla ändringar konsolideras i slutet av varje månad i [versionsinformationen](release-notes.md).

**Noteringar om tidig version nedan kan ändras utan föregående meddelande till releasedatum**. Länkar, skärmar och uppdaterad dokumentation publiceras i [versionsinformationen](release-notes.md) på releasedatum.

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
<p>Nu kan du definiera externa leveranser och externa leveransmallar i webbgränssnittet för Campaign. I det här läget genereras meddelanden i en indatafil som kan delas med din externa leverantör. Läget Extern leverans är standardläge för direktpostkanalen.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Styra och filtrera leveransen med typografi</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skapa typologier och typologiregler i Adobe Campaign webbgränssnitt. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Typologier verifierar att dina leveranser alltid innehåller nödvändiga element (t.ex. en länk för att avbryta prenumerationen eller en ämnesrad), eller filtreringsregler som utesluter grupper från det avsedda målet (t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder).</p>
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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


