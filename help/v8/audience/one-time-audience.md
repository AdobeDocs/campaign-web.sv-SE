---
audience: end-user
title: Skapa en engångspublik för en leverans
description: Lär dig hur du skapar en engångspublik för en leverans.
badge: label="Begränsad tillgänglighet"
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: a3476e46c29723af8246683a005543cfd605e7df
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# Skapa en engångspublik {#one-time}

I det här avsnittet beskrivs hur du skapar en målgrupp när du skapar en ny leverans. I det här fallet är målet för mottagarna som ska inkluderas i leveransgruppen att fråga databasen med frågemodelleraren.

Den slutliga målgruppen används bara en gång för den här leveransen. Den sparas inte i målgruppslistan.

När du definierar huvudmålet för en leverans kan du också:

* [Välj en befintlig målgrupp](add-audience.md) från **[!UICONTROL Audiences]** lista.
* [Läsa in en målgrupp från en extern fil](file-audience.md) (endast för e-post).

Så här skapar du en ny målgrupp direkt från en leverans:

1. Från **Målgrupp** i leveransguiden klickar du på **[!UICONTROL Select audience]** -knappen.

   ![](assets/segment-builder0.png)

1. Välj **Skapa en egen**. Frågemodelleraren visas. Det gör att du kan definiera målgruppen för leveransen genom att filtrera data i databasen. [Lär dig använda frågemodelleraren](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png)

1. När frågan är klar klickar du **Bekräfta** för att använda målgruppen som huvudmål för leveransen.

   Ni kan också ställa in en kontrollgrupp för att mäta effekten av era kampanjer. Kontrollgruppen tar inte emot meddelandet. På så sätt kan du jämföra beteendet hos den population som fick meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](control-group.md)
