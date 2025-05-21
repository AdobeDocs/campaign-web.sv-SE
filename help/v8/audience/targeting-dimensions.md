---
title: Måldimensioner
description: Läs mer om målinriktning av dimensioner på Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Måldimensioner {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Välj måldimension"
>abstract="Med målgruppsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter och mycket annat. Som standard väljs målet i den inbyggda tabellen Mottagare för e-post och SMS. För push-meddelanden är standardmåldimensionen prenumerantprogram."

Måldimensionen, som också kallas målmappning, är den typ av data som en åtgärd hanterar. Den definierar målgruppen, t.ex. profiler, kontraktsanställda, operatörer eller prenumeranter.

## Målgruppsdimensioner för arbetsflöden {#workflow}

Måldimensionen för ett arbetsflöde definieras av den första **[!UICONTROL Build audience]**-aktiviteten och används för alla efterföljande aktiviteter fram till arbetsflödets slut. När du till exempel frågar profiler från databasen innehåller den utgående övergången data av typen &quot;mottagare&quot;, som överförs till nästa aktivitet.

Byt måldimension i ett arbetsflöde med en [Ändra dimensionsaktivitet](../workflows/activities/change-dimension.md). Detta gör att du kan fråga databasen i en viss tabell, t.ex. köp eller prenumerationer, och sedan ändra måldimensionen till mottagare för att skicka leveranser till motsvarande profiler.

När du väljer en måldimension (i arbetsflödesinställningarna eller i aktiviteter som **Skapa målgrupp**, **Avstämning** eller **Ändra dimension**) visas en lista med vanliga scheman som standard. Om du vill visa alla tillgängliga scheman växlar du till knappen **[!UICONTROL Show all schemas]**. Alternativvalet sparas för varje användare.

![Skärmbild som visar gränssnittet för måldimensionen med knappen Visa alla scheman aktiverad.](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Måldimensioner {#list}

Som standard har e-post- och SMS-leveransmallar målprofiler. Måldimensionen använder fälten i tabellen **nms:mottagare**. För push-meddelanden är standardmåldimensionen **Subscriber applications nms:appSubscriptionRcp** som är länkad till mottagartabellen.

Använd andra inbyggda målmappningar i arbetsflöden och leveranser enligt nedan:

| Namn | Använd för att leverera | Schema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Mottagare | Profiler/mottagare (inbyggd mottagartabell) | nms:mottagare |
| Besökare | Besökare vars profiler samlades in via hänskjutning (viral marketing for ex) | mns:besökare |
| Prenumerationer | Profiler som prenumererar på en informationstjänst som ett nyhetsbrev | nms:prenumeration |
| Prenumerationer på besökare | Besökare som prenumererar på en informationstjänst | nms:visitorSub |
| Operatorer | Adobe Campaign operatorer | nms:operator |
| Extern fil | Leverans via en fil som innehåller all nödvändig information | Inget länkat schema, inget mål har angetts |
| Prenumerationsprogram | Profiler som prenumererar på ett program | nms:appSubscriptionRcp |

Skapa dessutom nya målmappningar baserat på specifika behov. Utför endast den här åtgärden från klientkonsolen. Läs mer i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=sv-SE#new-mapping){target="_blank"}.