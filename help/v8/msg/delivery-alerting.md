---
audience: end-user
title: Leveransvarningar
description: Lär dig hur du arbetar med leveransvarningar.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 037b04475370b1a34ecec31ef2a774866278ce65
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Kom igång med leveransvarningar {#gs-delivery-alerting}

Leveransvarningar är ett varningshanteringssystem som gör det möjligt för användargrupper att automatiskt få e-postmeddelanden med information om leveransen. Mottagarna övervakar pågående leveranser som bearbetas av Adobe Campaign och vidtar lämpliga åtgärder om problem uppstår.

Meddelanden anpassas baserat på särskilda varningsvillkor som definieras via Adobe Campaign webbanvändargränssnitt.

Mer information om hur du hanterar leveransfel finns i [Adobe Campaign v8-dokumentationen (konsolen)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}.

## Innehåll i e-postmeddelanden {#content}

E-postmeddelanden innehåller följande avsnitt:

* **Sammanfattning**: Visar antalet leveranser som uppfyller dina definierade villkor, med etiketter och färger för varje villkor.
* **Information**: Visar alla definierade leveransvillkor för instrumentpanelen och motsvarande leveranser för varje kriterium.

![Beskrivning: I den här skärmbilden visas e-postmeddelandets layout, inklusive sammanfattnings- och informationsavsnitten.](assets/alerting-email.png)

## Ställ in leveransaviseringar {#set-up}

Om du vill konfigurera de här varningarna kan du skapa och hantera Campaign-webbgränssnittet:

* **Leveransaviseringspaneler**: Ange mottagare, ange aviseringsvillkor som ska inkluderas i instrumentpanelen och få åtkomst till en historik över skickade aviseringar. [Lär dig arbeta med instrumentpaneler](../msg/delivery-alerting-dashboards.md).
* **Leveransaviseringskriterier**: Campaign-webbanvändargränssnittet innehåller fördefinierade aviseringskriterier, till exempel leveranser med låg genomströmning eller leveranser vars förberedelse misslyckades. Du kan lägga till dessa villkor på din kontrollpanel eller skapa egna kriterier som passar dina behov. [Lär dig arbeta med villkor](../msg/delivery-alerting-criteria.md).

Meddela t.ex. användare med administrationsrättigheter endast om felaktiga leveranser utförts och meddela marknadsföringsanvändare om leveranser med en hög felkvot för mjuk avhoppning. För att uppnå detta skapar du två separata kontrollpaneler med rätt villkor för varje mottagargrupp.

>[!NOTE]
>
>Om du vill få åtkomst till och konfigurera kontrollpaneler och aviseringsvillkor måste du ha **administrationsbehörighet** eller vara en del av säkerhetsgruppen **Leveransövervakare**. Standardanvändare har inte åtkomst till instrumentpaneler i Adobe Campaign-gränssnittet, men kan få varningsmeddelanden. [Läs mer om åtkomst och behörigheter](../get-started/permissions.md).