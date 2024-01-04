---
title: Måldimensioner
description: Läs mer om målinriktning av dimensioner på Adobe Campaign Web
badge: label="Begränsad tillgänglighet"
source-git-commit: 9fd523a04ac4bfb2d760202b1f7e9bd9e7097dfe
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 1%

---

# Måldimensioner {#targeting-dimensions}

Målgruppsdimensionen, även kallad. målmappning, är den typ av data som hanteras av en åtgärd. Det gör att du kan definiera målpopulationen: profiler, kontraktsanställda, operatörer, prenumeranter osv.

Måldimensionen för ett arbetsflöde definieras av den första **[!UICONTROL Build audience]** aktiviteten och används för alla andra aktiviteter fram till arbetsflödets slut. Om du till exempel gör en fråga om profilerna från databasen, kommer den utgående övergången att innehålla data av typen &quot;mottagare&quot; och den kommer att överföras till nästa aktivitet.

Observera att du kan byta måldimension i ett arbetsflöde med en [Ändra dimensionsaktivitet](../workflows/activities/change-dimension.md). Detta gör att du till exempel kan ställa frågor till databasen i en viss tabell, som inköp eller prenumerationer, och sedan ändra måldimensionen till mottagare för att skicka leveranser till motsvarande profiler.

Som standard har e-post- och SMS-leveransmallar målprofiler. Måldimensionen använder därför fälten i **nms:mottagare** tabell. Standardmåldimensionen för push-meddelanden är **Prenumerationsprogram nms:appSubscriptionRcp**, som är länkad till mottagartabellen.

Du kan även använda andra inbyggda målmappningar i dina arbetsflöden och leveranser som listas nedan:

| Namn | Använd för | Schema |
|---|---|---|
| Mottagare | Leverera till mottagare (inbyggd mottagartabell) | nms:mottagare |
| Besökare | Leverera till besökare vars profiler har samlats in via hänskjutning (viral marketing) för ex. | mns:besökare |
| Prenumerationer | Leverera till mottagare som prenumererar på en informationstjänst som ett nyhetsbrev | nms:prenumeration |
| Prenumerationer på besökare | Skicka till besökare som prenumererar på en informationstjänst | nms:visitorSub |
| Operatorer | Leverera till Adobe Campaign | nms:operator |
| Extern fil | Leverera via en fil som innehåller all information som behövs för leveransen | Inget länkat schema, inget mål har angetts |
| Prenumerationsprogram | Leverera till mottagare som prenumererar på ett program | nms:appSubscriptionRcp |

Dessutom kan du skapa en ny målmappning beroende på dina behov. Detta görs från klientkonsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
