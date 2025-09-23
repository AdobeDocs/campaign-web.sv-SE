---
title: Målinriktning och filtrering
description: Läs mer om målgruppsanpassning och filtrering i Adobe Campaign webbgränssnitt
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Målinriktning och filtrering {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Välj måldimension"
>abstract="Med målgruppsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter och mycket annat. Som standard väljs målet i den inbyggda tabellen Mottagare för e-post och SMS. För push-meddelanden är standardmåldimensionen prenumerantprogram."

Måldimensionen, som också kallas målmappning, är den typ av data som en åtgärd hanterar. Den definierar målgruppen, t.ex. profiler, kontraktsanställda, operatörer eller prenumeranter. Filtreringsdimensionen gör att du kan tillämpa filter på målpopulationen genom att referera till relaterade kriterier utan att ändra huvudmåldimensionen.

## Måldimensioner {#targeting}

Måldimensionen för ett arbetsflöde definieras av den första **[!UICONTROL Build audience]**-aktiviteten och används för alla efterföljande aktiviteter fram till arbetsflödets slut. När du till exempel frågar profiler från databasen innehåller den utgående övergången data av typen &quot;mottagare&quot;, som överförs till nästa aktivitet.

Byt måldimension i ett arbetsflöde med en [Ändra dimensionsaktivitet](../workflows/activities/change-dimension.md). Detta gör att du kan fråga databasen i en viss tabell, t.ex. köp eller prenumerationer, och sedan ändra måldimensionen till mottagare för att skicka leveranser till motsvarande profiler.

När du väljer en måldimension (i arbetsflödesinställningarna eller i aktiviteter som **Skapa målgrupp**, **Avstämning** eller **Ändra dimension**) visas en lista med vanliga scheman som standard. Om du vill visa alla tillgängliga scheman växlar du till knappen **[!UICONTROL Show all schemas]**. Alternativvalet sparas för varje användare.

![Skärmbild som visar gränssnittet för måldimensionen med knappen Visa alla scheman aktiverad.](assets/targeting-dimension-show-all.png){zoomable="yes"}

Som standard har e-post- och SMS-leveransmallar målprofiler. Måldimensionen använder fälten i tabellen **nms:recipient**. För push-meddelanden är standardmåldimensionen **Prenumerantprogramnamn:appSubscriptionRcp**, som är länkat till mottagartabellen.

Använd andra inbyggda målmappningar i arbetsflöden och leveranser enligt nedan:

| Namn | Använd för att leverera | Schema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Mottagare | Profiler/mottagare (inbyggd mottagartabell) | nms:recipient |
| Besökare | Besökare vars profiler samlades in via hänskjutning (viral marketing for ex) | mns:visitor |
| Prenumerationer | Profiler som prenumererar på en informationstjänst som ett nyhetsbrev | nms:subscription |
| Prenumerationer på besökare | Besökare som prenumererar på en informationstjänst | nms:visitorSub |
| Operatorer | Adobe Campaign operatorer | nms:operator |
| Extern fil | Leverans via en fil som innehåller all nödvändig information | Inget länkat schema, inget mål har angetts |
| Prenumerationsprogram | Profiler som prenumererar på ett program | nms:appSubscriptionRcp |

Skapa dessutom nya målmappningar baserat på specifika behov. Utför endast den här åtgärden från klientkonsolen. Läs mer i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=sv-SE#new-mapping){target="_blank"}.

## Filtrera dimensioner {#filtering}

Med målinriktningsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter osv. Filtreringsdimensionen gör att du kan tillämpa filter på den här populationen genom att referera till relaterade data utan att ändra huvudmåldimensionen. Du kan t.ex. välja populationen baserat på specifika kriterier som avtalsägare eller nyhetsbrevprenumeranter.

Filtreringsdimensioner är bara tillgängliga i aktiviteten **Skapa publik**.

Om du vill välja kunder som har haft en livförsäkring i över 5 år väljer du följande:

* Måldimension: **Klienter**
* Filtreringsdimension: **Kontraktsinnehavare**.

Du kan sedan definiera filtreringsvillkoren i aktiviteten **Skapa publik**. Se den här [sidan](../workflows/activities/build-audience.md).

Vid dimensionsurval visas endast kompatibla filterdimensioner i gränssnittet. Dessa två dimensioner måste vara relaterade, så innehållet i filtreringsdimensionslistan beror på vilken måldimension som valts i det första fältet.
