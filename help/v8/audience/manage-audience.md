---
audience: end-user
title: Kom igång med målgrupper
description: Lär dig hur du arbetar med målgrupper på Adobe Campaign Web
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: b330230a031a366b674ebac37681274ee89ec6c8
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Kom igång med målgrupper {#monitor-manage}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Egenskaper"
>abstract="Här finns en sammanfattning av målgruppsegenskaperna, t.ex. dess ursprung eller lagringsmapp. Klicka på länken i avsnittet **Senaste arbetsflöde** för att öppna det arbetsflöde som har använts för att skapa målgruppen."

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
>abstract="Målgruppsdata är inte tillgängliga. Vänta tills arbetsflödets körning har avslutats."

Målgruppen är huvudmålet för leveransen: de profiler som tar emot meddelandena. Listan över målgrupper som är tillgängliga för användning i Campaign Web finns på menyn **[!UICONTROL Audiences]**.

![Skärmbild som visar en lista över tillgängliga målgrupper på Campaign Web.](assets/audiences-list.png){zoomable="yes"}

Målgrupper kan komma från flera olika källor. Kolumnen **[!UICONTROL Origin]** anger var en viss målgrupp har skapats:

* **[!UICONTROL Adobe Campaign]**: Dessa målgrupper har skapats i [Adobe Campaign webbanvändargränssnitt](create-audience.md) eller i [Adobe Campaign v8-klientkonsolen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=sv-SE){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dessa målgrupper har skapats i Adobe Experience Platform och är integrerade i Campaign Web med Adobe Sources and Destinations-integrering. Lär dig hur du konfigurerar den här integreringen i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=sv-SE){target="_blank"}.

  ➡️ [Upptäck den här funktionen i en video](#video)

Om du vill ha mer information om en viss målgrupp öppnar du den i listan. Publiken visas tillsammans med antalet profiler som ingår i publiken. Uppdatera antalet målgrupper när som helst med knappen **[!UICONTROL Calculate]**.

Om du vill förhandsgranska det tillfälliga schemat för en målgrupp klickar du på knappen **[!UICONTROL Schema preview]** under avsnittet Egenskaper.

På fliken **[!UICONTROL Data]** kan du visualisera de profiler som är en del av målgruppen. Anpassa den här vyn genom att lägga till ytterligare kolumner eller använda avancerade filter för att förfina de data som visas.

![Skärmbild som visar målgruppsinformation, inklusive profiler och anpassningsalternativ.](assets/audiences-details.png){zoomable="yes"}

Om du vill duplicera eller ta bort en målgrupp klickar du på knappen **[!UICONTROL More action]** i målgruppslistan bredvid målgruppsnamnet eller i en skärm med målgruppsinformation.

## Instruktionsvideo {#video}

Lär dig hur du skapar ett mål som ska användas av en Experience Platform-användare i Adobe Campaign webbgränssnitt.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Detaljerad information om hur du konfigurerar integreringen av Adobe-källor och mål finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=sv-SE){target="_blank"}.