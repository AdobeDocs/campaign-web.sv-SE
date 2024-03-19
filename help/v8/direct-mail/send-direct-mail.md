---
audience: end-user
title: Förhandsgranska och skicka direktreklam
description: Lär dig hur du förhandsgranskar och skickar direktreklam via Adobe Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---


# Förhandsgranska och skicka direktreklam {#send-direct-mail}

När du har konfigurerat extraheringsfilen för direktutskick kan du använda testprofiler för att förhandsgranska den. Om du har inkluderat anpassat innehåll kan du undersöka hur det här innehållet visas i kolumnerna med hjälp av testprofildata. På så sätt kan du se till att filinnehållet återges korrekt och att de anpassade elementen införlivas på rätt sätt.

När extraheringsfilen är klar kan du skicka den direkt för att generera filen och dela den med din direktreklamleverantör. [Lär dig hur du skickar direktreklam](#dm-send)

## Förhandsgranska extraheringsfilen {#preview-dm}

De viktigaste stegen för att förhandsgranska extraheringsfilen är följande. Mer information om hur du förhandsgranskar leveranser finns i [det här avsnittet](../preview-test/preview-content.md).

1. Använd **[!UICONTROL Simulate content]** för att förhandsgranska ditt personaliserade innehåll.

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. Klicka **[!UICONTROL Add test profile(s)]** om du vill markera en eller flera profiler för att förhandsvisa deras data i extraheringsfilens innehåll.

1. I den högra rutan hittar du en förhandsgranskning av extraheringsfilen, där personaliserade element dynamiskt ersätts med data från den valda profilen.

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## Skicka korrektur {#test-dm}

Använda **Adobe Campaign** kan du skicka korrektur innan du skickar dem till huvudmålgruppen. Det här steget är viktigt när du ska validera leveransen och identifiera eventuella problem. Testmottagarna kan granska element som personaliseringsinställningar, säkerställa optimala prestanda och upptäcka eventuella fel. Med den här processen kan du förfina och optimera extraheringsfilen innan du når huvudmålgruppen.

För direktutskick genereras ett prov av extraheringsfilen med hjälp av data från de valda testprofilerna när du skickar korrektur. Så här öppnar du den:

1. På skärmen för att simulera innehåll klickar du på **[!UICONTROL Send proof]** och följer samma steg som för alla typer av leveranser för att skicka ett bevis. [Lär dig hur du skickar korrektur](../preview-test/test-deliveries.md)

1. När beviset har skickats kan du öppna det från **[!UICONTROL View proofs]** eller från leveranslistan. [Lär dig hur du får åtkomst till skickade korrektur](../preview-test/test-deliveries.md#access-test-deliveries)

1. På kontrollpanelen klickar du på **[!UICONTROL Preview file]** för att få tillgång till en förhandsgranskning av extraheringsfilen.

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Endast de första 100 raderna visas i förhandsvisningsfilen.

## Skicka direktmejl {#send-dm}

När du är klar att skicka direktreklam till dina kunder kan du skicka leveransen för att påbörja dataextraheringen i den angivna extraheringsfilen. Följ dessa steg för att göra detta:

1. När du har utformat innehållet i extraheringsfilen klickar du på **[!UICONTROL Review & send]** från **[!UICONTROL Delivery]** sida.

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. Klicka **[!UICONTROL Prepare]** och övervaka framstegen och statistiken.

   Om några fel inträffar, se **[!UICONTROL Logs]** om du vill ha detaljerad information om felet.

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. Skicka meddelandena genom att klicka på **[!UICONTROL Send]** för att fortsätta med den slutliga sändningsprocessen.

1. Bekräfta skicka-åtgärden genom att klicka på knappen **[!UICONTROL Send]**.

   Om direktleveransen har schemalagts klickar du på **[!UICONTROL Send as scheduled]** -knappen. Läs mer om leveransplanering i [det här avsnittet](../msg/gs-messages.md#schedule-the-delivery-sending).

När leveransen har skickats genereras extraheringsfilen automatiskt och exporteras till den plats som anges i **[!UICONTROL Routing]** externt konto som valts i leveransmallens [avancerade inställningar](../advanced-settings/delivery-settings.md).

Du kan spåra dina KPI-data (Key Performance Indicator) från leveranssidan och data från **[!UICONTROL Logs]** -menyn.

Du kan också börja mäta effekten av ditt meddelande med inbyggda rapporter. [Läs mer](../reporting/direct-mail.md)