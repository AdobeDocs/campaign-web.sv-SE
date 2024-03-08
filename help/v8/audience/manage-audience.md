---
audience: end-user
title: Övervaka och hantera målgrupper
description: Lär dig övervaka och hantera målgrupper på Adobe Campaign Web
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Övervaka och hantera målgrupper {#monitor-manage}

## Vad är en publik? {#what}

Målgruppen är huvudmålet för leveransen: de profiler som tar emot meddelandena. Vilken typ av målgrupp det är beror på målmappningen som definieras i leveransmallen. Läs mer om leveransmallar i [den här sidan](../msg/delivery-template.md).

Om du vill definiera en målgrupps befolkning kan du:

* [Skapa nya målgrupper](create-audience.md) från **[!UICONTROL Audiences]** meny,
* [Välj en befintlig målgrupp](add-audience.md) som har skapats som en lista i klientkonsolen eller som kommer från Adobe Experience Platform,
* [Bygg en ny publik](../query/query-modeler-overview.md) med frågemodelleraren genom att definiera och kombinera filtervillkor,
* [Använda en målgrupp från en extern fil](file-audience.md). Det här alternativet är bara tillgängligt för fristående e-postleveranser och kan inte användas i kampanjleveranser.

När ni riktar in er på en målgrupp kan ni också definiera **kontrollgrupper** för att undvika att skicka meddelanden till en del av er målgrupp och mäta effekten av era kampanjer. [Lär dig hur du ställer in en kontrollgrupp](control-group.md)

>[!NOTE]
>
>När meddelanden skickas i samband med ett kampanjarbetsflöde definieras målgruppen i en specifik **Bygg målgrupper** arbetsflödesaktivitet. I det här sammanhanget kan du inte läsa in en målgrupp från en fil för en e-postleverans, och målgruppen definieras endast i den här dedikerade aktiviteten. Lär dig definiera målgruppen för leveransen i ett kampanjarbetsflöde i [det här avsnittet](../workflows/activities/build-audience.md)

## Övervaka målgrupper {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Egenskaper"
>abstract="Här hittar du en sammanfattning av målgruppsegenskaperna, t.ex. ursprung, lagringsmapp eller dess status. Klicka på länken i **Senaste arbetsflöde** för att öppna det arbetsflöde som har använts för att skapa målgruppen."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Målgruppsstorlek"
>abstract="Här hittar du det totala antalet profiler inom målgruppen. Klicka på knappen Beräkna för att uppdatera och beräkna om målgruppsresultaten."

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Målgruppsfel"
>abstract="Målgruppsdata är inte tillgängliga. Vänta på att arbetsflödets körning avslutas."

Listan över målgrupper som kan användas på Campaign Web finns på **[!UICONTROL Audiences]** -menyn.

![](assets/audiences-list.png){zoomable=&quot;yes&quot;}

Målgrupper kan komma från flera olika källor. The **[!UICONTROL Origin]** kolumner anger var en viss målgrupp har skapats:

* **[!UICONTROL Adobe Campaign]**: Dessa målgrupper skapas i Adobe Campaign V8-konsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dessa målgrupper skapas i Adobe Experience Platform och integreras i Campaign Web med hjälp av integreringen Adobe Sources and Destinations. Lär dig hur du konfigurerar den här integreringen i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

  ➡️ [Upptäck den här funktionen i video](#video)

* **[!UICONTROL Adobe Campaign WebUI]**: Dessa målgrupper skapas med Campaign-webbens målgruppsarbetsflöden. [Lär dig skapa målgrupper](create-audience.md)

Om du vill ha mer information om en viss målgrupp öppnar du den i listan. Publiken visas tillsammans med antalet profiler som ingår i publiken. Du kan när som helst uppdatera antalet målgrupper med **[!UICONTROL Calculate]** -knappen.

The **[!UICONTROL Data]** kan du visa de profiler som är en del av publiken. Du kan anpassa den här vyn genom att lägga till fler kolumner eller använda avancerade filter för att förfina de data som visas.

![](assets/audiences-details.png){zoomable=&quot;yes&quot;}

Om du vill duplicera eller ta bort en målgrupp klickar du på **[!UICONTROL More action]** som finns i målgruppslistan bredvid målgruppsnamnet eller i en målgruppsinformationsskärm.

## Instruktionsvideo {#video}

Lär dig hur du skapar en målgrupp som ska användas i Experience Platform i Adobe Campaign webbgränssnitt.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Detaljerad information om hur du konfigurerar integreringen för Adobe-källor och -destinationer finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.
