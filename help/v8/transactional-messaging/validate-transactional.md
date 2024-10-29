---
audience: end-user
title: Validera transaktionsmeddelanden
description: Lär dig hur du validerar ett transaktionsmeddelande i Campaign Web User Interface
source-git-commit: e0d87d22d9712837f085f94f9d9ba63e96f36b36
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Validera transaktionsmeddelanden

Under eller efter att du har skapat ditt transaktionsmeddelande kanske du vill validera innehållet med hjälp av ett dataexempel.

## Simulera innehåll {#simulate-content}

Följ de här stegen för att simulera innehållet i ditt meddelande:

* Kontrollera att personaliseringssökvägen i meddelandeinnehållet matchar ditt kontextexempel. I exemplet nedan använder vi sökvägen *rtEvent.ctx.basicDetails.firstName* för att visa testprofilens förnamn

  Du kan ändra meddelandets innehåll eller kontextexemplet så att de justeras.

  ![](assets/validate-verification.png){zoomable="yes"}

* Klicka på knappen **[!UICONTROL Simulate content]** om du vill förhandsgranska ditt transaktionsmeddelande med de data du angav i kontextexemplet.

  ![](assets/validate-simulate.png){zoomable="yes"}

  När du har kontrollerat innehållet klickar du på knappen **[!UICONTROL Close]**.

* Glöm inte att klicka på knappen **[!UICONTROL Republish]** om du har gjort några ändringar i innehållet.

## Skicka bevis

Om du vill testa och uppleva transaktionsmeddelandet så som det kommer att levereras via den valda kanalen (till exempel e-post, SMS eller push-meddelanden) kan du använda korrekturfunktionen.

Klicka på knappen **[!UICONTROL Send proof]** i fönstret [simuleringsinnehåll](#simulate-content).

![](assets/transactional-proof.png){zoomable="yes"}

I det nya fönstret som visas anger du e-postadressen (eller telefonnumret, beroende på kanalen) där du vill ha korrekturet. När du har angett den önskade adressen klickar du på knapparna **[!UICONTROL Send proof]** och **[!UICONTROL Confirm]**. Med den här åtgärden kan du skicka ett exempel på ditt transaktionsmeddelande, vilket säkerställer att alla personaliseringar, dynamiskt innehåll och formatering visas på rätt sätt som för slutanvändarna.

![](assets/transactional-sendproof.png){zoomable="yes"}

Detta är ett viktigt steg för att identifiera eventuella problem innan du publicerar ditt transaktionsmeddelande.
