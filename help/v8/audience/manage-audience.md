---
audience: end-user
title: Kom igång med målgrupper
description: Lär dig hur du arbetar med målgrupper på Adobe Campaign Web
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 78c288f6681040170d49f6b67a3db362710f9d0c
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Kom igång med målgrupper {#monitor-manage}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Egenskaper"
>abstract="Här hittar du en sammanfattning av målgruppsegenskaperna, t.ex. dess ursprung eller lagringsmapp. Klicka på länken i avsnittet **Senaste arbetsflöde** för att öppna det arbetsflöde som har använts för att skapa målgruppen."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Målgruppsstorlek"
>abstract="Här hittar du det totala antalet profiler inom målgruppen. Klicka på knappen **Beräkna** för att uppdatera och beräkna målgruppsresultaten på nytt."

>[!CONTEXTUALHELP]
>id="acw_audiences_targeting"
>title="Målinriktning"
>abstract="Målinriktning"

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Målgruppsfel"
>abstract="Målgruppsdata är inte tillgängliga. Vänta på att arbetsflödets körning avslutas."

Målgruppen är huvudmålet för leveransen: de profiler som tar emot meddelandena. Listan över målgrupper som är tillgängliga för användning i Campaign Web finns på menyn **[!UICONTROL Audiences]**.

![](assets/audiences-list.png){zoomable="yes"}

Målgrupper kan komma från flera olika källor. Kolumnerna **[!UICONTROL Origin]** anger var en viss målgrupp har skapats:

* **[!UICONTROL Adobe Campaign]**: Dessa målgrupper har skapats i [Adobe Campaign webbanvändargränssnitt](create-audience.md) eller i [Adobe Campaign v8-klientkonsolen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dessa målgrupper har skapats i Adobe Experience Platform och är integrerade i Campaign Web med hjälp av integreringen Adobe Sources and Destinations. Lär dig hur du konfigurerar den här integreringen i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

  ➡️ [Upptäck den här funktionen i videon](#video)

Om du vill ha mer information om en viss målgrupp öppnar du den i listan. Publiken visas tillsammans med antalet profiler som ingår i publiken. Du kan när som helst uppdatera antalet målgrupper med knappen **[!UICONTROL Calculate]**.

På fliken **[!UICONTROL Data]** kan du visa profilerna som är en del av målgruppen. Du kan anpassa den här vyn genom att lägga till fler kolumner eller använda avancerade filter för att förfina de data som visas.

![](assets/audiences-details.png){zoomable="yes"}

Om du vill duplicera eller ta bort en målgrupp klickar du på knappen **[!UICONTROL More action]** i målgruppslistan bredvid målgruppsnamnet eller i en skärm med målgruppsinformation.

## Instruktionsvideo {#video}

Lär dig hur du skapar en målgrupp som ska användas i Experience Platform i Adobe Campaign webbgränssnitt.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Detaljerad information om hur du konfigurerar integreringen för Adobe-källor och -mål finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.
