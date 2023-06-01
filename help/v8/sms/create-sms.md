---
audience: end-user
title: Skapa en SMS-leverans
description: Lär dig hur du skapar och skickar SMS med Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: ec61c17d5a72b4d324d9a9a2cc71c85093c124ea
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 6%

---

# Skapa en SMS-leverans {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="SMS-leveransegenskaper"
>abstract="Egenskaperna omfattar de vanligaste leveransparametrarna som hjälper dig att både namnge och klassificera leveransen. Om leveransen baseras på ett utökat schema är specifika fält för anpassade alternativ tillgängliga."

1. Från **[!UICONTROL Deliveries]** hemsida, klicka **[!UICONTROL Create delivery]**.

1. Under **[!UICONTROL Channel]** väljer du SMS som kanal och väljer en mall. Läs mer om mallar

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.

1. Ange **[!UICONTROL Label]** för leverans och åtkomst till **[!UICONTROL Additional options]** nedrullningsbar meny.

   +++Konfigurera följande inställningar baserat på dina behov.
   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en viss mapp.
   * **[!UICONTROL Delivery code]**: Ordna leveranserna med din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange e-postens natur för klassificeringssyften.
+++

1. Från **[!UICONTROL Custom options]** kan du komma åt ditt utökade schema med specifika anpassade fält.

1. Klicka på **[!UICONTROL Select audience]** för att rikta sig till en befintlig målgrupp eller skapa en egen. Läs mer.

1. Aktivera **[!UICONTROL Enable control]** gruppalternativ för att ställa in en kontrollgrupp för att mäta effekten av leveransen, så att du kan jämföra beteendet hos den population som tog emot meddelandet med beteendet hos kontakter som inte gjorde det. Läs mer

1. Klicka **[!UICONTROL Edit content]** för att börja designa innehållet i SMS-meddelandet.

1. Om du vill schemalägga leveransen till ett visst datum och en viss tid aktiverar du **[!UICONTROL Enable scheduling]** alternativ. När du har initierat leveransen skickas meddelandet automatiskt på exakt det datum och klockslag som du har angett för mottagaren.
