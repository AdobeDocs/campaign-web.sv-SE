---
audience: end-user
title: Skicka meddelanden till prenumeranterna på en tjänst
description: Lär dig hur du skickar meddelanden till prenumeranterna på en tjänst
badge: label="Beta"
source-git-commit: e5ef71de970468fce418cc06cb9d2c25c0c40306
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 1%

---


# Skicka meddelanden till prenumeranterna på en tjänst

Du kan skapa prenumerationstjänster i Adobe Campaign och skicka meddelanden till dina prenumeranter. Lär dig hur du skapar prenumerationstjänster i [den här sidan](../audience//manage-services.md#create-service).

Om du vill skicka meddelanden till dina prenumeranter skapar du en specifik publik som identifierar prenumeranterna och skapar sedan leveransen enligt nedan.

1. Skapa en målgrupp. Läs mer om målgrupper i [den här sidan](../audience/create-audience.md).

1. I **[!UICONTROL Build audience]** aktivitet, visa avancerade attribut och markera **[!UICONTROL Recipient]** > **[!UICONTROL Subscriptions]** > **[!UICONTROL Service]**.

   I det här exemplet väljer du de användare som prenumererar på tjänsten som har **Luma Newsletter** etikett.

   ![](assets/service-audience-subscribers.png)

1. Spara publiken.
1. Skapa en leverans. Steg för att skapa en leverans beskrivs i [den här sidan](../msg/gs-messages.md#create-delivery).
1. Bläddra till leveransinställningarna och ändra standardmålmappningen till **Prenumerationer (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. I huvudmåldelen av leveransen väljer du den målgrupp du skapade ovan.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Skapa meddelandeinnehåll, testa och skicka leveransen, enligt informationen i [det här avsnittet](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

Leveransen skickas endast till prenumeranterna av tjänsten.
