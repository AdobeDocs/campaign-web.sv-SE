---
audience: end-user
title: Kom igång med externa leveranser
description: Lär dig skapa och skicka externa leveranser med Adobe Campaign Web
exl-id: 08fe9333-aa35-4acf-ba41-4c6895049bbc
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Skicka externa leveranser {#gs-direct-mail}


Med Adobe Campaign kan ni hantera leveranser som skapats utanför Campaign för att massleverera personaliserade e-postmeddelanden, SMS-meddelanden eller push-meddelanden (iOS och Android) via ett externt system.

<!--The supported channels are Email, Mobile (SMS), and Push (iOs and Android).-->

När du skapar en extern leverans genererar Adobe Campaign automatiskt en extraheringsfil som innehåller alla målprofiler och valda data. Den här filen skickas till den server som du väljer och som kommer att hantera sändningsprocessen åt dig.

## Skapa ett dedikerat externt konto {#routing-external-account}

Du måste först konfigurera ett specifikt externt konto som ska användas i dina externa leveranser. Det måste vara av typen **[!UICONTROL Routing]**.

>[!NOTE]
>
>Lär dig hur du skapar ett externt konto av routningstyp i [det här avsnittet](../administration/external-account.md#routing).

Välj till exempel kanalen **[!UICONTROL Mobile (SMS)]** för det externa kontot. **[!UICONTROL External]** är markerat som standard som **[!UICONTROL Delivery mode]**.

![](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## Skapa och skicka extern leverans {#create-external-delivery}

När det specifika externa kontot har konfigurerats skapar du den externa leveransen. Följ stegen nedan.

1. Skapa en leverans. [Lär dig hur](create-deliveries.md)

   Du har tre alternativ:

   * **I ett arbetsflöde**: Lägg till en extern kanalaktivitet (e-post, SMS eller push) i arbetsflödet. Detaljerade instruktioner om hur du konfigurerar arbetsflödet finns på [den här sidan](../workflows/gs-workflow-creation.md).
   * **I en kampanj**: När du har skapat en kampanj kan du skapa en extern leverans via e-post, SMS eller push-kanal. Mer information om hur du konfigurerar kampanjen finns på [den här sidan](../campaigns/gs-campaigns.md).
   * **Fristående leverans**: Engagera kunderna direkt och direkt med en extern leverans. [Lär dig skapa en leverans](../msg/gs-deliveries.md)

1. I leverans- eller leveransmallen [settings](../advanced-settings/delivery-settings.md) väljer du det externa konto som du skapade för den kanal du vill använda (i det här exemplet SMS-kanalen) och sparar.

   ![](assets/external-delivery-routing.png){zoomable="yes"}

   >[!NOTE]
   >
   >Om du skapar en leverans måste du se till att du har valt en [leveransmall](delivery-template.md) med ett externt konto av typen **[!UICONTROL Routing]**, annars kan du inte välja det dedikerade konto du har skapat [ ovan](#routing-external-account).

1. Klicka på **[!UICONTROL Edit content]** i avsnittet **[!UICONTROL Content]**.

   ![](assets/external-delivery-edit-content.png){zoomable="yes"}

1. Till skillnad från en standardleverans utformar du inte själva meddelandets innehåll. I stället måste du definiera egenskaper och kolumner för filen som ska skickas till det externa systemet.

   ![](assets/external-delivery-file-properties.png){zoomable="yes"}

   Följ samma steg som när du utformar innehållet i extraheringsfilen som genereras av [direktutskick](../direct-mail/content-direct-mail.md):

   * Definiera egenskaperna för extraheringsfilen. [Läs mer](../direct-mail/content-direct-mail.md#properties)
   * Markera kolumnerna som innehåller den information som ska exporteras till filen. [Läs mer](../direct-mail/content-direct-mail.md#content)

1. Du kan förhandsgranska filen och skicka korrektur <!--not in UI right now - to check-->. [Lär dig hur](../direct-mail/send-direct-mail.md#preview-dm)

   ![](assets/external-delivery-simulate.png){zoomable="yes"}

1. Skicka leveransen för att generera extraheringsfilen. [Lär dig hur](../direct-mail/send-direct-mail.md#send-dm)

När leveransen har skickats genereras extraheringsfilen automatiskt och exporteras till den plats som anges i det [externa kontot](../administration/external-account.md#create-ext-account) som har valts i leveransmallens inställningar.

Du kan spåra KPI:er från leveranssidan och data på menyn **[!UICONTROL Logs]**.
