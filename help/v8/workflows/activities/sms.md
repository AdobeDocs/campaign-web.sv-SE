---
audience: end-user
title: Använd SMS-arbetsflödesaktiviteten
description: Lär dig hur du använder SMS-arbetsflödesaktiviteten
badge: label="Alpha" type="Positive"
source-git-commit: c0e5902d3ee504aa5aa4e55f18416facfe4020b1
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 1%

---


# SMS {#sms}

The **SMS** -aktiviteten tillhandahåller funktioner för att skicka SMS-meddelanden i ett arbetsflöde. Det möjliggör automatisering av SMS-utskick till ett specifikt mål som fastställs i samma arbetsflöde.

Om du vill definiera mottagare av SMS kan du konfigurera dem före SMS-leveransaktiviteten i arbetsflödet med hjälp av aktiviteten Skapa målgrupp. Läs mer.

1. När du har skapat och konfigurerat ett nytt arbetsflöde lägger du till en Build-målgruppsaktivitet för att välja en befintlig målgrupp eller använder regelbyggaren för att definiera en egen fråga.

1. Lägg till en SMS-kanalaktivitet i arbetsflödet.

   ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. Välj aktivitet. På leveransmenyn väljer du de mallar som du vill använda för leveransen. Läs mer om mallar

1. Klicka på Skapa leverans för att konfigurera SMS-leveransen. Mer information om SMS-leverans finns på den här sidan.

1. När leveransen är klar går du tillbaka till arbetsflödet och klickar på Start för att starta arbetsflödet.

1. Som standard utlöses meddelandeförberedelsefasen när ett leveransarbetsflöde initieras, utan att meddelandet skickas omedelbart.

   Klicka på Granska och skicka på den avancerade menyn i SMS-aktiviteten för att bekräfta sändningen.

1. Klicka på Skicka på kontrollpanelen för SMS-leverans.
