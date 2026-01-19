---
audience: end-user
title: Skapa kampanjer med Adobe Campaign Web
description: Lär dig skapa flerkanalskampanjer med Adobe Campaign Web
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: f1fe8e08401f6ad98ab6920c9ae33fa6336c209d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Skapa din första kampanj {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Egenskaper för kampanjskapande"
>abstract="Ange kampanjinställningarna på den här skärmen: välj en mall och ange en etikett för kampanjen. Bläddra till de extra inställningarna om du vill ändra standardnamnet på den interna mappen, lägga till en beskrivning och välja den som ska tilldelas."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Kampanjegenskaper"
>abstract="På den här skärmen kan du kontrollera och uppdatera kampanjinställningarna: etikett, internt namn, mapp och beskrivning. Du kan också visa vilken användare det är tilldelat."

Om du vill skapa en ny kampanj definierar du dess inställningar, schema och inkluderar arbetsflöden och leveranser.

## Skapa kampanjen {#campaign-create}

Så här skapar du en ny kampanj:

1. Klicka på menyn **[!UICONTROL Campaigns]** och klicka på knappen **[!UICONTROL Create campaign]**.

   ![Skärmbild som visar knappen &quot;Skapa kampanj&quot; på menyn Kampanjer](assets/create-campaign-button.png)

1. Välj den **mall** som ska användas och ange en etikett för kampanjen. [Läs mer](manage-campaigns.md#manage-campaign-templates).
1. Ändra vid behov följande **ytterligare alternativ**: internt namn, mapp, tilldelad, beskrivning och typ.
1. Definiera **schemat** för din kampanj. Lär dig hur du ställer in kampanjschemat i [det här avsnittet](#campaign-schedule).
1. Klicka på **Skapa**.

   ![Skärmbild som visar skärmen för kampanjegenskaper, inklusive fält för internt namn, mapp, tilldelad, beskrivning och natur.](assets/create-a-campaign-properties.png)

1. Lägg till arbetsflöden och leveranser till kampanjen:

   * Klicka på **Skapa arbetsflöde** på fliken **Arbetsflöden**. Ett standardarbetsflöde läggs automatiskt till när du skapar kampanjen. Läs mer om hur du [skapar ett arbetsflöde](../workflows/create-workflow.md).

   * Klicka på **Skapa leverans** på fliken **Leveranser**. [Läs mer](../msg/gs-messages.md)

## Övervaka och spåra kampanjen {#campaign-monitoring}

Kampanjövervakning är ett viktigt steg för att analysera hur effektiv er kampanj är. Öppna kampanjen och klicka på knappen **Loggar**.

Du kan även visa de dedikerade rapporterna genom att klicka på knappen **Rapporter** . Se [avsnittet](../reporting/campaign-reports.md).

## Definiera kampanjschemat {#campaign-schedule}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="Kampanjschema"
>abstract="Välj kampanjschemat. Du kan skapa kampanjen och den startar när startdatumet nås. Som standard är kampanjens startdatum skapandedatum och varar i 5 dagar. Start- och slutdatum visas i kampanjlistan och kan användas som filter."

Kampanjen startar när startdatumet nås. Så länge startdatumet inte nås har kampanjen statusen **[!UICONTROL Draft]**. När startdatumet nås blir det **[!UICONTROL In progress]**. När slutdatumet har nåtts ställs kampanjen in på **[!UICONTROL Completed]**.

Start- och slutdatum visas i kampanjlistan och kan användas som filter. Se [avsnittet](manage-campaigns.md#access-campaigns).

>[!NOTE]
>
>Du kan ändra de här egenskaperna senare från ikonen **Konfigurera kampanjinställningar** bredvid kampanjetiketten. Se [avsnittet](gs-campaigns.md#campaign-dashboard).

När datumet har nåtts skickas leveranser som skapats i kampanjen i ett arbetsflöde och som är klart att skickas. För detta måste arbetsflödet ha startats.

<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.
-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header

About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and helps you organize your marketing activities: you can separate them by country, by brand, by unit, and similar criteria.

A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.

To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

* Timeline
* About dynamic reports
* Creating a campaign

In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card, and access a program or sub-program.

Click on the Create button, and select Campaign.

In the Creation mode screen, select a campaign type.

The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date for your campaign. These dates only apply to the campaign itself.

Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

>[!NOTE]
>
>Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.

Programs and campaigns icons and statuses:

Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

* Gray: the program/campaign has not yet started - Editing status.
* Blue: the program/campaign is in progress - In progress status.
* Green: the program/campaign has finished - Finished status.

By default, the current date is automatically shown as the validity start date, and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.

Business.Adobe.com resources
-->