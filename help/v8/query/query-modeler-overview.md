---
audience: end-user
title: Arbeta med frågemodelleraren
description: Lär dig hur du arbetar med Adobe Campaign Web Query Modeler.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 66882fccf771cd6d3fa85f47d42b3ee53d1485f7
workflow-type: tm+mt
source-wordcount: '556'
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
| **Definiera målgrupper**: Ange den målgrupp du vill ha i dina meddelanden eller arbetsflöden och skapa enkelt nya målgrupper som är anpassade efter dina behov. [Lär dig skapa målgrupper](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Anpassa arbetsflödesaktiviteter**: Använd regler i arbetsflödesaktiviteter, som **Dela** och **Avstämning**, för att anpassa dem efter dina specifika krav. [Läs mer om arbetsflödesaktiviteter](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Fördefinierade filter**: Skapa fördefinierade filter som fungerar som genvägar under olika filtreringsåtgärder, oavsett om du arbetar med datalistor eller skapar en målgrupp för en leverans. [Lär dig arbeta med fördefinierade filter](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Filtret rapporterar data**: Lägg till regel för att filtrera data som visas i rapporter. [Lär dig arbeta med rapporter](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Anpassa listor**: Skapa anpassade regler för att filtrera data som visas i listor som mottagare, leveranslistor osv. [Lär dig filtrera listor](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Bygg villkorligt innehåll**: gör e-postinnehåll dynamiskt genom att skapa villkor som definierar vilket innehåll som ska visas för olika mottagare, vilket säkerställer personaliserade och relevanta meddelanden. [Lär dig hur du skapar villkorligt innehåll](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} |

## Gränssnitt för frågemodelleraren {#interface}

Frågemodelleraren innehåller en central arbetsyta där du skapar frågan och en höger ruta med information om frågan.

![](assets/query-interface.png){zoomable="yes"}

### Den centrala arbetsytan {#canvas}

Frågemodellerarens centrala arbetsyta är där du lägger till och kombinerar de olika komponenterna som skapar din fråga. [Lär dig skapa en fråga](build-query.md)

Verktygsfältet i det övre högra hörnet av arbetsytan innehåller alternativ för att enkelt ändra frågekomponenterna och navigera på arbetsytan:

* **Flera markeringslägen**: Markera flera filtreringskomponenter för att kopiera och klistra in dem där du vill.
* **Rotera**: Växla arbetsytan lodrätt.
* **Anpassa till skärmen**: Anpassa arbetsytans zoomnivå till skärmen.
* **Zooma ut** / **Zooma in**: Zooma ut eller in på arbetsytan.
* **Visningsschema**: Öppnar en ögonblicksbild av arbetsytan som visar att du finns.

### Rutan Regelegenskaper {#rule-properties}

Till höger visas information om frågan i rutan **[!UICONTROL Rule properties]**. Det gör att du kan utföra olika åtgärder för att kontrollera frågan och se till att den passar dina behov. Den här rutan visas när du skapar en fråga för att skapa en målgrupp. [Lär dig hur du kontrollerar och validerar din fråga](build-query.md#check-and-validate-your-query)
