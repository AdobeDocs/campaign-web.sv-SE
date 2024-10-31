---
audience: end-user
title: Leveransavisering
description: Lär dig arbeta med leveransaviseringar.
exl-id: b91ef82b-f3e9-4704-87a2-0e3f75104572
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# Kontrollpaneler för leveransaviseringar {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Kontrollpaneler för leveransvarningar"
>abstract="Leveransavisering är ett aviseringshanteringssystem som gör det möjligt för användargrupper att automatiskt få e-postmeddelanden med information om leveranskörningar. Kontrollpaneler för leveransaviseringar låter dig ange vem som ska ta emot e-postaviseringar, välja och konfigurera aviseringsvillkor som ska användas för att skicka dessa aviseringar och få åtkomst till historiken för alla skickade aviseringar."

Kontrollpaneler för leveransaviseringar låter dig ange vem som ska ta emot e-postaviseringar, välja och konfigurera aviseringsvillkor som ska användas för att skicka dessa aviseringar och få åtkomst till historiken för alla skickade aviseringar. De är tillgängliga från menyn **Leveransavisering** i det vänstra navigeringsfönstret under fliken **Instrumentpaneler**.

![](assets/alerting-dashboard-list.png)

## Skapa en leveranstavla {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Skapa tavla för leveransaviseringar"
>abstract="Om du skapar en kontrollpanel för leveransavisering kan du ange vem som ska ta emot e-postaviseringar, välja och konfigurera aviseringsvillkor som ska användas för att skicka dessa aviseringar och visa historiken för alla skickade aviseringar."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Allmänna parametrar för leveransaviseringar"
>abstract="Ange allmänna egenskaper för kontrollpanelen för leveransaviseringar. Fältet **Välj aviseringsgrupp** gör att du kan ange operatörsgruppen **** för att ta emot aviseringar som skickas från den här instrumentpanelen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Kriterier för leveransavisering"
>abstract="I det här avsnittet lägger du till villkor som du vill använda för att skicka aviseringar från den här kontrollpanelen. Välj bland fördefinierade kriterier eller skapa egna kriterier som anpassas efter specifika behov."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Kriterieparametrar"
>abstract="Kriterierna har standardparametervärden som definierar hur de måste tillämpas. I det här avsnittet kan du ändra dessa värden så att de passar dina behov."

Så här skapar du en kontrollpanel för leverans:

1. Navigera till menyn **Leveransvarning** i den vänstra navigeringsrutan och klicka på **Skapa leveransinstrumentpanel**.

   ![](assets/alerting-dashboard.png)

1. Namnge instrumentpanelen i fältet **Etikett**. Fältet **Internt namn** fylls i automatiskt och är skrivskyddat.

