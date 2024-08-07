---
audience: end-user
title: Skicka SMS-leverans
description: Lär dig hur du skickar SMS med Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Förhandsgranska och skicka en SMS-leverans {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nytt karantänmätvärde"
>abstract="Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras."

## Förhandsgranska SMS-leveransen{#preview-sms}

När du har definierat meddelandeinnehållet kan du använda testprofiler för att förhandsgranska och testa det. Om du har inkluderat anpassat innehåll kan du undersöka hur det här innehållet visas i meddelandet med hjälp av testprofildata. På så sätt kan du se till att meddelandet visas som det ska och att all personlig information presenteras korrekt.

De viktigaste stegen för att förhandsgranska SMS-leveransen är följande. Mer information om hur du förhandsgranskar leveranser finns i [det här avsnittet](../preview-test/preview-content.md).

1. Använd **[!UICONTROL Simulate content]** från din leveransinnehållssida för att förhandsgranska ditt personliga innehåll.

   ![](assets/sms_send_1.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Add test profile(s)]** om du vill välja en eller flera testprofiler eller profiler.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. I den högra rutan hittar du en förhandsgranskning av SMS-leveransen, där personaliserade element dynamiskt ersätts med data från den valda profilen.

   ![](assets/sms_send_3.png){zoomable="yes"}

Nu kan ni granska och skicka SMS-meddelanden till er målgrupp.

## Testa SMS-leveransen {#test-sms}

Med **Adobe Campaign** kan du testa ett meddelande innan du skickar det till huvudmålgruppen, vilket är ett viktigt steg när det gäller att validera din e-postkampanj och identifiera potentiella problem.

Att skicka in korrektur är ett viktigt steg när det gäller att säkerställa kvaliteten och effektiviteten vid leveransen. Korrekturmottagare kan granska olika element som länkar, avanmälningslänkar och bilder samt identifiera eventuella fel i återgivning, innehåll, personaliseringsinställningar och SMS-konfiguration. Denna process hjälper er att utvärdera och optimera ert SMS noggrant innan ni når er huvudmålgrupp.

![](../assets/do-not-localize/book.png) Lär dig hur du skickar korrektur i [det här avsnittet](../preview-test/test-deliveries.md).

![](assets/sms_send_6.png){zoomable="yes"}

## Skicka SMS-leverans {#send-sms}

1. När du har anpassat SMS-innehållet klickar du på **[!UICONTROL Review & send]** på sidan **[!UICONTROL Delivery]**.

   ![](assets/sms_send_4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Prepare]** och övervaka förloppet och statistiken.

   Om det uppstår några fel hittar du detaljerad information om felet på loggmenyn.

1. Skicka meddelandena genom att klicka på **[!UICONTROL Send]** för att fortsätta med den sista sändningsprocessen.

   ![](assets/sms_send_5.png){zoomable="yes"}

   Om SMS-leveransen har schemalagts klickar du på knappen **[!UICONTROL Send as scheduled]**. Läs mer om leveransplanering i [det här avsnittet](../msg/gs-messages.md#schedule-the-delivery-sending).


1. Bekräfta skicka-åtgärden genom att klicka på knappen **[!UICONTROL Send]**.

När leveransen har skickats kan du spåra dina KPI-data (Key Performance Indicator) från leveranssidan och data på **[!UICONTROL Logs]**-menyn.

Nu kan du börja mäta effekten av ditt meddelande med inbyggda rapporter. [Läs mer](../reporting/sms-report.md)
