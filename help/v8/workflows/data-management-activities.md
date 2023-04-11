---
audience: end-user
title: Arbeta med arbetsflöden för datahanteringsaktiviteter
description: Lär dig använda datahanteringsaktiviteter i Adobe Campaign webbarbetsflöden
badge: label="Alpha" type="Positive"
source-git-commit: ee418ea42bc4568f2ff1f0fe9080825764fee65d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Datahanteringsaktiviteter {#data-management}

översikt: vad de används för vilket användningsfall du kan använda dem

visa tillgängliga aktiviteter + kort beskrivning + ref to section

## Berikning {#enrichment}

beskrivning: lägga till en eller flera anrikningsdata, kan utnyttja för att personalisera leveranser med hjälp av följande exempel: hämta det senaste köpet eller den senaste digitala prenumerationen och det totala beloppet för ett köp och anpassa ett e-postmeddelande med det

processexempel: hämta fyra senaste köp som är mindre än 100$ och anpassa ett e-postmeddelande med det
1. lägg till aktivitet
1. välj attribut att använda som anrikningsdata

   + visa avancerade fält, alternativ
   + knappen i

   Obs! attribut från måldimensionen

1. Välj hur data samlas in
1. antal poster som ska hämtas om du vill hämta en samling med flera poster
1. Använda filter och skapa regel

   + markera ett befintligt filter
   + spara filtret för återanvändning
   + visa resultatet av filtret visuellt eller i kodvyn

1. sortera poster med ett attribut

utnyttja anrikningsdata i kampanjen

där vi kan använda anrikningsdata: personalisera e-post, andra användningsfall?
