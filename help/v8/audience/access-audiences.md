---
audience: end-user
title: Övervaka och hantera målgrupper
description: Lär dig övervaka och hantera målgrupper på Adobe Campaign Web
badge: label="Beta"
source-git-commit: 4924653e67f77a2108574e743c9016c6fc95a7e6
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---


# Övervaka och hantera målgrupper {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="Den här målgruppen är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här målgruppen. Kontakta administratören om det behövs för att ge dig åtkomst."

Listan över målgrupper som kan användas på Campaign Web finns på **[!UICONTROL Audiences]** -menyn.

![](assets/audiences-list.png)

Målgrupper kan komma från flera olika källor. The **[!UICONTROL Origin]** kolumner anger var en viss målgrupp har skapats:

* **[!UICONTROL Adobe Campaign]**: Dessa målgrupper skapas i Adobe Campaign V8-konsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dessa målgrupper skapas i Adobe Experience Platform och integreras i Campaign Web med hjälp av integreringen Adobe Sources and Destinations. Lär dig hur du konfigurerar den här integreringen i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Adobe Campaign WebUI]**: Dessa målgrupper skapas med Campaign-webbens målgruppsarbetsflöden. [Lär dig skapa målgrupper](create-audience.md)

Om du vill ha mer information om en viss målgrupp öppnar du den i listan. Publiken visas tillsammans med antalet profiler som ingår i publiken. Du kan när som helst uppdatera antalet målgrupper med **[!UICONTROL Calculate]** -knappen.

The **[!UICONTROL Data]** kan du visa de profiler som är en del av publiken. Du kan anpassa den här vyn genom att lägga till fler kolumner eller använda avancerade filter för att förfina de data som visas.

![](assets/audiences-details.png)

Om du vill duplicera eller ta bort en målgrupp klickar du på **[!UICONTROL More action]** som finns i målgruppslistan bredvid målgruppsnamnet eller i en målgruppsinformationsskärm.
