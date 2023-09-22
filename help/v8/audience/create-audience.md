---
audience: end-user
title: Skapa och hantera målgrupper
description: Lär dig skapa och hantera målgrupper på Adobe Campaign Web
badge: label="Beta"
source-git-commit: ab445f332b62baa98f9f9e84a80cc336cd88efe0
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 0%

---


# Skapa målgrupper {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Målgrupper"
>abstract="Från den här skärmen kan du komma åt listan över alla målgrupper som kan användas i dina leveranser. Klicka **Skapa** skapa nya målgrupper i en visuell arbetsyta med hjälp av olika arbetsflödesaktiviteter som **Dela** eller **Exkludera**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Målgruppsinställningar"
>abstract="Ange målgruppens namn och ytterligare alternativ och klicka sedan på **Skapa publik** -knappen."

Med Campaign Web kan ni skapa nya målgrupper i ett visuellt arbetsflöde. Förutom att börja från scratch och skapa en enkel målgrupp kan ni också utnyttja arbetsflödesaktiviteter för att förfina er målgrupp. Ni kan till exempel kombinera flera olika målgrupper till en enda, berika er målgrupp med externa attribut eller dela upp en grupp i flera målgrupper baserat på valfria regler.

När ni väl har skapat ert arbetsflöde lagras målgrupperna automatiskt i Campaign-databasen tillsammans med era befintliga. Dessa målgrupper kan sedan inrikta sig på kampanjer eller fristående leveranser.

## Skapa din första målgrupp {#create}

Så här skapar du en målgrupp:

1. Navigera till **[!UICONTROL Audiences]** och klickar på **[!UICONTROL Create Audience]** i det övre högra hörnet.
1. Ange en etikett för er målgrupp.
1. Expandera **[!UICONTROL Additional options]** för att konfigurera avancerade målgruppsparametrar.

   Som standard skapas målgrupper i **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** utforskarmenyn. Du kan ändra standardlagringsplatsen med **[!UICONTROL Folder]** fält.

   ![](assets/audiences-settings.png)

1. När du har konfigurerat målgruppsinställningarna klickar du på **[!UICONTROL Create Audience]** -knappen. En arbetsyta i arbetsflödet visas med två standardaktiviteter:

   * **[!UICONTROL Build audience]**: Detta är startpunkten i arbetsflödet, så att du kan skapa en målgrupp och använda den som grund för arbetsflödet.

   * **[!UICONTROL Save audience]**: Detta är det sista steget i arbetsflödet, vilket gör att du kan spara arbetsflödesresultaten som en ny målgrupp.

1. Öppna **[!UICONTROL Build audience]** och använd regelbyggaren för att definiera den population som ska ingå i målgruppen genom att filtrera data i databasen. [Lär dig konfigurera en målgruppsaktivitet](../workflows/activities/build-audience.md)

1. Om du vill utföra ytterligare åtgärder för den population som är avsedd för arbetsflödet lägger du till så många aktiviteter som behövs och kopplar ihop dem. Mer information om hur du konfigurerar arbetsflödesaktiviteter finns i [arbetsflödesdokumentation](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktiviteter är inte tillgängliga för målgruppsarbetsflöden.

   ![](assets/audience-creation-canvas.png)

1. Konfigurera **[!UICONTROL Save audience]** för att ange hur du vill spara den beräknade populationen uppströms i arbetsflödet. [Lär dig konfigurera en Spara målgruppsaktivitet](../workflows/activities/save-audience.md)

1. När arbetsflödet är klart klickar du **[!UICONTROL Start]** för att genomföra det.

Arbetsflödet sparas i **[!UICONTROL Workflows]** -listan, medan de resulterande målgrupperna är tillgängliga i **[!UICONTROL Audiences]** lista.

## Exempel på målgruppsarbetsflöde {#example}

I exemplet nedan visas ett målgruppsarbetsflöde som är konfigurerat för att rikta sig till kvinnliga kunder som bor i New York och skapa två nya målgrupper beroende på deras senaste köp (Yoga eller Löpande utrustning).

![](assets/audiences-example.png)

1. The **[!UICONTROL Build audience]** Aktiviteten riktar sig till alla kvinnliga profiler som bor i New York.
1. The **[!UICONTROL Enrichment]** aktiviteten berikar publiken med information från inköpstabellen för att identifiera vilken typ av produkt kunderna har köpt.
1. The **[!UICONTROL Split]** aktiviteten delar upp arbetsflödet i två banor baserat på kundens senaste köp.
1. The **[!UICONTROL Save audience]** aktiviteter i slutet av varje bana skapar två nya målgrupper i databasen, inklusive den population som beräknas i varje bana.

## Övervaka och hantera målgrupper {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Målgruppsfel"
>abstract="Målgruppsdata är inte tillgängliga. Vänta på att arbetsflödets körning avslutas."

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
