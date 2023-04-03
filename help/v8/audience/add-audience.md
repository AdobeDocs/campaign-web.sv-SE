---
audience: end-user
title: Välj en målgrupp
description: Lär dig hur du väljer en målgrupp
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 2%

---


# Välj en målgrupp {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Välj en befintlig målgrupp"
>abstract="Målgrupperna definieras i Adobe Campaign v8 Console. Om du har tillgång till en Adobe Experience Platform-integrering bör du även kunna se plattformsdefinierade målgrupper."

I det här avsnittet beskrivs hur du väljer en befintlig målgrupp när du definierar målpopulationen för en e-postleverans. Om du vill skapa en ny publik kan du läsa följande [section](segment-builder.md).

1. Från **Målgrupp** i leveransguiden klickar du på **[!UICONTROL Select audience]** -knappen.

   ![](assets/create-audience.png)

1. Välj **[!UICONTROL Select audience]** för att använda en befintlig målgrupp. Om du vill skapa en ny målgrupp som ska användas i det här e-postmeddelandet väljer du **Skapa en egen**. Se detta [section](segment-builder.md).

   På den här skärmen visas alla befintliga målgrupper som definierats i Adobe Campaign-konsolen eller från Adobe Experience Platform.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Om du vill utnyttja Adobe Experience Platform målgrupper måste du konfigurera integreringen med Destinations. Se [Destinationsdokumentation](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.htmll?lang=sv){target="_blank"}.

1. Välj en målgrupp och klicka **Välj**.

1. Klicka **Redigera regler** om ni vill förfina er målgrupp.

   ![](assets/create-audience3.png)

1. Med regelbyggaren kan ni utöka målgruppen med ytterligare filter eller genom att kombinera olika målgrupper. Se det här [section](segment-builder.md).

   ![](assets/create-audience4.png)

1. Klicka **Spara**.

Ni kan också ställa in en kontrollgrupp för att mäta effekten av era kampanjer. Kontrollgruppen tar inte emot meddelandet. På så sätt kan du jämföra beteendet hos den population som fick meddelandet med beteendet hos kontakter som inte gjorde det. Se [section](control-group.md).