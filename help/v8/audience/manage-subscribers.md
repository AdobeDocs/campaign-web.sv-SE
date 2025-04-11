---
audience: end-user
title: Hantera prenumeranterna
description: Lär dig hur du hanterar och levererar till abonnenter av en tjänst på Adobe Campaign Web
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Hantera prenumeranterna {#manage-subscribers}

När du [har skapat en tjänst](manage-services.md#create-service) kan du lägga till prenumeranter, avsluta prenumerationer och skicka meddelanden till prenumeranterna för den tjänsten.

Prenumerationshanteringen finns på den här sidan. Mer information om hur du skickar meddelanden till dina prenumeranter finns i [det här avsnittet](../msg/send-to-subscribers.md).

## Lägg till prenumeranter till tjänsten {#add-subscribers}

Följ stegen nedan om du vill lägga till prenumeranter manuellt.

1. Välj en befintlig tjänst i listan **[!UICONTROL Subscription services]**.

1. Gå till fliken **[!UICONTROL Subscribers]** och klicka på **[!UICONTROL Add subscribers]**.

   ![Skärmbild som visar fliken Abonnenter i gränssnittet för prenumerationstjänster.](assets/service-subscribers-tab.png){zoomable="yes"}

1. Markera de profiler som du vill lägga till i listan och klicka på **[!UICONTROL Confirm]**.

   ![Skärmbild som visar gränssnittet för profilval för att lägga till prenumeranter.](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Send]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->om du vill att de valda mottagarna ska få prenumerationens [bekräftelsemeddelande](manage-services.md#create-confirmation-message) som du definierade när du [skapade tjänsten](manage-services.md#create-service).

   ![Skärmbild som visar bekräftelsemeddelandegränssnittet för att lägga till prenumeranter.](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >Om du väljer **[!UICONTROL Cancel]** skickas inget bekräftelsemeddelande till de valda profilerna, men de prenumererar.

De tillagda profilerna visas på fliken **[!UICONTROL Subscribers]**. De prenumererar nu på din tjänst.

## Ta bort prenumeranter från tjänsten {#remove-subscribers}

### Avbeställ profiler manuellt {#manual-unsubscription}

När du har [lagt till prenumeranter](#add-subscribers) i tjänsten kan du avbeställa dem manuellt. Följ stegen nedan.

1. Välj en befintlig tjänst i listan **[!UICONTROL Subscription services]**.

1. Klicka på ikonen med tre punkter bredvid det önskade mottagarnamnet och välj **[!UICONTROL Delete]**.

   ![Skärmbild som visar borttagningsalternativet för att avbryta prenumerationsutskick av profiler.](assets/service-subscribers-delete.png){zoomable="yes"}

1. Bekräfta borttagning.

1. Klicka på **[!UICONTROL Send]** om du vill att den valda mottagaren ska få det [bekräftelsemeddelande](manage-services.md#create-confirmation-message) som du definierade när du [skapade tjänsten](manage-services.md#create-service).

   ![Skärmbild som visar bekräftelsemeddelandegränssnittet för att avbryta prenumerationen.](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

Mottagaren tas bort från fliken **[!UICONTROL Subscribers]** och prenumererar inte längre på tjänsten.

### Avbeställ automatiskt {#automatic-unsubscription}

En prenumerationstjänst kan ha en begränsad varaktighet. Profiler avbryts automatiskt när giltighetsperioden går ut.

Den här perioden anges när [tjänsten](manage-services.md#create-service) skapas. Inaktivera alternativet **[!UICONTROL Unlimited validity period]** från **[!UICONTROL Additional options]** och definiera en giltighetsperiod för tjänsten.

![Skärmbild som visar giltighetsperiodens konfiguration för en prenumerationstjänst.](assets/service-create-validity-period.png){zoomable="yes"}

När den angivna tidsperioden har gått ut upphör alla prenumeranter automatiskt att prenumerera på tjänsten.