---
audience: end-user
title: Förbered och skicka ett e-postmeddelande
description: Lär dig hur du förbereder och skickar ett e-postmeddelande med webbgränssnittet i Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: label="Beta"
source-git-commit: 95d44fa2c44a346aad3aab1962e84917532cc966
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 1%

---


# Förbered och skicka e-post {#prepare-send}

## Förbered sändningen {#prepare}

När du har definierat [innehåll](../content/edit-content.md), [publik](../audience/add-audience.md) och schemalägga är du redo att förbereda din e-postleverans.

Under beredningen beräknas målpopulationen och meddelandeinnehållet genereras för varje profil som ingår i målet. När färdigställandet är klart är meddelandena klara att skickas, antingen omedelbart eller vid det schemalagda datumet och den schemalagda tidpunkten.

Valideringsreglerna som används vid leveransförberedelsen beskrivs i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/validate/delivery-analysis.html){target="_blank"}.

De viktigaste stegen för att förbereda sändningen visas nedan.

1. Klicka på **[!UICONTROL Review and send]**.

   ![](assets/email-review-and-send.png)


1. Klicka på **[!UICONTROL Prepare]** i det övre högra hörnet och bekräfta.

   ![](assets/email-prepare.png)

   >[!NOTE]
   >
   >Om du har schemalagt din leverans och inaktiverat **[!UICONTROL Enable confirmation before sending]** kan förberedelse och sändning grupperas tillsammans under **[!UICONTROL Prepare and send]** -knappen. [Läs mer om planering](../email/create-email.md#schedule)

1. Förberedelseförloppet visas. Beroende på storleken på målpopulationen kan den här åtgärden ta en stund.

   Du kan när som helst avbryta beredningen med **[!UICONTROL Stop preparation]** -knappen.

   ![](assets/email-stop-preparation.png)

   >[!NOTE]
   >Under beredningsfasen skickas inga meddelanden. Du kan därför starta eller stoppa detta utan risk för att påverka något.

1. Kontrollera KPI:erna när färdigställandet är klart. Om antalet meddelanden som ska skickas inte matchar dina förväntningar ändrar du målgruppen och startar om förberedelsen.

   ![](assets/email-preparation-complete.png)

   Här visas olika KPI:er:

   * **[!UICONTROL Targeted]**: antalet mottagare.
   * **[!UICONTROL To deliver]**: antalet meddelanden som ska skickas.
   * **[!UICONTROL To exclude]**: antalet meddelanden som utelämnats av en [typologiregel](../advanced-settings/delivery-settings.md#typology).

1. Klicka på **[!UICONTROL Logs]** och kontrollera att det inte finns något fel. I det sista loggmeddelandet visas eventuella felmeddelanden och antalet fel. [Läs mer](delivery-logs.md)

   ![](assets/email-prepare-logs.png)

1. Om ett kritiskt fel upptäcks som förhindrar att leveransen skickas, visas statusen för förberedelsen som misslyckad på kontrollpanelen för leverans.

   ![](assets/email-prepare-error.png)

1. Om du ändrar något efter färdigställandet måste du starta om preparatet för att dessa ändringar ska beaktas.

När färdigställandet är klart utan fel är ditt meddelande klart att skickas.

## Skicka meddelandet {#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Levererat"
>abstract="Antal meddelanden som har levererats. Indikatorn uppdateras var femte minut. Procentandelen som visas baseras på det totala antalet skickade meddelanden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Öppnar"
>abstract="Antalet öppnade meddelanden. Indikatorn uppdateras var femte minut. Procentandelen som visas är förhållandet mellan antalet distinkta öppningar och antalet levererade meddelanden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Klickningar"
>abstract="Antalet mottagare som klickade minst en gång i e-postmeddelandet. Indikatorn uppdateras var femte minut. Procentandelen som visas är förhållandet mellan antalet distinkta klickningar och antalet levererade meddelanden."

När [förberedelse](#prepare) är klar kan du nu skicka ditt e-postmeddelande.

Om meddelandet är schemalagt skickas det vid angivet datum och klockslag. [Läs mer](#schedule-the-send)

### Skicka omedelbart {#send-immediately}

Följ stegen nedan om du vill skicka ett e-postmeddelande omedelbart.

1. Klicka på **[!UICONTROL Send]** i det övre högra hörnet.

   ![](assets/email-send.png)

1. Bekräfta den här åtgärden för att omedelbart skicka meddelandet till huvudmålet.

1. Sändningsförloppet visas.

### Schemalägg sändningen {#schedule-the-send}

Om du har schemalagt ditt e-postmeddelande att skicka det vid ett senare datum och en senare tidpunkt följer du stegen nedan.

1. Innan du trycker **[!UICONTROL Review and send]** ska du kontrollera att du har definierat ett schema för e-postmeddelandet. [Läs mer](../email/create-email.md#schedule)

1. Klicka på **[!UICONTROL Send as scheduled button]** i det övre högra hörnet.

   ![](assets/email-send-as-scheduled.png)

1. Klicka på **[!UICONTROL Confirm sending]**. Leveransen skickas på det schemalagda datumet till huvudmålet.

   >[!NOTE]
   >
   >Om du har inaktiverat **[!UICONTROL Enable confirmation before sending]** kan förberedelse och sändning grupperas tillsammans under **[!UICONTROL Prepare and send]** -knappen. [Läs mer om planering](../email/create-email.md#schedule)

## Pausa eller stoppa sändningen {#pause-stop-sending}

Oavsett om leveransen är schemalagd eller inte kan två åtgärder utföras när som helst under sändningsprocessen:

* Klicka **[!UICONTROL Pause sending]** för att avbryta sändningen av meddelandena. Du kan fortsätta skicka när som helst.

* Klicka **[!UICONTROL Stop sending]** för att omedelbart avbryta sändningen. Varken förberedelsen eller sändningen kan återupptas när den har stoppats.

![](assets/email-send-pause-or-stop.png)

## Kontrollera nyckeltal {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Skickade mått"
>abstract="Totalt antal meddelanden som bearbetats under leveransanalysen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Felmått"
>abstract="Totalt antal fel som sammanställts under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden."

När sändningen är klar kan du kontrollera de nyckeltal som visas:

![](assets/email-send-kpis.png)

* **[!UICONTROL Sent]**: antalet meddelanden som levereras. Procentandelen som visas baseras på det totala antalet meddelanden som ska levereras.

* **[!UICONTROL Delivered]**: antalet meddelanden som har levererats. Procentandelen som visas baseras på det totala antalet skickade meddelanden.

* **[!UICONTROL Opens]**: antalet öppnade meddelanden. Procentandelen som visas är antalet distinkta öppningar jämfört med antalet levererade meddelanden.

* **[!UICONTROL Clicks]**: antalet mottagare som klickade minst en gång i e-postmeddelandet. Den procentandel som visas är antalet distinkta klick jämfört med antalet levererade meddelanden.

* **[!UICONTROL Errors]**: antalet e-postmeddelanden med felstatus. Procentandelen som visas baseras på det totala antalet skickade meddelanden.

>[!NOTE]
>
>Alla indikatorer uppdateras var femte minut efter att leveransen påbörjats. Indikatorerna för leveransförberedelser är i realtid.

Du kan också kontrollera loggarna. [Läs mer](delivery-logs.md)