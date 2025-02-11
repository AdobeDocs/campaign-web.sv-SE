---
audience: end-user
title: Leveransvarningar
description: Lär dig hur du arbetar med leveransvarningar.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Kom igång med leveransvarningar {#gs-delivery-alerting}


Delivery Alerting är ett varningshanteringssystem som gör det möjligt för användargrupper att automatiskt få e-postmeddelanden med information om leveransen. Mottagarna kan övervaka pågående leveranser som bearbetas av Adobe Campaign och vidta lämpliga åtgärder om problem uppstår.

Meddelanden kan anpassas baserat på särskilda varningsvillkor som definieras via Adobe Campaign webbanvändargränssnitt.

Mer information om hur du hanterar leveransfel finns i [Adobe Campaign v8-dokumentationen (konsolen)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}.

## Innehåll i e-postmeddelanden {#content}

E-postmeddelanden innehåller följande avsnitt:

* **Sammanfattning**: Visar antalet leveranser som uppfyller dina definierade villkor, med etiketter och färger för varje villkor.
* **Information**: Visar alla definierade leveransvillkor för instrumentpanelen och motsvarande leveranser för varje kriterium.

![](assets/alerting-email.png)

## Ställ in leveransaviseringar {#set-up}

För att du enklare ska kunna konfigurera de här varningarna kan du skapa och hantera Campaign-webbanvändargränssnittet:

* **Leveransaviseringspaneler**: Ange mottagare, ange aviseringsvillkor som ska inkluderas i instrumentpanelen och få åtkomst till en historik över skickade aviseringar. [Lär dig arbeta med instrumentpaneler](../msg/delivery-alerting-dashboards.md)
* **Leveransvillkor**: Webbanvändargränssnittet för kampanj innehåller fördefinierade varningsvillkor (leveranser med låg genomströmning, leveranser vars förberedelse misslyckades ...) som du kan lägga till på instrumentpanelen. Du kan också skapa egna kriterier som passar dina behov. [Lär dig arbeta med villkor](../msg/delivery-alerting-criteria.md)

Säg att du bara vill meddela användare med administrationsrättigheter om felaktiga leveranser och marknadsföringsanvändare om leveranser med en hög felkvot för mjuk avhoppning. För att uppnå detta skapar du två separata kontrollpaneler med rätt villkor för varje mottagargrupp.

>[!NOTE]
>
>Om du vill få åtkomst till och konfigurera kontrollpaneler och aviseringsvillkor måste du ha **administrationsbehörighet** eller vara en del av säkerhetsgruppen **Leveransövervakare**. Standardanvändare har inte åtkomst till instrumentpaneler i Adobe Campaign-gränssnittet, men kan få varningsmeddelanden. [Läs mer om åtkomst och behörigheter](../get-started/permissions.md)
