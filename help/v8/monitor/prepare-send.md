---
audience: end-user
title: Förbered och skicka ett e-postmeddelande
description: Lär dig hur du förbereder och skickar ett e-postmeddelande med webbgränssnittet i Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 0%

---

# Förbered och skicka e-post {#prepare-send}

## Förbered sändningen {#prepare}

När du definierar ditt [innehåll](../email/edit-content.md), [målgrupp](../audience/add-audience.md) och [schema](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule) kan du förbereda din e-postleverans.

Under leveransförberedelsen beräknas målpopulationen och meddelandeinnehållet genereras för varje profil som ingår i målet. När färdigställandet är klart är meddelandena klara att skickas, antingen omedelbart eller vid det schemalagda datumet och den schemalagda tidpunkten.

Verifieringsreglerna som används vid leveransförberedelsen beskrivs i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html?lang=sv-SE){target="_blank"}.

De viktigaste stegen för att förbereda sändningen visas nedan.

1. Klicka på **[!UICONTROL Review and send]** på kontrollpanelen för leverans.

   ![Granska och skicka-knappen på kontrollpanelen för leverans](assets/email-review-and-send.png){zoomable="yes"}

1. Klicka på knappen **[!UICONTROL Prepare]** i det övre högra hörnet och bekräfta.

   ![Förbered-knappen på kontrollpanelen för leverans](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >Om du schemalägger leveransen och inaktiverar alternativet **[!UICONTROL Enable confirmation before sending]** grupperas förberedelsestegen och sändningsstegen under knappen **[!UICONTROL Prepare and send]**. [Läs mer om schemaläggning](../msg/gs-deliveries.md#gs-schedule)

1. Förberedelseförloppet visas. Beroende på storleken på målpopulationen kan den här åtgärden ta en stund.

   Du kan när som helst stoppa förberedelsen med knappen **[!UICONTROL Stop preparation]**.

   ![Stoppa förberedelseknappen på kontrollpanelen för leverans](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >Under beredningsfasen skickas inga meddelanden. Du kan starta eller stoppa detta utan risk för att påverka någonting.

1. Kontrollera KPI:erna när beredningen är klar. Om antalet meddelanden som ska skickas inte matchar dina förväntningar ändrar du målgruppen och startar om förberedelsen.

   ![Förberedelser för helskärm med KPI:er](assets/email-preparation-complete.png){zoomable="yes"}

   Här visas olika KPI:er:

   * **[!UICONTROL Targeted]**: antalet mottagare.
   * **[!UICONTROL To deliver]**: antalet meddelanden som ska skickas.
   * **[!UICONTROL To exclude]**: antalet meddelanden som utelämnats av en [typologiregel](../advanced-settings/delivery-settings.md#typology).

1. Klicka på knappen **[!UICONTROL Logs]** och kontrollera att det inte finns några fel. I det sista loggmeddelandet visas eventuella felmeddelanden och antalet fel. [Läs mer](delivery-logs.md)

   ![Knappen Loggar på kontrollpanelen för leverans](assets/email-prepare-logs.png){zoomable="yes"}

1. Om ett kritiskt fel upptäcks som förhindrar att leveransen skickas, visas statusen för förberedelsen som misslyckad på kontrollpanelen för leverans.

   ![Felstatus på kontrollpanelen för leverans](assets/email-prepare-error.png){zoomable="yes"}

1. Om du ändrar något efter färdigställandet, ska du starta om preparatet för att ta hänsyn till dessa ändringar.

När färdigställandet är klart utan fel är ditt meddelande klart att skickas.

## Skicka meddelandet {#send}

När [förberedelsen](#prepare) är klar kan du skicka ditt e-postmeddelande.

Om meddelandet är schemalagt skickas det vid angivet datum och tid. [Läs mer om schemaläggning](../msg/gs-deliveries.md#gs-schedule)

### Skicka omedelbart {#send-immediately}

Följ stegen nedan om du vill skicka ett e-postmeddelande omedelbart.

1. Klicka på knappen **[!UICONTROL Send]** i det övre högra hörnet på kontrollpanelen för leverans.

   ![Skicka-knappen på kontrollpanelen för leverans](assets/email-send.png){zoomable="yes"}

1. Bekräfta den här åtgärden för att omedelbart skicka meddelandet till huvudmålet.

1. Sändningsförloppet visas.

### Schemalägg sändning {#schedule-the-send}

Om du schemalägger ditt e-postmeddelande att skicka det vid ett senare datum och en senare tidpunkt följer du stegen nedan.

1. Innan du klickar på knappen **[!UICONTROL Review and send]** måste du definiera ett schema för e-postmeddelandet. [Läs mer om schemaläggning](../msg/gs-deliveries.md#gs-schedule)

1. Klicka på **[!UICONTROL Send as scheduled button]** i det övre högra hörnet på kontrollpanelen för leverans.

   ![Skicka som schemalagd knapp på kontrollpanelen för leverans](assets/email-send-as-scheduled.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Confirm sending]**. Leveransen skickas på det schemalagda datumet till huvudmålet.

   >[!NOTE]
   >
   >Om du inaktiverar alternativet **[!UICONTROL Enable confirmation before sending]** grupperas förberedelsen och skickastegen tillsammans under knappen **[!UICONTROL Prepare and send]**. [Läs mer om schemaläggning](../msg/gs-deliveries.md#gs-schedule)

## Pausa eller stoppa sändningen {#pause-stop-sending}

Oavsett om din leverans är schemalagd eller inte<!--TBC--> kan två åtgärder utföras när som helst under sändningsprocessen:

* Klicka på **[!UICONTROL Pause sending]** om du vill avbryta sändningen av meddelandena. Du kan fortsätta skicka när som helst.

* Klicka på **[!UICONTROL Stop sending]** för att omedelbart avbryta sändningen. Varken förberedelsen eller sändningen kan återupptas när den har stoppats.

![Pausa eller stoppa sändning av knappar på kontrollpanelen för leverans](assets/email-send-pause-or-stop.png){zoomable="yes"}

## Kontrollera nyckeltal {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Levererat"
>abstract="Antal meddelanden som har levererats. Indikatorn uppdateras var femte minut. Procentandelen som visas baseras på det totala antalet skickade meddelanden."
>additional-url="https://experienceleague.adobe.com/sv/docs/campaign-web/v8/reports/kpis" text="Förstå nyckeltal"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Öppnar"
>abstract="Antalet öppnade meddelanden. Indikatorn uppdateras var femte minut. Procentandelen som visas är förhållandet mellan antalet distinkta öppningar och antalet levererade meddelanden."
>additional-url="https://experienceleague.adobe.com/sv/docs/campaign-web/v8/reports/kpis" text="Förstå nyckeltal"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Klickningar"
>abstract="Antalet mottagare som klickat minst en gång i e-postmeddelandet. Indikatorn uppdateras var femte minut. Procentandelen som visas är förhållandet mellan antalet distinkta klickningar och antalet levererade meddelanden."
>additional-url="https://experienceleague.adobe.com/sv/docs/campaign-web/v8/reports/kpis" text="Förstå nyckeltal"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Skickat"
>abstract="Totalt antal meddelanden som bearbetats under leveransanalysen."
>additional-url="https://experienceleague.adobe.com/sv/docs/campaign-web/v8/reports/kpis" text="Förstå nyckeltal"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Fel"
>abstract="Totalt antal fel som sammanställts under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden."
>additional-url="https://experienceleague.adobe.com/sv/docs/campaign-web/v8/reports/kpis" text="Förstå nyckeltal"

När sändningen är klar kan du kontrollera de nyckeltal som visas:

![KPI:er visas efter sändning](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL Sent]**: antalet meddelanden som levereras. Procentandelen som visas baseras på det totala antalet meddelanden som ska levereras.

* **[!UICONTROL Delivered]**: antalet meddelanden som har levererats. Procentandelen som visas baseras på det totala antalet skickade meddelanden.

* **[!UICONTROL Opens]**: antalet öppnade meddelanden. Procentandelen som visas är antalet distinkta öppningar jämfört med antalet levererade meddelanden.

* **[!UICONTROL Clicks]**: antalet mottagare som klickade minst en gång i e-postmeddelandet. Den procentandel som visas är antalet distinkta klick jämfört med antalet levererade meddelanden.

* **[!UICONTROL Errors]**: antalet e-postmeddelanden med felstatus. Procentandelen som visas baseras på det totala antalet skickade meddelanden.

>[!NOTE]
>
>Alla indikatorer uppdateras var femte minut efter att leveransen påbörjats. Indikatorerna för leveransförberedelser är i realtid.

Läs mer om KPI:er på [den här sidan](../reporting/kpis.md).

Du kan också kontrollera loggarna. [Läs mer](delivery-logs.md)