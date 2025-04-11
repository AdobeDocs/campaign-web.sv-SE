---
audience: end-user
title: Skapa en engångspublik för en leverans
description: Lär dig hur du skapar en engångspublik för en leverans.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Skapa en engångspublik {#one-time}

I det här avsnittet beskrivs hur du skapar en målgrupp när du skapar en ny leverans. I det här scenariot används profiler som ingår i leveransgruppen för att fråga databasen med hjälp av frågemodelleraren. Den slutliga målgruppen används bara en gång för den här leveransen och sparas inte i målgruppslistan.

När du definierar huvudmålet för en leverans kan du också:
* [Välj en befintlig målgrupp](add-audience.md) i listan **[!UICONTROL Audiences]**.
* [Läs in en målgrupp från en extern fil](file-audience.md) (endast för e-post).

Så här skapar du en ny målgrupp för en leverans:

1. Klicka på knappen **[!UICONTROL Select audience]** i sektionen **Målgrupp** i leveransassistenten.

   [Skärmbild som visar Audience-delen av leveransassistenten med knappen Select audience (Välj publik) markerad](assets/segment-builder0.png){zoomable="yes"}

1. Välj **Skapa en egen** för att öppna frågemodelleraren. Med frågemodelleraren kan du definiera målpopulationen genom att filtrera data i databasen. [Lär dig använda frågemodelleraren](../query/query-modeler-overview.md).

   [Skärmbild som visar frågemodelleringsgränssnittet](assets/query-modeler.png){zoomable="yes"}

1. När frågan är klar klickar du på **Bekräfta** för att använda den slutliga målgruppen som huvudmål för leveransen.

   Ni kan också ställa in en kontrollgrupp för att mäta effekten av era kampanjer. Kontrollgruppen tar inte emot meddelandet. På så sätt kan du jämföra beteendet hos den population som fick meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](control-group.md).