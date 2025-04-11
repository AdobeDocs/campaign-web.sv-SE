---
audience: end-user
title: Validera transaktionsmeddelanden
description: Lär dig hur du validerar ett transaktionsmeddelande i Campaign Web User Interface
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Validera transaktionsmeddelanden

Under eller efter att du har skapat ditt transaktionsmeddelande kanske du vill validera innehållet med hjälp av ett dataexempel.

## Simulera innehåll {#simulate-content}

Följ de här stegen för att simulera innehållet i ditt meddelande:

* Kontrollera att personaliseringssökvägen i meddelandeinnehållet matchar ditt kontextexempel. I exemplet nedan använder du sökvägen *rtEvent.ctx.basicDetails.firstName* för att visa testprofilens förnamn.

  Du kan ändra meddelandeinnehållet eller kontextexemplet så att de justeras.

  ![Skärmbild som visar verifieringen av anpassningssökvägar i meddelandeinnehållet](assets/validate-verification.png){zoomable="yes"}

* Klicka på knappen **[!UICONTROL Simulate content]** om du vill förhandsgranska ditt transaktionsmeddelande med data som har angetts i kontextexemplet.

  ![Skärmbild som visar knappen Simulera innehåll och förhandsvisningsfunktionen](assets/validate-simulate.png){zoomable="yes"}

  När du har granskat ditt innehåll klickar du på knappen **[!UICONTROL Close]**.

* Kontrollera att du klickar på knappen **[!UICONTROL Republish]** om du har gjort några ändringar i innehållet.

## Skicka bevis

Använd korrekturfunktionen om du vill testa och uppleva transaktionsmeddelandet som det skulle ha skickats via den valda kanalen, till exempel e-post, SMS eller push-meddelanden.

Klicka på knappen **[!UICONTROL Send proof]** i fönstret [simuleringsinnehåll](#simulate-content).

![Skärmbild som visar knappen Skicka korrektur i fönstret för simuleringsinnehåll](assets/transactional-proof.png){zoomable="yes"}

I det nya fönstret som visas anger du e-postadressen eller telefonnumret, beroende på kanalen, där du vill ha korrekturet. Klicka på knapparna **[!UICONTROL Send proof]** och **[!UICONTROL Confirm]** när du har angett den önskade adressen. Den här åtgärden skickar ett exempel på ditt transaktionsmeddelande och ser till att alla anpassningar, dynamiskt innehåll och formatering visas korrekt som de skulle ha gjort för slutanvändarna.

![Skärmbild som visar funktionen Skicka korrektur och bekräftelseprocessen](assets/transactional-sendproof.png){zoomable="yes"}

Det här steget är viktigt för att identifiera eventuella problem innan du publicerar ditt transaktionsmeddelande.