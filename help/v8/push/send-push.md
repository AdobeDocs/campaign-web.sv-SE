---
audience: end-user
title: Skicka en leverans av push-meddelanden
description: Lär dig hur du skickar ett push-meddelande via Adobe Campaign Web
badge: label="Alpha"
source-git-commit: c24b53ee17e81805f0717682202d2d4154c96c1e
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Förhandsgranska och skicka en leverans av push-meddelanden {#send-push-delivery}

## Förhandsgranska leverans av push-meddelanden {#preview-push}

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet. Om du har inkluderat anpassat innehåll kan du undersöka hur det här innehållet visas i meddelandet med hjälp av testprofildata. På så sätt kan du se till att meddelandet återges korrekt och att de anpassade elementen införlivas på rätt sätt.

De viktigaste stegen för att förhandsgranska SMS-leveransen är följande. Mer information om hur du förhandsgranskar leveranser finns i [det här avsnittet](../preview-test/preview-content.md).

1. Använd **[!UICONTROL Simulate content]** för att förhandsgranska ditt personaliserade innehåll.

   ![](assets/push_send_1.png)

1. Klicka **[!UICONTROL Add subscribers(s)]** om du vill välja en eller flera profiler för att förhandsgranska deras data i push-meddelandeinnehållet.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. I den högra rutan hittar du en förhandsgranskning av push-meddelandet, där personaliserade element dynamiskt ersätts med data från den valda profilen.

   ![](assets/push_send_7.png)

Nu kan ni granska och skicka push-meddelanden till era målgrupper.

## Testa leveransen av push-meddelanden {#test-push}

Använda **Adobe Campaign**kan du testa push-meddelanden innan du skickar dem till huvudmålgruppen. Det här steget är viktigt när du ska validera leveransen och identifiera eventuella problem.
Testmottagarna kan granska element som länkar, bilder och personaliseringsinställningar för att få bästa möjliga prestanda och upptäcka eventuella fel. Med den här processen kan ni förfina och optimera era push-meddelanden innan ni når er huvudmålgrupp.

![](../assets/do-not-localize/book.png) Lär dig hur du skickar push-meddelanden för testning i [det här avsnittet](../preview-test/proofs.md#subscribers).

![](assets/push_send_6.png)

## Skicka push-meddelanden {#send-push}

1. När du har anpassat ditt push-meddelandeinnehåll klickar du på **[!UICONTROL Review & send]** från **[!UICONTROL Delivery]** sida.

   ![](assets/push_send_2.png)

1. Klicka **[!UICONTROL Prepare]**och övervaka framstegen och statistiken.

   Om det uppstår några fel hittar du detaljerad information om felet på loggmenyn.

   ![](assets/push_send_3.png)

1. Skicka meddelanden genom att klicka på **[!UICONTROL Send]** för att fortsätta med den slutliga sändningsprocessen.

1. Bekräfta skicka-åtgärden genom att klicka på knappen **[!UICONTROL Send]** eller **[!UICONTROL Send as scheduled]** -knappen.

   ![](assets/push_send_4.png)

När leveransen har skickats kan du spåra dina KPI-data (Key Performance Indicator) från leveranssidan och data från **[!UICONTROL Logs]** -menyn.

Nu kan du börja mäta effekten av ditt meddelande med inbyggda rapporter. [Läs mer](../reporting/push-report.md)
