---
audience: end-user
title: Arbeta med frågemodelleraren
description: Lär dig hur du arbetar med Adobe Campaign Web Query Modeler.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 4de9a8afea6a07971ebd23982a1a1ab98bc70045
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Arbeta med frågemodelleraren {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Ny frågemodellerare"
>abstract="Adobe Campaign Web har en frågemodellerare som förenklar filtreringen av databaser för att välja specifika mål baserat på olika kriterier. Detta inkluderar användning av avancerade uttryck och operatorer. Frågemodelleraren är tillgänglig i alla sammanhang där du behöver definiera regler för att filtrera data."

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Ny frågemodellerare"
>abstract="Adobe Campaign Web har en frågemodellerare som förenklar filtreringen av databaser för att välja specifika mål baserat på olika kriterier. Detta inkluderar användning av avancerade uttryck och operatorer. Frågemodelleraren är tillgänglig i alla sammanhang där du behöver definiera regler för att filtrera data."

<!--TO REMOVE ABOVE-->


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
| **Definiera målgrupper**: Ange den målgrupp du vill rikta in dig på i dina meddelanden eller arbetsflöden och skapa enkelt nya målgrupper som är anpassade efter dina behov. | ![](assets/access-audience.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Anpassa arbetsflödesaktiviteter**: tillämpa regler i arbetsflödesaktiviteter, som Dela och Avstämning, för att anpassa dem efter dina specifika krav. | ![](assets/access-workflow.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Fördefinierade filter**: Skapa fördefinierade filter som fungerar som genvägar under olika filtreringsåtgärder, oavsett om du arbetar med datalistor eller skapar en målgrupp för en leverans. | ![](assets/access-predefined-filter.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Filtrera rapportdata**: Lägg till regel för att filtrera data som visas i rapporter. | ![](assets/access-reports.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **Anpassa listor**: Skapa anpassade regler för att filtrera data som visas i listor som mottagare, leveranslistor osv. | ![](assets/access-lists.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |

<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png){zoomable="yes"}

 +++
-->

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
