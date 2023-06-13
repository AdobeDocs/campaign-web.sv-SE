---
audience: end-user
title: Kom igång med kampanjer
description: Lär dig hur du börjar med flerkanalskampanjer
badge: label="Alpha" type="Positive"
exl-id: f2b9f8e6-5ded-4a47-89e9-96650cd78229
source-git-commit: e933562e4046d9cdea9fc898e5c4c4c9a7e9ee38
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---


# Kom igång med kampanjer {#campaigns}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Utforma och skicka flerkanalskampanjer"
>abstract="Adobe Campaign-funktioner hjälper er att hantera centraliserade kunddata, utforma kundkommunikation och kampanjer och skapa personaliserade upplevelser i olika kanaler: E-post, push och SMS."

Med Adobe Campaign kan ni enkelt samordna era riktade marknadsföringssatsningar med den inbyggda kampanjhanteringsfunktionen. Med möjligheten att definiera ett schema kan ni planera kampanjernas varaktighet och tidsplanering för att anpassa dem till strategiska mål och maximera målgruppernas engagemang.

Genom att lägga till flera arbetsflöden och leveranser som är specifika för kampanjen kan ni skapa personaliserade upplevelser i olika kanaler och säkerställa att varje kontaktyta passar den avsedda målgruppen.

Kampanjerna erbjuder dedikerade rapporteringsmått för att få omfattande insikter om resultatet för hela kampanjen, så att ni kan bedöma hur effektiv den är, identifiera trender och fatta datadrivna beslut för att optimera framtida insatser.

<!--
Use Adobe Campaign to create cross-channel campaigns. With its marketing campaign orchestration capabilities, you can manage and centralize customer data, design customer communications and campaigns, and create personalized experiences across different channels. In this version, email, push and SMS channels are available.

Design and execute high-volume email campaigns to deliver personalized messages, for all platforms and screen sizes. 
Measure the effectiveness of your deliveries with detailed reports including the counts of opens, clicks, forwards, and more. With Adobe Campaign segmentation capabilities, you can run queries against a high-volume database, and easily define dynamic marketing segments which perfectly target your campaigns.
-->

<!--
Get Started with campaigns
Adobe Campaign offers a set of solutions that help you personalize and deliver campaigns across all of your online and offline channels. You can create, configure, execute and analyze marketing campaigns. All marketing campaigns can be managed from a unified control center. Discover how to browse and create marketing campaigns in this section.

Campaigns include actions (deliveries) and processes (importing or extracting files), as well as resources (marketing documents, delivery outlines). They are used in marketing campaigns. Campaigns are part of a program, and programs are included in a campaign plan.
-->

## Få tillgång till och hantera era kampanjer{#access-campaigns}

Om du vill skapa en ny kampanj eller hantera befintliga kampanjer klickar du på **[!UICONTROL Campaigns]** -menyn. Det finns två flikar:

* The **Bläddra** alla befintliga kampanjer visas på fliken. Du kan klicka på en kampanj för att öppna instrumentpanelen eller skapa en ny kampanj genom att klicka på **Skapa kampanj** -knappen. Se det här [section](create-campaigns.md#create-campaigns)

* The **Mallar** På -fliken visas alla tillgängliga kampanjmallar. Kampanjmallar är förkonfigurerade så att de kan återanvändas för att skapa nya kampanjer. De skapas från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html).

Varje kampanj i listan visar information om dess aktuella status, skapandedatum, senaste gången den ändrades osv.

Du kan anpassa de kolumner som visas genom att klicka på **Konfigurera kolumn för en anpassad layout** -ikonen i det övre högra hörnet av listan. På så sätt kan du lägga till ytterligare information i listan. Dessutom finns det ett sökfält och filter som gör det enklare att söka i listan. [Läs mer](../get-started/user-interface.md#list-screens)

Du kan till exempel filtrera efter kampanjschemat. Öppna filterpanelen och använd **Start - slutdatum** avsnitt:

![Kampanjlista](assets/campaign-filter-on-dates.png)

## Kontrollpanelen för kampanjer{#campaign-dashboard}

I **Bläddra** klickar du på en kampanj för att visa dess instrumentpanel. Det finns två flikar:

* The **Arbetsflöden** På -fliken visas alla arbetsflöden som är kopplade till kampanjen. På den här fliken kan du även skapa ett nytt arbetsflöde i kampanjen. Se det här [section](create-campaigns.md#create-campaigns)
* The **Leveranser** På fliken visas alla leveranser som är kopplade till kampanjen. På den här fliken kan du även skapa en ny leverans i kampanjen. Se det här [section](create-campaigns.md#create-campaigns)

The **Konfigurera kampanjinställningar** kan du ändra kampanjens egenskaper som definierades när kampanjen skapades. Se det här [section](create-campaigns.md#create-campaigns)

## Övervaka och spåra loggar{#campaign-monitoring}

Kampanjövervakning är ett viktigt steg för att analysera era kampanjer. Öppna kampanjen och klicka på **Loggar** -knappen.

Du kan även visa dedikerade rapporter genom att klicka på **Rapporter** -knappen. Se det här [section](../reporting/campaign-reports.md).

## Duplicera och ta bort

Du kan duplicera eller ta bort en kampanj:

* Klicka på ellipsknappen i listan över kampanjer och välj sedan **Duplicera** eller **Ta bort**.
* från själva kampanjen klickar du på **Mer** knapp och markera **Duplicera** eller **Ta bort**.

>[!NOTE]
>
>The **Leverans** På fliken visas alla leveranser som är länkade till kampanjen, men leveranser som har skapats i ett arbetsflöde kan inte tas bort därifrån. Om du vill ta bort en leverans som har skapats i ett arbetsflöde måste du ta bort leveransaktiviteten från arbetsflödet.

