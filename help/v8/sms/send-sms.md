---
audience: end-user
title: Skicka SMS-leverans
description: Lär dig hur du skickar SMS med Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Förhandsgranska och skicka en SMS-leverans {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nytt karantänmätvärde"
>abstract="Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras."

## Förhandsgranska SMS-leveransen {#preview-sms}

När du har definierat meddelandeinnehållet kan du använda testprofiler för att förhandsgranska och testa det. Om personaliserat innehåll inkluderas bör du undersöka hur innehållet visas i meddelandet med hjälp av testprofildata. Detta gör att meddelandet visas som det ska och att personaliserad information presenteras korrekt.

De viktigaste stegen för att förhandsgranska SMS-leveransen är följande. Mer information om hur du förhandsgranskar leveranser finns i [det här avsnittet](../preview-test/preview-content.md).

1. Använd **[!UICONTROL Simulate content]** från din leveransinnehållssida för att förhandsgranska ditt personliga innehåll.

   ![Förhandsgranska anpassat SMS-innehåll](assets/sms_send_1.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Add test profile(s)]** om du vill välja en eller flera testprofiler eller profiler.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. I den högra rutan visas en förhandsgranskning av SMS-leveransen, där personaliserade element dynamiskt ersätts med data från den valda profilen.

   ![Förhandsgranskningsfönstret med personlig SMS-leverans](assets/sms_send_3.png){zoomable="yes"}

Granska och skicka SMS-meddelanden till er målgrupp.

## Testa SMS-leveransen {#test-sms}

Testa ett meddelande med **Adobe Campaign** innan du skickar det till huvudmålgruppen. I det här steget valideras din e-postkampanj och potentiella problem identifieras.

Det är viktigt att skicka in korrektur för att säkerställa kvaliteten och effektiviteten vid leveransen. Korrekturmottagare granskar olika element som länkar, avanmälningslänkar och bilder och identifierar eventuella fel i återgivning, innehåll, personaliseringsinställningar och SMS-konfiguration. Denna process utvärderar och optimerar ert SMS noggrant innan ni når er målgrupp.

![Bokikon för att skicka korrektur](../assets/do-not-localize/book.png) Lär dig hur du skickar korrektur i [det här avsnittet](../preview-test/test-deliveries.md).

![Testar SMS-leverans](assets/sms_send_6.png){zoomable="yes"}

## Skicka SMS-leverans {#send-sms}

1. När du har anpassat SMS-innehållet klickar du på **[!UICONTROL Review & send]** på sidan **[!UICONTROL Delivery]**.

   ![Granska och skicka SMS-leverans](assets/sms_send_4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Prepare]** och övervaka förloppet och statistiken.

   Om fel uppstår hittar du detaljerad information om felet på loggmenyn.

1. Skicka meddelandena genom att klicka på **[!UICONTROL Send]** för att fortsätta med den sista sändningsprocessen.

   ![Skickar SMS-leverans](assets/sms_send_5.png){zoomable="yes"}

   Om SMS-leveransen är schemalagd klickar du på knappen **[!UICONTROL Send as scheduled]**. Läs mer om leveransplanering i [det här avsnittet](../msg/gs-messages.md#schedule-the-delivery-sending).

1. Bekräfta skicka-åtgärden genom att klicka på knappen **[!UICONTROL Send]**.

När leveransen har skickats kan du spåra dina KPI-data (Key Performance Indicator) från din leveranssida och data från **[!UICONTROL Logs]**-menyn.

Börja mäta effekten av ert budskap med inbyggda rapporter. [Läs mer](../reporting/sms-report.md)