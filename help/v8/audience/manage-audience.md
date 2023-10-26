---
audience: end-user
title: Övervaka och hantera målgrupper
description: Lär dig övervaka och hantera målgrupper på Adobe Campaign Web
badge: label="Beta"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Övervaka och hantera målgrupper {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Målgruppsfel"
>abstract="Målgruppsdata är inte tillgängliga. Vänta på att arbetsflödets körning avslutas."

Listan över målgrupper som kan användas på Campaign Web finns på **[!UICONTROL Audiences]** -menyn.

![](assets/audiences-list.png)

Målgrupper kan komma från flera olika källor. The **[!UICONTROL Origin]** kolumner anger var en viss målgrupp har skapats:

* **[!UICONTROL Adobe Campaign]**: Dessa målgrupper skapas i Adobe Campaign V8-konsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dessa målgrupper skapas i Adobe Experience Platform och integreras i Campaign Web med hjälp av integreringen Adobe Sources and Destinations. Lär dig hur du konfigurerar den här integreringen i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

>[!NOTE]
>
>Om du vill använda Adobe Experience Platform målgrupper i Campaign måste du konfigurera integreringen med Adobe Sources and Destinations. Se [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL Adobe Campaign WebUI]**: Dessa målgrupper skapas med Campaign-webbens målgruppsarbetsflöden. [Lär dig skapa målgrupper](create-audience.md)

Om du vill ha mer information om en viss målgrupp öppnar du den i listan. Publiken visas tillsammans med antalet profiler som ingår i publiken. Du kan när som helst uppdatera antalet målgrupper med **[!UICONTROL Calculate]** -knappen.

The **[!UICONTROL Data]** kan du visa de profiler som är en del av publiken. Du kan anpassa den här vyn genom att lägga till fler kolumner eller använda avancerade filter för att förfina de data som visas.

![](assets/audiences-details.png)

Om du vill duplicera eller ta bort en målgrupp klickar du på **[!UICONTROL More action]** som finns i målgruppslistan bredvid målgruppsnamnet eller i en målgruppsinformationsskärm.
