---
audience: end-user
title: Skapa kampanjer med Adobe Campaign Web
description: Lär dig skapa flerkanalskampanjer med Adobe Campaign Web
badge: label="Alpha"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: 5dec05aeffa1268ec3d9b371f4ea91f830247a4f
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 1%

---


# Skapa din första kampanj {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Egenskaper för kampanjskapande"
>abstract="Definiera egenskaper och metadata för kampanjen."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Kampanjegenskaper"
>abstract="Definiera kampanjinställningar och metadata."

Om du vill skapa en ny kampanj måste du definiera dess egenskaper, schemalägga och inkludera arbetsflöden och leveranser.

## Skapa kampanjen{#campaign-create}

Så här skapar du en ny kampanj:

1. Klicka på **[!UICONTROL Campaigns]** och klickar på **[!UICONTROL Create campaign]** -knappen.
1. Välj **Mall** för att använda och tillhandahålla en etikett för kampanjen. Kampanjmallar är förkonfigurerade så att de kan återanvändas för att skapa nya kampanjer. De skapas från klientkonsolen.
   [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html).
1. Om det behövs kan du ändra följande **Ytterligare alternativ**: internt namn, mapp, tilldelad, beskrivning och typ.
1. Definiera **Schema** av er kampanj. Kampanjen startar när startdatumet nås. Start- och slutdatum visas i kampanjlistan och kan användas som filter. Se det här [section](manage-campaigns.md#access-campaigns).

   ![Definiera kampanjegenskaper](assets/campaign-properties.png)

   >[!NOTE]
   >
   >Du kan alltid ändra dessa egenskaper senare från **Konfigurera kampanjinställningar** -ikonen bredvid kampanjetiketten. Se det här [section](gs-campaigns.md#campaign-dashboard).

1. Klicka **Skapa**.
1. Lägg till arbetsflöden och leveranser till kampanjen:

   * Från **Arbetsflöden** flik, klicka **Skapa arbetsflöde**. Ett standardarbetsflöde läggs automatiskt till när du skapar kampanjen. Läs mer om hur [skapa ett arbetsflöde](../workflows/create-workflow.md).
   * Från **Leveranser** flik, klicka **Skapa leverans**. [Läs mer](../msg/gs-messages.md)

1. Använd **Loggar** och **Rapportering** knappar för att analysera kampanjens resultat.

## Övervaka och spåra kampanjen{#campaign-monitoring}

Kampanjövervakning är ett viktigt steg för att analysera hur effektiv er kampanj är. Öppna kampanjen och klicka på **Loggar** -knappen.

Du kan även visa dedikerade rapporter genom att klicka på **Rapporter** -knappen. Se det här [section](../reporting/campaign-reports.md).



<!--
	+++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Workflow list"
>abstract="List of workflows available for your campaign. Use the 'Create workflow' button to add a workflow in your campaign."

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.

-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header


About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and help you organize your marketing activities: you can separate them by country, by brand, by unit, etc.
A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.
To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

Timeline
About dynamic reports
Creating a campaign
In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card and access a program or sub-program.

Click on the Create button and select Campaign.

In the Creation mode screen, select a campaign type.



The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date to your campaign. These dates only apply to the campaign itself.



Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

NOTE
Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.


Programs and campaigns icons and statuses
Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

Gray: the program/campaign has not yet started - Editing status.
Blue: the program/campaign is in progress - In progress status.
Green: the program/campaign has finished - Finished status. By default, the current date is automatically shown as the validity start date and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.


Business.Adobe.com resources
-->
