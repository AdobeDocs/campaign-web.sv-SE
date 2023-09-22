---
audience: end-user
title: Skapa en engångspublik för en leverans
description: Lär dig hur du skapar en engångspublik för en leverans.
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Skapa en engångspublik för en leverans {#sone-time}

I det här avsnittet beskrivs hur du skapar en målgrupp när du skapar en ny leverans. I det här fallet är det mottagarna som ska inkluderas i leveransmålgruppen som mål genom att fråga databasen med regelbyggaren.

Den slutliga målgruppen används bara en gång för den här leveransen. Den sparas inte i målgruppslistan.

När du definierar huvudmålet för en leverans kan du också:

* [Välj en befintlig målgrupp](add-audience.md) från **[!UICONTROL Audiences]** lista.
* [Läsa in en målgrupp från en extern fil](file-audience.md) (endast för e-post).

Så här skapar du en ny målgrupp direkt från en leverans:

1. Från **Målgrupp** i leveransguiden klickar du på **[!UICONTROL Select audience]** -knappen.

   ![](assets/segment-builder0.png)

1. Välj **Skapa en egen**. Regelverktyget visas. Det gör att du kan definiera målgruppen för leveransen genom att filtrera data i databasen. [Lär dig hur du använder regelbyggaren](segment-builder.md)

   ![](assets/segment-builder.png)

1. När frågan är klar klickar du **Bekräfta** för att använda målgruppen som huvudmål för leveransen.

   Ni kan också ställa in en kontrollgrupp för att mäta effekten av era kampanjer. Kontrollgruppen tar inte emot meddelandet. På så sätt kan du jämföra beteendet hos den population som fick meddelandet med beteendet hos kontakter som inte gjorde det. [Läs mer](control-group.md)
