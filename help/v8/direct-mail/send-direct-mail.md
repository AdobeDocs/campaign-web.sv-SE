---
audience: end-user
title: Förhandsgranska och skicka direktreklam
description: Lär dig hur du förhandsgranskar och skickar direktreklam via Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# Förhandsgranska och skicka direktreklam {#send-direct-mail}

När du har konfigurerat extraheringsfilen för direktutskick kan du använda testprofiler för att förhandsgranska den. Om du har inkluderat anpassat innehåll kan du undersöka hur det här innehållet visas i kolumnerna med hjälp av testprofildata. På så sätt kan du se till att filinnehållet återges korrekt och att de anpassade elementen införlivas på rätt sätt.

När extraheringsfilen är klar kan du skicka den direkt för att generera filen och dela den med din direktreklamleverantör. [Lär dig hur du skickar direktreklam](#dm-send)

## Förhandsgranska extraheringsfilen {#preview-dm}

De viktigaste stegen för att förhandsgranska extraheringsfilen är följande. Mer information om hur du förhandsgranskar leveranser finns i [det här avsnittet](../preview-test/preview-content.md).

1. Använd **[!UICONTROL Simulate content]** från din leveransinnehållssida för att förhandsgranska ditt personliga innehåll.

   ![](assets/dm-simulate.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Add test profile(s)]** om du vill välja en eller flera profiler för att förhandsgranska deras data i extraheringsfilens innehåll.

1. I den högra rutan hittar du en förhandsgranskning av extraheringsfilen, där personaliserade element dynamiskt ersätts med data från den valda profilen.

   ![](assets/dm-preview-right.png){zoomable="yes"}

## Skicka korrektur {#test-dm}

Med **Adobe Campaign** kan du skicka korrektur innan du skickar dem till huvudmålgruppen. Det här steget är viktigt när du ska validera leveransen och identifiera eventuella problem. Testmottagarna kan granska element som personaliseringsinställningar, säkerställa optimala prestanda och upptäcka eventuella fel. Med den här processen kan du förfina och optimera extraheringsfilen innan du når huvudmålgruppen.

För direktutskick genereras ett prov av extraheringsfilen med hjälp av data från de valda testprofilerna när du skickar korrektur. Så här öppnar du den:

1. Klicka på knappen **[!UICONTROL Send proof]** på skärmen för att simulera innehåll och följ samma steg som för alla typer av leveranser för att skicka ett korrektur. [Lär dig skicka korrektur](../preview-test/test-deliveries.md)

1. När korrekturet har skickats kan du komma åt det från knappen **[!UICONTROL View proofs]** eller från leveranslistan. [Lär dig hur du får åtkomst till skickade korrektur](../preview-test/test-deliveries.md#access-test-deliveries)

1. Klicka på knappen **[!UICONTROL Preview file]** på kontrollpanelen för att öppna en förhandsgranskning av extraheringsfilen.

   ![](assets/dm-proof.png){zoomable="yes"}

   >[!NOTE]
   >
   >Endast de första 100 raderna visas i förhandsvisningsfilen.

## Skicka direktmejl {#send-dm}

När du är klar att skicka direktreklam till dina kunder kan du skicka leveransen för att påbörja dataextraheringen i den angivna extraheringsfilen. Följ dessa steg för att göra detta:

1. När du har utformat innehållet i extraheringsfilen klickar du på **[!UICONTROL Review & send]** på sidan **[!UICONTROL Delivery]**.

   ![](assets/dm-review-send.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Prepare]** och övervaka förloppet och statistiken.

   Om det uppstår några fel hittar du detaljerad information om felet på **[!UICONTROL Logs]**-menyn.

   ![](assets/dm-prepare.png){zoomable="yes"}

1. Skicka meddelandena genom att klicka på **[!UICONTROL Send]** för att fortsätta med den sista sändningsprocessen.

1. Bekräfta skicka-åtgärden genom att klicka på **[!UICONTROL Send]**.

   Om direktmeddelandeleveransen har schemalagts klickar du på knappen **[!UICONTROL Send as scheduled]**. Läs mer om leveransplanering i [det här avsnittet](../msg/gs-messages.md#schedule-the-delivery-sending).

När leveransen har skickats genereras extraheringsfilen automatiskt och exporteras till den plats som anges i det **[!UICONTROL Routing]** externa kontot som valts i leveransmallens [avancerade inställningar](../advanced-settings/delivery-settings.md).

Du kan spåra dina KPI-data (Key Performance Indicator) från din leveranssida och dina data från **[!UICONTROL Logs]**-menyn.

Du kan också börja mäta effekten av ditt meddelande med inbyggda rapporter. [Läs mer](../reporting/direct-mail.md)
