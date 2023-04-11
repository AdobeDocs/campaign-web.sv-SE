---
audience: end-user
title: Arbeta med arbetsflöden för datahanteringsaktiviteter
description: Lär dig använda datahanteringsaktiviteter i Adobe Campaign webbarbetsflöden
badge: label="Alpha" type="Positive"
source-git-commit: 5efcdf2da104b86bf3ee37ee7162495c2d99fb48
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Datahanteringsaktiviteter {#data-management}

översikt: vad de används för vilket användningsfall du kan använda dem

visa tillgängliga aktiviteter + kort beskrivning + ref to section

## Berikning {#enrichment}

Aktiviteten Enrichment används ofta i ett arbetsflöde efter riktade aktiviteter. Det gör att du kan förbättra måldata med ytterligare information från databasen.

Anrikningsdata kan komma antingen:

* **Från samma arbetsregister** som den som är inriktad på ditt arbetsflöde:

   *Ange en grupp kunder som målgrupp och lägg till fältet&quot;Födelsedatum&quot; i den aktuella arbetstabellen*

* **Från en annan arbetstabell**:

   *Ange kunder som målgrupp och lägg till fälten&quot;Belopp&quot; och&quot;Typ av produkt&quot; som kommer från tabellen&quot;Inköp&quot;*.

När berikningsdata har lagts till i arbetsflödet kan de sedan användas i aktiviteter som lagts till efter Enrichment-aktiviteten för att segmentera kunder i olika grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får genklang hos målgruppen.

Du kan till exempel lägga till information om kundernas inköp i arbetsflödets arbetsregister och använda dessa data för att anpassa e-postmeddelanden med deras senaste köp eller hur mycket som spenderas på dessa inköp.

Så här lägger du till en fördjupningsaktivitet i arbetsflödet:

1. lägg till aktivitet
1. välj attribut att använda som anrikningsdata

   visa avancerat fält, alternativ i

   Obs! attribut från måldimensionen

1. Välj hur data samlas in
1. antal poster som ska hämtas om du vill hämta en samling med flera poster
1. Använda filter och skapa regel

   markera ett befintligt filter och spara filtret för att återanvända resultatet av filtret visuellt eller i kodvyn

1. sortera poster med ett attribut

utnyttja anrikningsdata i kampanjen

där vi kan använda anrikningsdata: personalisera e-post, andra användningsfall?
