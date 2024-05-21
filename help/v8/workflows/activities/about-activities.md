---
audience: end-user
title: Arbeta med arbetsflödesaktiviteter
description: Lär dig hur du arbetar med arbetsflödesaktiviteter
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---


# Om arbetsflödesaktiviteter {#workflow-activities}

Arbetsflödesaktiviteter grupperas i tre kategorier. Beroende på sammanhanget kan tillgängliga aktiviteter variera.

Alla aktiviteter beskrivs i avsnitten nedan:

* [Verksamheter som rör målinriktning och datahantering](#targeting)
* [Kanalaktiviteter](#channel)
* [Flödeskontroll](#flow-control)

![](../assets/workflow-activities.png)

## Verksamheter som riktar sig till {#targeting}

Dessa aktiviteter är specifika för målgruppsanpassning. Med dem kan du skapa ett eller flera mål genom att definiera en målgrupp och dela eller kombinera dessa målgrupper med hjälp av skärnings-, union- eller uteslutningsåtgärder.

* [Bygg målgrupper](build-audience.md): Definiera målpopulationen. Du kan antingen välja en befintlig målgrupp eller använda frågemodelleraren för att definiera en egen fråga.
* [Ändra datakälla](change-data-source.md): Ändra datakällan för arbetsflödets arbetstabell.&quot;
* [Ändra dimension](change-dimension.md): Ändra målinriktningsdimensionen när du skapar arbetsflödet.
* [Kombinera](combine.md): Utför segmentering på den inkommande populationen. Du kan använda en union, en skärning eller ett undantag.
* [Deduplicering](deduplication.md): Ta bort dubbletter i resultatet/resultaten av inkommande aktiviteter.
* [Berikning](enrichment.md): Definiera ytterligare data som ska bearbetas i arbetsflödet. Med den här aktiviteten kan du utnyttja den inkommande övergången och konfigurera aktiviteten för att slutföra utdataövergången med ytterligare data.
* [Inkrementell fråga](incremental-query.md): Fråga databasen på schemalagd basis. Varje gång den här aktiviteten körs utesluts resultaten från tidigare körningar. På så sätt kan du bara rikta in dig på nya element.
* [Avstämning](reconciliation.md): Definiera länken mellan data i Adobe Campaign-databasen och data i en arbetstabell, till exempel data som lästs in från en extern fil.
* [Spara målgrupper](save-audience.md): Uppdatera en befintlig målgrupp eller skapa en ny målgrupp från den population som beräknas uppströms i ett arbetsflöde.
* [Dela](split.md): Segmentera inkommande population i flera deluppsättningar.

## Datahanteringsaktiviteter {#data}

Dessa aktiviteter är specifika för att hantera och berika populationsdata.

* [Extrahera fil](extract-file.md): Exportera data från Adobe Campaign till ett annat system som en extern fil.
* [Läs in fil](load-file.md): Arbeta med profiler och data som lagras i en extern fil.
* [Överföringsfil](transfer-file.md): Ta emot eller skicka filer, testa om det finns filer eller lista med filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll.
* [JavaScript-kod](javascript-code.md): Kör ett JavaScript-kodfragment i ett arbetsflödes sammanhang.
* [Prenumerationstjänster](subscription-services.md): Prenumerera eller avbeställ flera profiler till/från en tjänst i en enda åtgärd.
* [Uppdatera data](update-data.md): Utför massuppdateringar på fält i databasen. Flera alternativ gör att du kan anpassa datauppdateringen.

## Kanalaktiviteter {#channel}

Med Adobe Campaign Web kan ni automatisera och genomföra marknadsföringskampanjer i flera kanaler. Du kan kombinera kanalaktiviteter på arbetsytan för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende. Följande **Kanal** aktiviteter är tillgängliga: E-post, SMS, Android och push-meddelanden från iOS. [Lär dig hur du ställer in en leverans i ett arbetsflöde](channels.md).

## Flödeskontroll {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Avsluta aktivitet"
>abstract="The **End** kan du grafiskt markera slutet av ett arbetsflöde. Denna aktivitet har ingen funktionell inverkan och är därför frivillig."

Följande aktiviteter är specifika för att organisera och köra arbetsflöden. Deras huvuduppgift är att samordna de övriga verksamheterna:

* [Och-join](and-join.md): Synkronisera flera körningsgrenar i ett arbetsflöde.
* **End**: Markera slutet av ett arbetsflöde grafiskt. Denna aktivitet har ingen funktionell inverkan och är därför valfri
* [Extern signal](external-signal.md): Utlös körningen av ett arbetsflöde från ett annat arbetsflöde eller ett API-anrop.
* [Gaffel](fork.md): Skapa utgående övergångar om du vill starta flera aktiviteter samtidigt.
* [Schemaläggare](scheduler.md): Schemalägg när arbetsflödet startas.
* [Testa](test.md): Aktivera övergångar baserat på angivna villkor.
* [Vänta](wait.md): Pausa körningen av en del av ett arbetsflöde tillfälligt.
