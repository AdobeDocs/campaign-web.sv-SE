---
audience: end-user
title: Arbeta med frågemodelleraren
description: Lär dig hur du arbetar med Adobe Campaign Web Query Modeler.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '693'
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

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="Förfina mål"
>abstract="Dessa regler kan bara ändras i klientkonsolen."

Adobe Campaign webbgränssnitt har en frågemodellerare som förenklar processen att filtrera databasen baserat på olika kriterier. Det garanterar full kompatibilitet med frågor som skapas i klientkonsolen, vilket underlättar en smidig övergång till webbanvändargränssnittet.

Dessutom hanterar frågemodelleraren mycket komplexa och långa frågor effektivt, vilket ger större flexibilitet och precision. Programmet har också stöd för fördefinierade filter under förhållanden, vilket gör det enkelt för användarna att förfina frågor samtidigt som avancerade uttryck och operatorer används för omfattande målgruppsanpassning och segmenteringsstrategier.

## Åtkomst till frågemodelleraren

Frågemodelleraren är tillgänglig i alla sammanhang där du behöver definiera regler för att filtrera data.

| Användning | Exempel |
|  ---  |  ---  |
| **Definiera målgrupper**: Ange den målgrupp du vill ha i dina meddelanden eller arbetsflöden och skapa enkelt nya målgrupper som är anpassade efter dina behov. [Lär dig skapa målgrupper](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild som visar hur du kommer åt gränssnittet för målgruppsskapande] |
| **Anpassa arbetsflödesaktiviteter**: Använd regler i arbetsflödesaktiviteter, som **Dela** och **Avstämning**, för att anpassa dem efter dina specifika krav. [Läs mer om arbetsflödesaktiviteter](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild som visar hur du får åtkomst till alternativ för anpassning av arbetsflöden] |
| **Fördefinierade filter**: Skapa fördefinierade filter som fungerar som genvägar under olika filtreringsåtgärder, oavsett om du arbetar med datalistor eller skapar en målgrupp för en leverans. [Lär dig arbeta med fördefinierade filter](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild som visar hur du får åtkomst till fördefinierade filter] |
| **Filtret rapporterar data**: Lägg till regler för att filtrera de data som visas i rapporter. [Lär dig arbeta med rapporter](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild som visar hur du filtrerar data i rapporter ] |
| **Anpassa listor**: Skapa anpassade regler för att filtrera data som visas i listor som mottagare eller leveranslistor. [Lär dig filtrera listor](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild som visar hur du anpassar listfilter] |
| **Bygg villkorligt innehåll**: Gör e-postinnehåll dynamiskt genom att skapa villkor som definierar vilket innehåll som ska visas för olika mottagare, vilket säkerställer personaliserade och relevanta meddelanden. [Lär dig hur du skapar villkorligt innehåll](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} [Bild som visar hur du skapar villkorligt innehåll] |

>[!NOTE]
>
>När du får åtkomst till ett objekt som skapats i klientkonsolen där regler har tillämpats, t.ex. en målgrupp eller ett fördefinierat filter, kan **[!UICONTROL Refine target]**-avsnittet visas. Detta innebär att ytterligare parametrar har konfigurerats för att förfina regelmålet. De här parametrarna kan bara ändras i konsolen.
>
>![Bilden visar en varning om förfiningsmål](assets/target-warning.png){zoomable="yes"}

## Gränssnitt för frågemodelleraren {#interface}

Frågemodelleraren innehåller en central arbetsyta där du skapar frågan och en höger ruta med information om frågan.

>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="Ny användarupplevelse"
>abstract="Använd den här växeln för att växla mellan den klassiska frågemodelleraren och den nya regelgenereringsupplevelsen."

![Bild som visar frågemodelleringsgränssnittet](assets/query-interface.png){zoomable="yes"}

### Den centrala arbetsytan {#canvas}

Frågemodellerarens centrala arbetsyta är den plats där du lägger till och kombinerar de olika komponenterna för att skapa din fråga. [Lär dig skapa en fråga](build-query.md)

Verktygsfältet i det övre högra hörnet av arbetsytan innehåller alternativ för att enkelt ändra frågekomponenterna och navigera på arbetsytan:

* **Flera markeringslägen**: Markera flera filtreringskomponenter för att kopiera och klistra in dem där du vill.
* **Rotera**: Växla arbetsytan lodrätt.
* **Anpassa till skärmen**: Anpassa arbetsytans zoomnivå till skärmen.
* **Zooma ut** / **Zooma in**: Zooma ut eller in på arbetsytan.
* **Visningsschema**: Öppna en ögonblicksbild av arbetsytan som visar din aktuella plats.

### Rutan Regelegenskaper {#rule-properties}

Till höger visas information om frågan i rutan **[!UICONTROL Rule properties]**. Det gör att du kan utföra olika åtgärder för att kontrollera frågan och se till att den passar dina behov. Den här rutan visas när du skapar en fråga för att skapa en målgrupp. [Lär dig hur du kontrollerar och validerar din fråga](build-query.md#check-and-validate-your-query)