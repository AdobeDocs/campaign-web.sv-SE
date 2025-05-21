---
audience: end-user
title: Kom igång med anpassade externa kanaler
description: Lär dig skapa och skicka anpassade externa kanaler med Adobe Campaign Web
source-git-commit: 7438ce1805cde00cf5b76f05d72bd19d2ef2343a
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Kom igång med anpassade externa kanaler {#gs-custom-channel}

Du kan, direkt från Adobe Campaign Web UI, samordna och genomföra leveranser baserat på anpassade externa kanaler som är integrerade med tredje part. Den anpassade externa kanalen skapas i klientkonsolen.

Ni kan konfigurera externa leveranser via anpassade kanaler i arbetsflöden eller som fristående leveranser, definiera er målgrupp och generera anpassningsbara exportfiler med alla nödvändiga kontakt- och personaliseringsdata.

>[!NOTE]
>
>Rapportering är inte tillgängligt i webbgränssnittet för externa kanaler för anpassade leveranser. Du måste bläddra till klientkonsolen för att komma åt rapporter.

Stegen nedan beskriver proceduren för en fristående leverans (en bild). De flesta steg liknar leveranser till callcenter. Mer information finns på [sidan](../call-center/create-call-center.md).

Så här skapar och skickar du en ny fristående anpassad extern leverans:

1. Skapa den anpassade externa kanalen, [läs mer](#create-channel)
1. Skapa leveransen, [läs mer](#create-delivery)
1. Definiera målgruppen, [läs mer](#select-audience)
1. Redigera innehållet, [läs mer](#edit-content)
1. Förhandsgranska och skicka leveransen, [läs mer](#preview-send)

## Skapa en anpassad extern kanal{#create-channel}

Först måste du konfigurera den anpassade externa kanalen. Här är huvudstegen som ska utföras i klientkonsolen:

1. Konfigurera schemat för att lägga till den nya kanalen i listan över tillgängliga kanaler.
1. Skapa ett nytt externt routningskonto.
1. Skapa en ny leveransmall som är kopplad till den nya kanalen.

Mer information finns i [dokumentationen för klientkonsolen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=sv-SE)

## Skapa leveransen{#create-delivery}

Följ de här stegen för att skapa leveransen och konfigurera dess egenskaper:

1. Välj menyn **[!UICONTROL Deliveries]** och klicka på knappen **[!UICONTROL Create delivery]**.

1. Välj önskad anpassad extern kanal, markera den associerade mallen och klicka på **[!UICONTROL Create delivery]** för att bekräfta.

   ![Skärmbild som visar hur en anpassad leverans skapas](assets/cus-create.png){zoomable="yes"}


1. Under **[!UICONTROL Properties]** anger du **[!UICONTROL Label]** för leveransen.

   ![Skärmbild som visar egenskapskonfigurationen för en anpassad leverans](assets/cus-properties.png){zoomable="yes"}

Mer information om hur du skapar leveranser finns i kundtjänstens [dokumentation](../call-center/create-call-center.md#create-delivery).

## Definiera målgruppen{#select-audience}

Nu måste ni definiera målgruppen som ska användas för extraheringsfilen.

1. Klicka på **[!UICONTROL Select audience]** i avsnittet **[!UICONTROL Audience]** på leveranssidan.

1. Välj en befintlig målgrupp eller skapa en egen.

   ![Skärmbild som visar målgruppsval för anpassad leverans](assets/cc-audience2.png){zoomable="yes"}

Mer information om målgruppsdefinition finns i kundtjänstens [dokumentation](../call-center/create-call-center.md#select-audience).

## Redigera innehållet{#edit-content}

Nu ska vi redigera innehållet i extraheringsfilen som ska genereras av den anpassade kanalleveransen.

1. Klicka på knappen **[!UICONTROL Edit content]** på leveranssidan.

1. Ange en **[!UICONTROL File name]**, markera en **[!UICONTROL File format]** och lägg till så många kolumner som behövs för extraheringsfilen.

   ![Skärmbild som visar attributkonfigurationsalternativen för extraheringsfilen.](assets/cc-content-attributes.png)

Mer information om innehållsutgåvan finns i callcentrets [dokumentation](../call-center/create-call-center.md#edit-content).

## Förhandsgranska och skicka leveransen{#preview-send}

När leveransinnehållet är klart kan du förhandsgranska det med testprofiler och skicka korrektur. Du kan sedan skicka leveransen för att generera extraheringsfilen.

1. Klicka på knappen **[!UICONTROL Simulate content]** på sidan för leveransinnehåll och välj testprofiler.

   ![Skärmbild som visar alternativet för att simulera innehåll på sidan för leveransinnehåll](assets/cus-simulate.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Review & send]** på leveranssidan och klicka på **[!UICONTROL Prepare]**. Bekräfta sedan.

   ![Skärmbild med förbered-alternativet och loggmenyn](assets/cus-prepare.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Send]** för att fortsätta med den sista sändningsprocessen och bekräfta sedan.

Mer information om förhandsgranskning och sändning finns i callcentrets [dokumentation](../call-center/create-call-center.md#preview-send).
