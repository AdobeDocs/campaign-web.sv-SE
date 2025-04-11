---
audience: end-user
title: Skicka meddelanden till prenumeranterna på en tjänst
description: Lär dig hur du skickar meddelanden till prenumeranterna på en tjänst
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Skicka meddelanden till prenumeranterna på en tjänst {#send-to-subscribers}

Du kan skapa prenumerationstjänster i Adobe Campaign och skicka meddelanden till dina prenumeranter. Lär dig hur du skapar prenumerationstjänster på [den här sidan](../audience//manage-services.md#create-service).

Om du vill skicka meddelanden till dina prenumeranter skapar du en specifik publik som identifierar prenumeranterna och skapar sedan leveransen enligt nedan.

1. Skapa en målgrupp. Ett nytt arbetsflöde skapas automatiskt. [Läs mer om målgrupper](../audience/create-audience.md).

1. För bättre läsbarhet kan du ändra arbetsflödets namn i fältet **Etikett** i arbetsflödesinställningarna. [Lär dig konfigurera arbetsflödesinställningar](../workflows/workflow-settings.md).

1. Öppna aktiviteten **[!UICONTROL Build audience]** och välj **[!UICONTROL Create audience]**. [Lär dig konfigurera en målgruppsaktivitet](../workflows/activities/build-audience.md).

   ![Skärmbild som visar konfigurationen för att skapa målgruppsaktivitet i Adobe Campaign.](assets/service-create-audience.png){zoomable="yes"}

1. Välj följande anpassade villkor i flödet för målgruppsskapande: **[!UICONTROL Subscriptions]** finns, t.ex. **[!UICONTROL Service]** är lika med den tjänst du definierade. I det här exemplet väljer du ditt **Luma yoga-nyhetsbrev**.

   ![Skärmbild som visar hur målgruppen skapas med anpassade villkor för prenumerationer i Adobe Campaign.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Välj **[!UICONTROL Confirm]** och klicka på **[!UICONTROL Start]** för att köra arbetsflödet.

1. Skapa en leverans. Steg för att skapa en leverans beskrivs på [den här sidan](../msg/gs-messages.md#create-delivery).

1. Bläddra till leveransinställningarna och ändra standardmålmappningen till **Prenumerationer (nms:subscriptions)**.

   ![Skärmbild som visar leveransinställningarna med målmappningen ändrad till Prenumerationer i Adobe Campaign.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. I huvudmåldelen av leveransen väljer du den målgrupp du skapade ovan.

   ![Skärmbild som visar huvudmåldelen av leveransen med den valda målgruppen i Adobe Campaign.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Skapa ditt meddelandeinnehåll, testa det och skicka leveransen, så som beskrivs i [det här avsnittet](../preview-test/preview-test.md).

   ![Skärmbild som visar leveransen som är klar att skickas i Adobe Campaign.](assets/service-delivery-ready.png){zoomable="yes"}

Leveransen skickas endast till prenumeranterna av tjänsten.