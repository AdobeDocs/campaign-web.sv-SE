---
audience: end-user
title: Skapa en engångspublik för en leverans
description: Lär dig hur du skapar en engångspublik för en leverans.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Skapa en engångspublik {#one-time}

I det här avsnittet beskrivs hur du skapar en målgrupp när du skapar en ny leverans. I det här fallet används de profiler som ska inkluderas i leveransgruppen för att fråga databasen med frågemodelleraren. Den slutliga målgruppen används bara en gång för den här leveransen. Den sparas inte i målgruppslistan.

När du definierar huvudmålet för en leverans kan du också:
* [Välj en befintlig målgrupp](add-audience.md) i listan **[!UICONTROL Audiences]**.
* [Läs in en målgrupp från en extern fil](file-audience.md) (endast för e-post).

Så här skapar du en ny målgrupp för en leverans:

1. Klicka på knappen **[!UICONTROL Select audience]** i sektionen **Målgrupp** i leveransassistenten.

   ![](assets/segment-builder0.png){zoomable="yes"}

1. Välj **Skapa en egen** för att öppna frågemodelleraren, som gör att du kan definiera målpopulationen genom att filtrera data från databasen. [Lär dig använda frågemodelleraren](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable="yes"}

1. När frågan är klar klickar du på **Bekräfta** för att använda den slutliga målgruppen som huvudmål för leveransen.

   Ni kan också ställa in en kontrollgrupp för att mäta effekten av era kampanjer. Kontrollgruppen tar inte emot meddelandet. På så sätt kan du jämföra beteendet hos den population som fick meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](control-group.md)