1. I fältet **Välj aviseringsgrupp** anger du den **operatörsgrupp** som ska ta emot aviseringar som skickas från den här instrumentpanelen. Alla medlemmar i den valda operatörsgruppen kommer att få varningarna.

   Läs mer om behörigheter och operatörsgrupper i [Adobe Campaign v8-dokumentationen (konsol)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. I avsnittet **Leveransaviseringsvillkor** lägger du till villkor som du vill använda för att skicka aviseringar. Välj bland fördefinierade kriterier eller skapa egna kriterier som passar in efter specifika behov. [Lär dig arbeta med villkor](../msg/delivery-alerting-criteria.md)

1. Kriterierna har standardparametervärden som definierar hur de ska användas. Du kan ändra de här värdena så att de passar dina behov från avsnittet **Parametrar för kriterier**.

   ![](assets/alerting-criteria-parameters.png)

   Som standard är t.ex. den minsta storleken på **leveransmålet** angett till 50, vilket innebär att en leverans inkluderas i aviseringen som skickas av den här instrumentpanelen endast om den har minst 50 profiler som mål. Du kan ändra den här parametern om du vill inkludera leveranser som är inriktade på färre än 50 profiler.

   Expandera avsnittet nedan om du vill ha mer information om varje kriterieparameter:

   +++Tillgängliga kriterieparametrar

   * **Minimistorlek för leveransmål**: Om du till exempel anger 100 i det här fältet skickas ett meddelande endast för leveranser med ett mål på 100 mottagare eller mer. Denna parameter gäller för alla kriterier.
   * **Övervakningsperiod före och efter kontaktdatumet (i timmar)**: Antal timmar före och efter den aktuella tiden. Endast leveranser med ett kontaktdatum inom detta tidsintervall beaktas. Denna parameter gäller för alla kriterier. Som standard är värdet för det här fältet inställt på 24 timmar.
   * **Maximal kvot för fel med mjuk studs**: Ett meddelande skickas för alla leveranser med en felkvot för mjuk studs som är större än det angivna värdet. Som standard är värdet för det här fältet 0,05 (5%).
   * **Maximal kvot för hårdstudsfel**: Ett meddelande skickas för alla leveranser med en hårdstudsfelkvot som är större än det angivna värdet. Som standard är fältets värde inställt på 0,05 (5 %).
   * **Lägsta tröskelvärde för leveranstid i statusen Påbörja väntande (i minuter)**: Ett meddelande skickas för alla leveranser med statusen Påbörja väntande längre än vad som anges i det här fältet. Det betyder att statusen Påbörja väntande inte har beaktats av systemet än.
   * **Minimitid som krävs för beräkning av dataflöde (i minuter)**: Endast leveranser som har startats (med statusen Pågående) under mer än den angivna varaktigheten beaktas för leveranser med kriteriet för låg dataström.
   * **Maximal procentandel av bearbetade meddelanden för beräkning av dataflöde**: Endast leveranser med en procentandel av bearbetade meddelanden som är lägre än den angivna procentandelen tas med i beräkningen för leveranser med lågt dataflöde.
   * **Minsta förväntade dataflöde (i skickade meddelanden per timme)**: Endast leveranser med ett dataflöde som är lägre än det angivna värdet beaktas för leveranser med lågt dataflöde.
   * **Minsta bearbetningskvot som krävs för kriteriet Leveranser pågår**: Endast leveranser med en högre procentandel bearbetade meddelanden än den angivna procentandelen beaktas.

+++

1. Kontrollpaneler för aviseringar är inaktiverade som standard, vilket innebär att e-postaviseringar som är länkade till den här kontrollpanelen inte skickas. Om du vill aktivera kontrollpanelen omedelbart växlar du alternativet **Aktiverad** i avsnittet **Allmänt**, bredvid urvalsfältet för varningsgruppen.

   Du kan också spara kontrollpanelen och aktivera den senare.

   ![](assets/alerting-dashboard-enable.png)

1. Klicka på knappen **Spara** om du vill spara varningsinstrumentpanelen.

Aviseringspanelen öppnas med tomma data. När du är redo att aktivera den och skicka meddelanden klickar du på knappen **Inställningar** och växlar alternativet **Aktiverad** om du inte har gjort det tidigare.

Varje gång en leverans uppfyller de kriterier som anges i den här kontrollpanelen skickas ett varningsmeddelande till den angivna operatörsgruppen.

## Hantera kontrollpaneler för aviseringar

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Leveransaviseringar har skickats"
>abstract="I det här avsnittet kan du visualisera information relaterad till de senaste skickade varningarna."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Leveransaviseringshistorik"
>abstract="Panelen **Historik** innehåller alla aviseringar som skickas från den här instrumentpanelen. Klicka på ett objekt för att komma åt motsvarande aviseringar som skickats vid den aktuella tidpunkten."

Alla skapade aviseringspaneler är tillgängliga på menyn **Leveransavisering** på fliken **Kontrollpaneler** .

![](assets/alerting-dashboard-list.png)

Du kan duplicera eller ta bort en instrumentpanel med knappen **Fler åtgärder** bredvid namnet.

Om du vill visa en detaljerad vy av en kontrollpanel klickar du på dess namn i listan. Från den här skärmen kan du visualisera den senaste skickade varningen. Alla skickade aviseringar visas i den vänstra rutan. Klicka på ett objekt för att komma åt motsvarande aviseringar som skickats vid den aktuella tidpunkten.

![](assets/alerting-dashboard-details.png)

Om du vill redigera instrumentpanelen klickar du på knappen **Inställningar** i det övre högra hörnet och gör önskade ändringar.
