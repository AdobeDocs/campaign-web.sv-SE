---
audience: end-user
title: Hantera prenumeranterna
description: Lär dig hur du hanterar och levererar till abonnenter av en tjänst på Adobe Campaign Web
badge: label="Beta"
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Hantera prenumeranterna {#manage-subscribers}

En gång [skapade en tjänst](manage-services.md#create-service)kan du lägga till prenumeranter, avsluta prenumerationer och skicka meddelanden till prenumeranterna för den tjänsten.

Prenumerationshanteringen finns på den här sidan. Mer information om hur du skickar meddelanden till prenumeranterna finns i [det här avsnittet](../msg/send-to-subscribers.md).

## Lägg till prenumeranter till tjänsten {#add-subscribers}

Följ stegen nedan om du vill lägga till prenumeranter manuellt.

1. Välj en befintlig tjänst från **[!UICONTROL Subscription services]** lista.

1. Välj **[!UICONTROL Subscribers]** och klicka **[!UICONTROL Add profiles]**.

   ![](assets/service-subscribers-tab.png)

1. Markera de profiler som du vill lägga till i listan och klicka på **[!UICONTROL Confirm]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Klicka på **[!UICONTROL Send]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> De valda mottagarna får prenumerationen [bekräftelsemeddelande](manage-services.md#create-confirmation-message) som du valde när [skapa tjänsten](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

De tillagda profilerna visas i **[!UICONTROL Subscribers]** lista. De prenumererar nu på din tjänst.

## Ta bort prenumeranter från tjänsten {#remove-subscribers}

### Avbeställ prenumerationer manuellt {#manual-unsubscription}

En gång [tillagda prenumeranter](#add-subscribers) till tjänsten kan du avbeställa prenumerationen manuellt. Följ stegen nedan.

1. Välj en befintlig tjänst från **[!UICONTROL Subscription services]** lista.

1. Klicka på ikonen med tre punkter bredvid det önskade mottagarnamnet och välj **[!UICONTROL Delete]**.

   ![](assets/service-subscribers-delete.png)

1. Bekräfta borttagning och klicka på **[!UICONTROL Send]**. Den valda mottagaren får en prenumeration [bekräftelsemeddelande](manage-services.md#create-confirmation-message) som du valde när [skapa tjänsten](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

Mottagaren tas bort från **[!UICONTROL Subscribers]** och prenumererar inte längre på din tjänst.

### Avbeställ automatiskt {#automatic-unsubscription}

En prenumerationstjänst kan ha en begränsad varaktighet. Mottagarna avbeställs automatiskt när giltighetsperioden går ut.

Den här perioden anges när [skapa tjänsten](manage-services.md#create-service). Från **[!UICONTROL Additional options]**, inaktivera **[!UICONTROL Unlimited validity period]** och definiera en giltighetsperiod för tjänsten.

![](assets/service-create-validity-period.png)

När den angivna tidsperioden har gått ut upphör alla prenumeranter automatiskt att prenumerera på tjänsten.
