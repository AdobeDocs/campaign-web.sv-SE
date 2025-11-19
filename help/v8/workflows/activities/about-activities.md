---
audience: end-user
title: Arbeta med arbetsflödesaktiviteter
description: Lär dig hur du arbetar med arbetsflödesaktiviteter
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Om arbetsflödesaktiviteter {#workflow-activities}

Arbetsflödesaktiviteter grupperas i tre kategorier. Beroende på sammanhanget kan tillgängliga aktiviteter variera.

Alla aktiviteter beskrivs i avsnitten nedan:

* [Verksamheter som rör målinriktning och datahantering](#targeting)
* [Kanalaktiviteter](#channel)
* [Flödeskontrollaktiviteter](#flow-control)

![Översikt över arbetsflödesaktiviteter](../assets/workflow-activities.png)

## Aktiviteter för målgruppsanpassning {#targeting}

Dessa aktiviteter är specifika för målgruppsanpassning. Med dem kan ni skapa en eller flera målgrupper genom att definiera en målgrupp och dela eller kombinera dessa målgrupper med hjälp av skärnings-, union- eller uteslutningsåtgärder.

* [Skapa målgrupp](build-audience.md): Definiera målpopulationen. Välj en befintlig målgrupp eller använd frågemodelleraren för att definiera en egen fråga.
* [Ändra datakälla](change-data-source.md): Ändra datakällan för arbetsflödets arbetsflödestabell.
* [Ändra dimension](change-dimension.md): Ändra måldimensionen när du skapar arbetsflödet.
* [Kombinera](combine.md): Utför segmentering på den inkommande populationen. Använd en union, en skärning eller ett undantag.
* [Deduplicering](deduplication.md): Ta bort dubbletter i resultatet av inkommande aktiviteter.
* [Berikning](enrichment.md): Definiera ytterligare data som ska bearbetas i arbetsflödet. Konfigurera aktiviteten för att slutföra utdataövergången med ytterligare data.
* [Inkrementell fråga](incremental-query.md): Fråga databasen på schemalagd basis. Varje gång den här aktiviteten körs utesluter den resultat från tidigare körningar och riktar sig endast till nya element.
* [Avstämning](reconciliation.md): Definiera länken mellan data i Adobe Campaign-databasen och data i en arbetstabell, till exempel data som lästs in från en extern fil.
* [Spara målgrupp](save-audience.md): Uppdatera en befintlig målgrupp eller skapa en ny målgrupp från den population som beräknas uppströms i ett arbetsflöde.
* [Dela](split.md): Segmentera den inkommande populationen i flera deluppsättningar.

## Datahanteringsaktiviteter {#data}

Dessa aktiviteter är specifika för att hantera och berika populationsdata.

* [Extrahera fil](extract-file.md): Exportera data från Adobe Campaign till ett annat system som en extern fil.
* [Läs in fil](load-file.md): Arbeta med profiler och data som lagras i en extern fil.
* [Överför fil](transfer-file.md): Ta emot eller skicka filer, testa om det finns filer eller lista med filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll.
* [JavaScript-kod](javascript-code.md): Kör ett JavaScript-kodfragment inom ett arbetsflödes kontext.
* [Prenumerationstjänster](subscription-services.md): Prenumerera eller avsluta prenumeration på flera profiler till eller från en tjänst i en enda åtgärd.
* [Uppdatera data](update-data.md): Utför massuppdateringar för fält i databasen. Flera alternativ gör att du kan anpassa datauppdateringen.

## Kanalaktiviteter {#channel}

Med Adobe Campaign Web kan ni automatisera och genomföra marknadsföringskampanjer i flera kanaler. Kombinera kanalaktiviteter på arbetsytan för att skapa flerkanaliga arbetsflöden som triggar åtgärder baserat på kundbeteende. Följande **kanalaktiviteter** är tillgängliga: e-post, SMS, Android och iOS push-meddelanden. [Lär dig hur du ställer in en leverans i ett arbetsflödes kontext](channels.md).

## Flödeskontrollaktiviteter {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Avsluta aktivitet"
>abstract="Med aktiviteten **End** kan du grafiskt markera slutet av ett arbetsflöde. Denna aktivitet har ingen funktionell inverkan och är därför frivillig."

Följande aktiviteter är specifika för att organisera och köra arbetsflöden. Deras huvuduppgift är att samordna de övriga verksamheterna:

* [And-join](and-join.md): Synkronisera flera körningsgrenar i ett arbetsflöde.
* **Slut**: Markera grafiskt slutet av ett arbetsflöde. Denna aktivitet har ingen funktionell inverkan och är därför frivillig.
* [Extern signal](external-signal.md): Utlös körningen av ett arbetsflöde från ett annat arbetsflöde eller ett API-anrop.
* [Förgrening](fork.md): Skapa utgående övergångar för att starta flera aktiviteter samtidigt.
* [Schemaläggare](scheduler.md): Schemalägg när arbetsflödet startar.
* [Test](test.md): Aktivera övergångar baserat på angivna villkor.
* [Vänta](wait.md): Pausa körningen av en del av ett arbetsflöde tillfälligt.