---
audience: end-user
title: Använd arbetsflödesaktiviteten för anrikning
description: Lär dig hur du använder arbetsflödesaktiviteten för anrikning
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---


# Berikning {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Anrikningsaktivitet"
>abstract="Med Enrichment-aktiviteten kan du förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter riktade aktiviteter.<br/>När berikningsdata har lagts till i arbetsflödet kan de användas i aktiviteter som lagts till efter Enrichment-aktiviteten för att segmentera kunder i olika grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får genklang hos målgruppen."

Med Enrichment-aktiviteten kan du förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter riktade aktiviteter.

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

