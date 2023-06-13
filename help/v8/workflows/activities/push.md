---
audience: end-user
title: Använd aktiviteten för push-meddelandearbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten för push-meddelanden
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# Push-meddelande {#push-activity}

The **Push-meddelande** Med leveransaktivitet kan du konfigurera sändning av push-meddelanden i ett arbetsflöde.

>[!BEGINTABS]

>[!TAB Push-meddelande (Android)]

1. När du har skapat och konfigurerat ett nytt arbetsflöde lägger du till en Build-målgruppsaktivitet för att välja en befintlig målgrupp eller använder regelbyggaren för att definiera en egen fråga.

1. Lägg till en kanalaktivitet för push-meddelanden (Android) i arbetsflödet.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Välj aktivitet. På leveransmenyn väljer du de mallar som du vill använda för leveransen. Läs mer om mallar

1. Klicka på Skapa leverans för att konfigurera leveransen av push-meddelanden. Mer information om push-meddelanden (Android) finns på den här sidan.

1. När leveransen är klar går du tillbaka till arbetsflödet och klickar på Start för att starta arbetsflödet.

1. Som standard utlöses meddelandeförberedelsefasen när ett leveransarbetsflöde initieras, utan att meddelandet skickas omedelbart.

   Klicka på Granska och skicka på den avancerade menyn i din Push-meddelandekanalsaktivitet (Android) för att bekräfta sändningen.

1. Klicka på Skicka på kontrollpanelen för push-meddelandeleverans.

>[!TAB Push-meddelande (iOS)]

1. När du har skapat och konfigurerat ett nytt arbetsflöde lägger du till en Build-målgruppsaktivitet för att välja en befintlig målgrupp eller använder regelbyggaren för att definiera en egen fråga.

1. Lägg till en kanalaktivitet för push-meddelanden (iOS) i arbetsflödet.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Välj aktivitet. På leveransmenyn väljer du de mallar som du vill använda för leveransen. Läs mer om mallar

1. Klicka på Skapa leverans för att konfigurera leveransen av push-meddelanden. Mer information om push-meddelanden (iOS) finns på den här sidan.

1. När leveransen är klar går du tillbaka till arbetsflödet och klickar på Start för att starta arbetsflödet.

1. Som standard utlöses meddelandeförberedelsefasen när ett leveransarbetsflöde initieras, utan att meddelandet skickas omedelbart.

   Klicka på Granska och skicka på den avancerade menyn i din kanalaktivitet för push-meddelanden (iOS) för att bekräfta sändningen.

1. Klicka på Skicka på kontrollpanelen för push-meddelandeleverans.

>[!ENDTABS]