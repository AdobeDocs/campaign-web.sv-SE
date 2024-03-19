---
audience: end-user
title: Arbeta med frågemodelleraren
description: Lär dig hur du arbetar med Adobe Campaign Web Query Modeler.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Arbeta med frågemodelleraren {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Ny frågemodellerare"
>abstract="Adobe Campaign Web har en frågemodellerare som förenklar filtreringen av databaser för att välja specifika mål baserat på olika kriterier. Detta inkluderar användning av avancerade uttryck och operatorer. Frågemodelleraren är tillgänglig i alla sammanhang där du behöver definiera regler för att filtrera data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Frågemodelleraren"
>abstract="Definiera filtreringskriterier för mottagare eller andra måldimensioner från databasen. Utnyttja er målgrupp på Adobe Experience Platform för att ytterligare förfina er målgrupp och maximera effekten av er kampanj."

Adobe Campaign webbgränssnitt har en frågemodellerare som förenklar processen att filtrera databasen baserat på olika kriterier. Det garanterar full kompatibilitet med frågor som skapas i klientkonsolen, vilket underlättar en smidig övergång till webbanvändargränssnittet.

Dessutom kan frågemodelleraren hantera mycket komplexa och långa frågor effektivt, vilket ger större flexibilitet och precision. Dessutom har den stöd för fördefinierade filter under förhållanden, vilket gör att du enkelt kan förfina dina frågor samtidigt som du använder avancerade uttryck och operatorer för omfattande målgruppsanpassning och segmenteringsstrategier.

## Åtkomst till frågemodelleraren

Frågemodelleraren är tillgänglig i alla sammanhang där du behöver definiera regler för att filtrera data.

| Användning | Exempel |
|  ---  |  ---  |
| **Definiera målgrupper**: Ange den målgrupp du vill rikta in dig på i dina meddelanden eller arbetsflöden och skapa enkelt nya målgrupper som är anpassade efter dina behov. [Lär er hur ni bygger målgrupper](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Anpassa arbetsflödesaktiviteter**: tillämpa regler i arbetsflödesaktiviteter, som **Dela** och **Avstämning**, för att passa in dina specifika krav. [Läs mer om arbetsflödesaktiviteter](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Fördefinierade filter**: Skapa fördefinierade filter som fungerar som genvägar under olika filtreringsåtgärder, oavsett om du arbetar med datalistor eller skapar en målgrupp för en leverans. [Lär dig hur du arbetar med fördefinierade filter](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Filtrera rapportdata**: Lägg till regel för att filtrera data som visas i rapporter. [Lär dig arbeta med rapporter](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Anpassa listor**: Skapa anpassade regler för att filtrera data som visas i listor som mottagare, leveranslistor osv. [Lär dig filtrera listor](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Skapa villkorsstyrt innehåll**: gör e-postinnehåll dynamiskt genom att skapa villkor som definierar vilket innehåll som ska visas för olika mottagare, vilket säkerställer personaliserade och relevanta meddelanden. [Lär dig hur du skapar villkorsstyrt innehåll](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} |

## Gränssnitt för frågemodelleraren {#interface}

Frågemodelleraren innehåller en central arbetsyta där du skapar frågan och en höger ruta med information om frågan.

![](assets/query-interface.png){zoomable=&quot;yes&quot;}

### Den centrala arbetsytan {#canvas}

Frågemodellerarens centrala arbetsyta är där du lägger till och kombinerar de olika komponenterna som skapar din fråga. [Lär dig hur du skapar en fråga](build-query.md)

Verktygsfältet i det övre högra hörnet av arbetsytan innehåller alternativ för att enkelt ändra frågekomponenterna och navigera på arbetsytan:

* **Flervalsläge**: Välj flera filterkomponenter som ska kopieras och klistras in på valfri plats.
* **Rotera**: Växla arbetsytan lodrätt.
* **Anpassa till skärm**: Anpassa arbetsytans zoomnivå till skärmen.
* **Zooma ut** / **Zooma in**: Zooma ut eller in på arbetsytan.
* **Visa karta**: Öppnar en ögonblicksbild av arbetsytan som visar att du befinner dig.

### Rutan Regelegenskaper {#rule-properties}

På höger sida, **[!UICONTROL Rule properties]** innehåller information om frågan. Det gör att du kan utföra olika åtgärder för att kontrollera frågan och se till att den passar dina behov. [Lär dig hur du kontrollerar och validerar din fråga](build-query.md#check-and-validate-your-query)
