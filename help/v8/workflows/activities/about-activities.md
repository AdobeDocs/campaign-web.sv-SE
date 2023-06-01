---
audience: end-user
title: Arbeta med arbetsflödesaktiviteter
description: Lär dig hur du arbetar med arbetsflödesaktiviteter
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c842829915784654b7130563d36dea188e84ff3d
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 4%

---


# Om arbetsflödesaktiviteter {#workflow-activities}

Arbetsflödesaktiviteter grupperas i tre kategorier. Beroende på sammanhanget kan tillgängliga aktiviteter variera.

Alla aktiviteter beskrivs i avsnitten nedan:

* [Målinriktade aktiviteter](#targeting)
* [Kanalaktiviteter](#channel)
* [Flödeskontrollaktiviteter](#flow-control)

![](../assets/wokflow-activities.png)

## Målinriktade aktiviteter {#targeting}

Dessa aktiviteter är specifika för målgruppsanpassning, ändring och berikning av populationsdata. Med dem kan du skapa ett eller flera mål genom att definiera en målgrupp och dela eller kombinera dessa målgrupper med hjälp av skärnings-, union- eller uteslutningsåtgärder.

* The [Bygg målgrupper](build-audience.md) kan du definiera målpopulationen. Du kan antingen välja en befintlig målgrupp eller använda regelbyggaren för att definiera en egen fråga.
* The [Kombinera](combine.md) kan segmentera den inkommande populationen. Du kan använda en union, en skärning eller ett undantag.
* The [Berikning](enrichment.md) kan du definiera ytterligare data som ska bearbetas i arbetsflödet. Med den här aktiviteten kan du utnyttja den inkommande övergången och konfigurera aktiviteten för att slutföra utdataövergången med ytterligare data.

## Kanalaktiviteter {#channel}

Med Adobe Campaign Web kan ni automatisera och köra marknadsföringskampanjer i flera kanaler, som e-post, SMS eller push. Med Adobe Campaign arbetsflöden kan du kombinera kanalaktiviteter på arbetsytan för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende.

Du kan till exempel skapa en välkomstkampanj för e-post som innehåller en serie meddelanden i olika kanaler, som e-post, SMS och push. Du kan också skicka ett uppföljningsmeddelande via e-post när en kund har slutfört ett köp eller skicka ett personligt födelsedagsmeddelande till en kund via SMS.

Genom att använda kanalaktiviteter kan ni skapa omfattande, personaliserade kampanjer som engagerar kunder över flera kontaktytor och driver konverteringar.

* [E-post](email.md)
* [Push](push.md)
* [SMS](sms.md)

## Flödeskontrollaktiviteter {#flow-control}

Följande aktiviteter är specifika för att organisera och köra arbetsflöden. Deras huvuduppgift är att samordna de övriga verksamheterna:

* The [Och-join](and-join.md) kan du synkronisera flera körningsgrenar i ett arbetsflöde.
* The [End](end.md) kan du grafiskt markera slutet av ett arbetsflöde. Denna verksamhet har ingen funktionell inverkan och är därför frivillig.
* The [Gaffel](fork.md) kan du skapa utgående övergångar och starta flera aktiviteter samtidigt.
* The [Vänta](wait.md) aktiviteten tillfälligt avbryter körningen av en del av ett arbetsflöde.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

