---
audience: end-user
title: Hantera mediefiler med Adobe Experience Manager as a Cloud Service
description: Lär dig hantera innehåll med Adobe Experience Manager as a Cloud Service
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: 8e035bbf92914f17607a15c184ecf48f5c0efb13
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 1%

---

# Hantera mallar med [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Kom igång med [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

Integreringen av Adobe Campaign webbgränssnitt med Adobe Experience Manager underlättar smidig hantering av e-postinnehåll och formulär direkt i Adobe Experience Manager.

![](assets/do-not-localize/book.png)[Läs mer om Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Skapa en mall i [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Navigera till [!DNL Adobe Experience Manager]-författarinstansen och klicka på Adobe Experience i det övre vänstra hörnet på sidan. Välj **[!UICONTROL Sites]** på menyn.

1. Åtkomst till **[!UICONTROL Campaigns > Name of your brand > Main Area > Name of your page]**.

1. Klicka på **[!UICONTROL Create]** och välj **[!UICONTROL Page]** i listrutan.

   ![](assets/aem_1.png)

1. Välj mallen **[!UICONTROL Adobe Campaign Email]** och ge nyhetsbrevet ett namn.

   ![](assets/aem_2.png)

1. Anpassa e-postinnehållet genom att lägga till komponenter, till exempel anpassningsfält från Adobe Campaign. [Läs mer](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. När e-postmeddelandet är klart går du till menyn **[!UICONTROL Page information]** och klickar på **[!UICONTROL Start workflow]**.

   ![](assets/aem_3.png)

1. I den första listrutan väljer du **[!UICONTROL Approve Adobe Campaign]** som arbetsflödesmodell och klickar på **[!UICONTROL Start workflow]**.

1. En ansvarsfriskrivning visas högst upp på sidan med datumet `This page is subject to the workflow Approve for Adobe Campaign`. Klicka på **[!UICONTROL Complete]** bredvid ansvarsfriskrivningen för att bekräfta granskningen och klicka på **[!UICONTROL Ok]**.

   ![](assets/aem_4.png)

1. Klicka på **[!UICONTROL Complete]** igen och välj **[!UICONTROL Newsletter approval]** i listrutan **[!UICONTROL Next Step]**.

Nyhetsbrevet är nu klart och synkroniserat i Adobe Campaign.

## Importera en Adobe Experience Manager as a Cloud Service-mall{#aem-templates-perso}

När mallen Experience Manager finns tillgänglig på Adobe Campaign Web som innehållsmall kan du identifiera och lägga in det innehåll som behövs för e-postmeddelandet, inklusive personalisering.

1. Klicka på **[!UICONTROL Create delivery]** på menyn **[!UICONTROL Deliveries]** i Campaign Web.

1. Välj den inbyggda mallen **[!UICONTROL Email delivery with AEM content]** i e-postmallfönstret.

   ![](assets/aem_5.png)

1. Ange en **[!UICONTROL Label]** för leveransen och konfigurera ytterligare alternativ baserat på dina behov:

   * **[!UICONTROL Internal name]**: tilldela en unik identifierare till leveransen.

   * **[!UICONTROL Folder]**: lagra leveransen i en viss mapp.

   * **[!UICONTROL Delivery code]**: använd det här fältet för att ordna leveranser baserat på din egen namnkonvention.

   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.

   * **[!UICONTROL Nature]**: Ange typ av e-post för klassificeringssyften.

1. Definiera en **[!UICONTROL Audience]** i e-postmeddelandet. [Läs mer](../email/create-email.md#define-audience)

1. Klicka på **[!UICONTROL Edit content]**.

1. Klicka på **[!UICONTROL Select AEM content]** på menyn **[!UICONTROL Edit content]**.

   ![](assets/aem_6.png)

1. Bläddra igenom AEM och välj den som ska importeras till Campaign Web.

   ![](assets/aem_8.png)

1. Observera att innehåll inte synkroniseras automatiskt. Om mallarna ändras direkt i Adobe Experience Manager väljer du bara **[!UICONTROL Refresh AEM content]** om du vill ha den senaste versionen av mallen.

1. Klicka på **[!UICONTROL Unlink AEM content]** om du vill ta bort länken mellan Experience Manager och Campaign eller om du vill anpassa din Experience Manager-mall ytterligare i e-postdesignern.

   ![](assets/aem_9.png)

1. Om du har lagt till anpassat innehåll i din Experience Manager-mall klickar du på **[!UICONTROL Simulate Content]** för att förhandsgranska hur det kommer att visas i meddelandet med testprofiler.

[Läs mer om förhandsgranskning och testprofiler](../preview-test/preview-content.md)

1. När du visar förhandsgranskningen av meddelandet ersätts alla anpassade element automatiskt med motsvarande data från den valda testprofilen.

   Om det behövs kan ytterligare testprofiler läggas till med knappen **[!UICONTROL Manage test profiles]**.

Leveransen är nu klar att skickas.
