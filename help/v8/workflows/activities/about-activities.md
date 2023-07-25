---
audience: end-user
title: Arbeta med arbetsflödesaktiviteter
description: Lär dig hur du arbetar med arbetsflödesaktiviteter
badge: label="Alfa"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 5%

---


# Om arbetsflödesaktiviteter {#workflow-activities}

Arbetsflödesaktiviteter grupperas i tre kategorier. Beroende på sammanhanget kan tillgängliga aktiviteter variera.

Alla aktiviteter beskrivs i avsnitten nedan:

* [Målinriktade aktiviteter](#targeting)
* [Kanalaktiviteter](#channel)
* [Flödeskontrollaktiviteter](#flow-control)

![](../assets/workflow-activities.png)

## Målinriktade aktiviteter {#targeting}

Dessa aktiviteter är specifika för målgruppsanpassning, ändring och berikning av populationsdata. Med dem kan du skapa ett eller flera mål genom att definiera en målgrupp och dela eller kombinera dessa målgrupper med hjälp av skärnings-, union- eller uteslutningsåtgärder.

* The [Bygg målgrupper](build-audience.md) kan du definiera målpopulationen. Du kan antingen välja en befintlig målgrupp eller använda regelbyggaren för att definiera en egen fråga.
* The [Kombinera](combine.md) kan segmentera den inkommande populationen. Du kan använda en union, en skärning eller ett undantag.
* The [Berikning](enrichment.md) kan du definiera ytterligare data som ska bearbetas i arbetsflödet. Med den här aktiviteten kan du utnyttja den inkommande övergången och konfigurera aktiviteten för att slutföra utdataövergången med ytterligare data.
* The [Dela](split.md) kan du segmentera inkommande population i flera deluppsättningar.

## Kanalaktiviteter {#channel}

Med Adobe Campaign Web kan ni automatisera och köra marknadsföringskampanjer i flera kanaler, som e-post, SMS eller push. Du kan kombinera kanalaktiviteter på arbetsytan för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende.

Följande **Kanal** aktiviteter är tillgängliga:

* E-post
* Push
* SMS

Se detta [section](enrichment.md).

## Flödeskontrollaktiviteter {#flow-control}

Följande aktiviteter är specifika för att organisera och köra arbetsflöden. Deras huvuduppgift är att samordna de övriga verksamheterna:

* The [Och-join](and-join.md) kan du synkronisera flera körningsgrenar i ett arbetsflöde.
* The **End** kan du grafiskt markera slutet av ett arbetsflöde. Denna aktivitet har ingen funktionell inverkan och är därför frivillig.
* The [Gaffel](fork.md) kan du skapa utgående övergångar och starta flera aktiviteter samtidigt.
* The [Vänta](wait.md) aktiviteten tillfälligt avbryter körningen av en del av ett arbetsflöde.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

