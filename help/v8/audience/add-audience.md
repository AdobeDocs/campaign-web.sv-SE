---
audience: end-user
title: Välj en befintlig målgrupp
description: Lär dig hur du väljer en målgrupp
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: 334014d3d89c878617b8e43ea73c9ff4e957f6d7
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 5%

---


# Välj en befintlig målgrupp {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Välj en befintlig målgrupp"
>abstract="Bläddra i listan för att välja en befintlig målgrupp. Använd ikonen Visa filter om du vill filtrera listan eller markera en viss mapp."

I det här avsnittet beskrivs hur du väljer en befintlig målgrupp när du definierar målpopulationen för en e-postleverans.

Du kan även:

* Bygg en ny publik. [Läs mer](segment-builder.md)
* Läsa in en målgrupp från en extern fil (endast för e-post). [Läs mer](file-audience.md)
* Använda en Adobe Experience Platform-målgrupp. [Läs mer](aep-audience.md).


Följ stegen nedan för att välja en befintlig målgrupp för ditt meddelande:

1. Från **Målgrupp** i leveransguiden klickar du på **[!UICONTROL Select audience]** -knappen.

   ![](assets/create-audience.png)

1. Välj **[!UICONTROL Select audience]** för att använda en befintlig målgrupp. Om du vill skapa en ny målgrupp som ska användas i det här e-postmeddelandet väljer du **Skapa en egen**. Se detta [section](segment-builder.md).

   På den här skärmen visas alla befintliga målgrupper för den aktuella mappen.

   ![](assets/create-audience2.png)

   Målgrupper skapas från **Målgrupp** vänster meny. De kan också skapas i klientkonsolen.

   Om du vill använda Adobe Experience Platform målgrupper måste du konfigurera integreringen med Destinations. Se [Dokumentation för Adobe Experience Platform Destinations](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.htmll?lang=sv){target="_blank"}.

1. Välj en målgrupp och klicka **Välj**.
1. Använd **Visa filter** om du vill visa filteralternativ. Klicka **Lägg till regler** för att komma åt regelbyggaren: med regelbyggaren kan du skapa avancerade filter för listan över målgrupper. Lär dig hur du använder regelbyggaren i det här [section](segment-builder.md).

   ![](assets/create-audience4.png)

1. Klicka **Spara**.

Ni kan också ställa in en kontrollgrupp för att mäta effekten av era kampanjer. Kontrollgruppen tar inte emot meddelandet. På så sätt kan du jämföra beteendet hos den population som fick meddelandet med beteendet hos kontakter som inte gjorde det. Läs mer i [det här avsnittet](control-group.md).