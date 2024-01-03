---
title: Arbeta med mottagare och målgrupper
description: Lär dig hur du arbetar med mottagare och målgrupper på Campaign Web
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Arbeta med mottagare och målgrupper {#about-recipients}

## Mottagare och målgrupper {#about}

I Adobe Campaign är målgruppen en leverans en målgrupp. En målgrupp är en uppsättning personer som har liknande beteenden och/eller egenskaper. Den här samlingen personer kan antingen genereras, markeras eller läsas in [enligt nedan](#audiences).

I de flesta fall består publiken av profiler som lagras som [mottagare](#recipients) i Adobe Campaign. Du kan även arbeta med andra målmappningar genom att ändra dimensionen enligt beskrivningen [i det här avsnittet](#targeting-dimensions).

## Måldimensioner {#targeting-dimensions}

Målgruppsdimensionen, även kallad. målmappning, är den typ av data som hanteras av en åtgärd. Det gör att du kan definiera målpopulationen: mottagare, avtalspliktiga mottagare, operatörer, prenumeranter osv.

Måldimensionen för ett arbetsflöde definieras av den första **[!UICONTROL Build audience]** aktiviteten och används för alla andra aktiviteter fram till arbetsflödets slut. Om du till exempel gör en fråga till mottagarna från databasen, kommer den utgående övergången att innehålla data av typen mottagare och den kommer att överföras till nästa aktivitet.

Observera att du kan byta måldimension i ett arbetsflöde med en [Ändra dimensionsaktivitet](../workflows/activities/change-dimension.md). Detta gör att du till exempel kan ställa frågor till databasen i en viss tabell, som inköp eller prenumerationer, och sedan ändra måldimensionen till mottagare för att skicka leveranser till motsvarande mottagare.

Som standard har mallar för e-post och SMS-leverans som mål **[!UICONTROL Recipients]**. Måldimensionen använder därför fälten i **nms:mottagare** tabell. Standardmåldimensionen för push-meddelanden är **Prenumerationsprogram nms:appSubscriptionRcp**, som är länkad till mottagartabellen.

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
