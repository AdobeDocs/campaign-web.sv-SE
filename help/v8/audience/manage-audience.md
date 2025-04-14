---
audience: end-user
title: Kom igång med målgrupper
description: Lär dig hur du arbetar med målgrupper på Adobe Campaign Web
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Kom igång med målgrupper {#monitor-manage}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Properties"
>abstract="Here you can find a summary of the audience properties, such as its origin or its storage folder. Click the link in the **Last workflow** section to open the workflow that has been used to create the audience."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Audience size"
>abstract="Here you can find the total number of profiles within the audience. Click the **Calculate** button to update and recalculate the audience results."

>[!CONTEXTUALHELP]
>id="acw_audiences_targeting"
>title="Targeting"
>abstract="Targeting"

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Audience error"
>abstract="Audience data is not available. Please wait for the end of the workflow execution."

Målgruppen är huvudmålet för leveransen: de profiler som tar emot meddelandena. Listan över målgrupper som är tillgängliga för användning i Campaign Web finns på menyn **[!UICONTROL Audiences]**.

![Skärmbild som visar en lista över tillgängliga målgrupper på Campaign Web.](assets/audiences-list.png){zoomable="yes"}

Målgrupper kan komma från flera olika källor. Kolumnen **[!UICONTROL Origin]** anger var en viss målgrupp har skapats:

* **[!UICONTROL Adobe Campaign]**: Dessa målgrupper har skapats i [Adobe Campaign webbanvändargränssnitt](create-audience.md) eller i [Adobe Campaign v8-klientkonsolen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dessa målgrupper har skapats i Adobe Experience Platform och är integrerade i Campaign Web med Adobe Sources and Destinations-integrering. Lär dig hur du konfigurerar den här integreringen i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

  ➡️ [Upptäck den här funktionen i videon](#video)

Om du vill ha mer information om en viss målgrupp öppnar du den i listan. Publiken visas tillsammans med antalet profiler som ingår i publiken. Uppdatera antalet målgrupper när som helst med knappen **[!UICONTROL Calculate]**.

På fliken **[!UICONTROL Data]** kan du visualisera de profiler som är en del av målgruppen. Anpassa den här vyn genom att lägga till ytterligare kolumner eller använda avancerade filter för att förfina de data som visas.

![Skärmbild som visar målgruppsinformation, inklusive profiler och anpassningsalternativ.](assets/audiences-details.png){zoomable="yes"}

Om du vill duplicera eller ta bort en målgrupp klickar du på knappen **[!UICONTROL More action]** i målgruppslistan bredvid målgruppsnamnet eller i en skärm med målgruppsinformation.

## Instruktionsvideo {#video}

Lär dig hur du skapar ett mål som ska användas av en Experience Platform-användare i Adobe Campaign webbgränssnitt.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Detaljerad information om hur du konfigurerar integreringen av Adobe-källor och mål finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.