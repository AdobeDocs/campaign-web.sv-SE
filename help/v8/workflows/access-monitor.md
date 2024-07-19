---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Få åtkomst till och hantera arbetsflöden {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Arbetsflöden"
>abstract="På den här skärmen kan du komma åt den fullständiga listan över fristående arbetsflöden och kampanjarbetsflöden, kontrollera deras aktuella status, senaste/nästa körningsdatum och skapa ett nytt arbetsflöde. Bläddra till fliken Mallar för att komma åt tillgängliga arbetsflödesmallar."

På menyn **[!UICONTROL Workflows]** kan du komma åt den fullständiga listan över arbetsflöden. Den här listan innehåller både **fristående arbetsflöden** som har skapats från den här skärmen och **kampanjarbetsflöden** som har skapats i en kampanj.

![](assets/workflow-list.png){zoomable="yes"}

Varje arbetsflöde i listan visar information om dess aktuella [status](#status), den senaste gången det kördes eller ändrades samt nästa schemalagda körningsdatum och -tid.

Du kan anpassa de kolumner som visas genom att klicka på ikonen **[!UICONTROL Configure column for a custom layout]** i det övre högra hörnet av listan. På så sätt kan du lägga till ytterligare information i listan, t.ex. den senaste felaktiviteten för varje arbetsflöde eller den använda måldimensionen.

Dessutom finns det ett sökfält och filter som gör det enklare att söka i listan. Du kan till exempel filtrera arbetsflödena så att de bara visar dem som tillhör en kampanj, eller de som bearbetas under ett visst datumintervall.

Om du vill duplicera eller ta bort ett arbetsflöde klickar du på ellipsknappen och väljer sedan **[!UICONTROL Duplicate]** eller **[!UICONTROL Delete]**.

>[!NOTE]
>
>Du kan duplicera ett pågående arbetsflöde, men du kan inte ta bort det.

## Arbetsflödenas status {#status}

Arbetsflöden kan ha flera statusvärden:

* **[!UICONTROL Draft]**: Arbetsflödet har skapats och sparats.
* **[!UICONTROL In progress]**: Arbetsflödet körs för närvarande.
* **[!UICONTROL Finished]**: Arbetsflödets körning är slutförd.
* **[!UICONTROL Paused]**: Arbetsflödet har pausats.
* **[!UICONTROL Erroneous]**: Ett fel uppstod i arbetsflödet. Öppna arbetsflödet och öppna loggarna och uppgifterna för att identifiera felet och åtgärda det. [Lär dig övervaka loggar och uppgifter](start-monitor-workflows.md#logs-tasks)

Detaljerad information om hur du startar och övervakar arbetsflödeskörning finns på [den här sidan](start-monitor-workflows.md).

## Arbetsflödesmallar {#templates}

Fliken **[!UICONTROL Templates]** visar alla tillgängliga arbetsflödesmallar.

Arbetsflödesmallar innehåller förkonfigurerade aktiviteter och övergripande egenskapskonfigurationer som kan återanvändas för att skapa nya arbetsflöden.

Du kan skapa arbetsflödesmallar från ett befintligt arbetsflöde eller från början. [Lär dig skapa arbetsflödesmallar](create-workflow.md#workflow-templates)
