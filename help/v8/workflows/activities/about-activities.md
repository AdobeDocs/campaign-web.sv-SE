---
audience: end-user
title: Arbeta med arbetsflödesaktiviteter
description: Lär dig hur du arbetar med arbetsflödesaktiviteter
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# Om arbetsflödesaktiviteter {#workflow-activities}

Arbetsflödesaktiviteter grupperas i tre kategorier. Beroende på sammanhanget kan tillgängliga aktiviteter variera.

Alla aktiviteter beskrivs i avsnitten nedan:

* [Verksamheter som rör målinriktning och datahantering](#targeting)
* [Kanalaktiviteter](#channel)
* [Flödeskontroll](#flow-control)

![](../assets/workflow-activities.png)

## Verksamheter som rör målinriktning och datahantering {#targeting}

Dessa aktiviteter är specifika för målgruppsanpassning, ändring och berikning av populationsdata. Med dem kan du skapa ett eller flera mål genom att definiera en målgrupp och dela eller kombinera dessa målgrupper med hjälp av skärnings-, union- eller uteslutningsåtgärder.

* Använd [Spara målgrupper](save-audience.md) aktivitet för att uppdatera en befintlig målgrupp eller skapa en ny målgrupp från den population som beräknas uppströms i ett arbetsflöde.
* Använd [Bygg målgrupper](build-audience.md) för att definiera målpopulationen. Du kan antingen välja en befintlig målgrupp eller använda frågemodelleraren för att definiera en egen fråga.
* Använd [Kombinera](combine.md) för att segmentera den inkommande populationen. Du kan använda en union, en skärning eller ett undantag.
* Använd [Dela](split.md) aktivitet för att segmentera inkommande population i flera delmängder.
* Använd [Avstämning](reconciliation.md) -aktivitet för att definiera länken mellan data i Adobe Campaign-databasen och data i en arbetstabell, till exempel data som lästs in från en extern fil.
* Använd [Berikning](enrichment.md) -aktivitet för att definiera ytterligare data som ska bearbetas i arbetsflödet. Med den här aktiviteten kan du utnyttja den inkommande övergången och konfigurera aktiviteten för att slutföra utdataövergången med ytterligare data.
* Använd [Deduplicering](deduplication.md) aktivitet för att ta bort dubbletter i resultat av inkommande aktiviteter.
* Använd [Ändra dimension](change-dimension.md) för att ändra målinriktningsdimensionen när du skapar arbetsflödet.
* Använd [Läs in fil](load-file.md) -aktivitet för att arbeta med profiler och data som lagras i en extern fil.

## Kanalaktiviteter {#channel}

Med Adobe Campaign Web kan ni automatisera och genomföra marknadsföringskampanjer i flera kanaler. Du kan kombinera kanalaktiviteter på arbetsytan för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende. Följande **Kanal** aktiviteter är tillgängliga: E-post, SMS, Android och push-meddelanden från iOS. [Lär dig hur du ställer in en leverans i ett arbetsflöde](channels.md).

## Flödeskontroll {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Avsluta aktivitet"
>abstract="The **End** kan du grafiskt markera slutet av ett arbetsflöde. Denna aktivitet har ingen funktionell inverkan och är därför frivillig."

Följande aktiviteter är specifika för att organisera och köra arbetsflöden. Deras huvuduppgift är att samordna de övriga verksamheterna:

* Använd [Schemaläggare](scheduler.md) aktivitet som ska schemaläggas när arbetsflödet startas.
* Använd [Och-join](and-join.md) för att synkronisera flera körningsgrenar i ett arbetsflöde.
* Lägg till en **End** om du vill att slutet av ett arbetsflöde ska markeras grafiskt. Denna aktivitet har ingen funktionell inverkan och är därför frivillig.
* Använd [Gaffel](fork.md) aktivitet för att skapa utgående övergångar för att starta flera aktiviteter samtidigt.
* Lägg till en [Vänta](wait.md) för att tillfälligt pausa körningen av en del av ett arbetsflöde.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

