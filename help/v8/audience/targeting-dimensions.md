---
title: Måldimensioner
description: Läs mer om målinriktning av dimensioner på Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Måldimensioner {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Välj måldimension"
>abstract="Med målinriktningsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter osv. Som standard väljs målet i den inbyggda tabellen Mottagare för e-post och SMS. För push-meddelanden är standardmåldimensionen prenumerantprogram."

Målgruppsdimensionen, även kallad. målmappning, är den typ av data som hanteras av en åtgärd. Det gör att du kan definiera målpopulationen: profiler, kontraktsanställda, operatörer, prenumeranter osv.

## Målgruppsdimensioner för arbetsflöden {#workflow}

Måldimensionen för ett arbetsflöde definieras av den första **[!UICONTROL Build audience]**-aktiviteten och används för alla andra aktiviteter fram till arbetsflödets slut. Om du till exempel gör en fråga om profilerna från databasen, kommer den utgående övergången att innehålla data av typen &quot;mottagare&quot; och den kommer att överföras till nästa aktivitet.

Observera att du kan växla måldimensionen i ett arbetsflöde med en [Ändra dimensionsaktivitet](../workflows/activities/change-dimension.md). Detta gör att du till exempel kan ställa frågor till databasen i en viss tabell, som inköp eller prenumerationer, och sedan ändra måldimensionen till mottagare för att skicka leveranser till motsvarande profiler.

När du väljer en måldimension (i arbetsflödesinställningarna eller i aktiviteter som **Skapa målgrupp**, **Avstämning** eller **Ändra dimension**) visas ett urval av vanliga scheman som standard i listan. Om du vill visa alla tillgängliga scheman aktiverar du knappen **[!UICONTROL Show all schemas]**. Alternativvalet sparas för varje användare.

![](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Måldimensioner {#list}

Som standard har e-post- och SMS-leveransmallar målprofiler. Måldimensionen använder därför fälten i tabellen **nms:receive**. För push-meddelanden är standardmåldimensionen **Subscriber applications nms:appSubscriptionRcp** som är länkad till mottagartabellen.

Du kan även använda andra inbyggda målmappningar i dina arbetsflöden och leveranser som listas nedan:

| Namn | Använd för | Schema |
|---|---|---|
| Mottagare | Leverera till profiler/mottagare (inbyggt mottagarregister) | nms:mottagare |
| Besökare | Leverera till besökare vars profiler har samlats in via hänskjutning (viral marketing) för ex. | mns:besökare |
| Prenumerationer | Leverera till profiler som prenumererar på en informationstjänst som ett nyhetsbrev | nms:prenumeration |
| Prenumerationer på besökare | Skicka till besökare som prenumererar på en informationstjänst | nms:visitorSub |
| Operatorer | Leverera till Adobe Campaign | nms:operator |
| Extern fil | Leverera via en fil som innehåller all information som behövs för leveransen | Inget länkat schema, inget mål har angetts |
| Prenumerationsprogram | Leverera till profiler som prenumererar på ett program | nms:appSubscriptionRcp |

Dessutom kan du skapa en ny målmappning beroende på dina behov. Åtgärden utförs endast från klientkonsolen. Läs mer i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
