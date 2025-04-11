---
audience: end-user
title: Schemalägg sändning av leverans
description: Lär dig schemalägga en leverans
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Schemalägg sändning av leverans {#schedule-sending}

Du kan schemalägga sändning av en leverans. Stegen beror på om det är en fristående leverans (en bild) eller om du arbetar i ett kampanjarbetsflöde.

## Fristående leverans

För fristående leveranser, schemalägg datum och tid direkt i leveransen. Se exempel nedan för varje typ av leverans: e-post, SMS och push-meddelanden.

### E-post {#schedule-email-standalone}

Så här schemalägger du sändning av e-postmeddelanden:

1. Aktivera alternativet **[!UICONTROL Enable scheduling]** i avsnittet **[!UICONTROL Schedule]** i leveransegenskaperna.

1. Ange önskat datum och tid för sändning och klicka på knappen **[!UICONTROL Review and send]**.

   ![Aktivera schemaläggning och ange datum och tid](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>Som standard är alternativet **[!UICONTROL Enable confirmation before sending]** aktiverat. Det här alternativet kräver att du bekräftar att leveransen ska skickas innan det schemalagda datumet och den schemalagda tidpunkten. Om du behöver skicka leveransen automatiskt på det schemalagda datumet och den schemalagda tidpunkten inaktiverar du det här alternativet.
>

1. Kontrollera att schemat är korrekt och klicka på knappen **[!UICONTROL Prepare]**.

![Kontrollera schema och förbered leverans](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. När färdigställandet är klart är meddelanden klara att skickas. Nyckeltal för leveransen visas, inklusive den totala målpopulationen, antalet meddelanden som ska levereras och antalet uteslutna mottagare. Klicka på knappen **[!UICONTROL Send as scheduled]** för att bekräfta att leveransen kommer att skickas på det schemalagda datumet och den schemalagda tiden till huvudmålet.

![Bekräfta sändning enligt schema](assets/schedule-email-standalone-send.png){zoomable="yes"}

### SMS

Följ samma steg som för e-postleveranser om du vill schemalägga SMS-leveransen för ett visst datum och en viss tid. [Se ovan](#schedule-email-standalone).

![Schemalägg SMS-leverans](assets/schedule-sms-standalone.png){zoomable="yes"}

Du kan även kontrollera att schemat används:

![Kontrollera SMS-schema](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### Push-meddelande

Om du vill schemalägga en fristående push-leverans för ett visst datum och en viss tid följer du samma steg som för e-postleveranser. [Se ovan](#schedule-email-standalone).

![Schemalägg leverans av push-meddelanden](assets/schedule-push-standalone.png){zoomable="yes"}

Du kan även kontrollera att schemat används:

![Kontrollera push-meddelandeschema](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### Fristående leverans i en kampanj

Du kan skapa en fristående leverans inom en kampanj utan att använda ett arbetsflöde. Ställ in datum- och tidsplanen för den här leveransen enligt ovan. Kampanjen kan ha ett eget schema, inklusive ett startdatum och ett slutdatum. Det här schemat påverkar inte ditt leveransschema.

![Fristående leverans i en kampanj](assets/schedule-delivery-standalone.png){zoomable="yes"}

## Schemalägg en leverans i ett kampanjarbetsflöde

I ett kampanjarbetsflöde är det bästa sättet att använda aktiviteten **[!UICONTROL Scheduler]** för att använda ett datum och en tid för att starta arbetsflödet, vilket innebär att leveransen skickas. [Läs mer om Schemaläggaren](../workflows/activities/scheduler.md).

![Schemalägg leverans i ett kampanjarbetsflöde](assets/schedule-workflow.png){zoomable="yes"}

Konfigurera datum och tid i aktiviteten **[!UICONTROL Scheduler]**.

![Konfigurera schemaläggningsaktivitet](assets/schedule-workflow-scheduler.png){zoomable="yes"}

>[!NOTE]
>
>När du använder aktiviteten **[!UICONTROL Scheduler]** för att schemalägga sändning av leverans i ett arbetsflöde ska du inte aktivera **[!UICONTROL Enable scheduling]**-växeln i aktivitetsinställningarna för **[!UICONTROL Delivery]**. Leveransen skickas automatiskt.
>

Om du aktiverar växeln **[!UICONTROL Enable scheduling]** i aktivitetsinställningarna för **[!UICONTROL Delivery]** och ställer in ett datum och en tid där, väntar leveransen på att skickas på detta datum och denna tid. Det innebär att om det är en fördröjning mellan arbetsflödets startdatum och sändningsdatumet kanske målgruppen inte är uppdaterad.