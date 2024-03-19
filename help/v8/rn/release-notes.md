---
title: Senaste versionsinformation
description: Upptäck nya funktioner i gränssnittet för webbkampanjer
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Versionsinformation {#latest-release}

<!--Last update: **March 19, 2024**-->

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

>[!AVAILABILITY]
>
>Den här versionen är tillgänglig för alla användare som startar [Campaign (konsol) version 8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html). Läs mer om Adobe Campaign kundkonsoluppdateringar och uppgraderingar i [Kampanjdokumentation v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html){target="_blank"}.

## Marsrelease {#24-3-release}

**Releasedatum**: 19-20 mars 2024

### Direktreklam, kanal {#24-3-dm}

**Direktreklam** kanalen kan nu användas i arbetsflöden och som fristående leveranser. Direktreklam är en offlinekanal som gör att du kan skapa, anpassa och generera extraheringsfiler och dela dem med direktreklamleverantörer för att skicka e-post till kunderna.

![](../assets/do-not-localize/direct-mail.gif)

### Ny arbetsflödesaktivitet för Ändra datakälla {#24-3-change-data-source}

The **Ändra datakälla** målaktiviteter gör att du kan ändra datakällan som används i arbetsflödets arbetsregister. Den här aktiviteten ger större flexibilitet genom att du kan hantera data i olika databaser och förbättra prestandan.

![](../assets/do-not-localize/change-data-source.gif)

### Förbättring av delad arbetsflödesaktivitet {#24-3-split}

Nu kan du använda **Generera alla delmängder i samma tabell** i **Dela** arbetsflödesaktivitet för att gruppera alla delmängder i en enda utdataövergång.

### Frågemodelleraren {#24-3-query-modeler}

* Frågemodelleraren kan nu användas i e-postdesignern. Du kan skapa villkor när du skapar villkorsstyrt innehåll.
* Fördefinierade värden är nu tillgängliga för datumtypsattribut när du skapar ett anpassat villkor.
* Det går inte längre att lägga till operatorer för en ny övergång i diagrammet. De kan bara läggas till i en befintlig övergång innan komponenterna filtreras för att gruppera dem.
