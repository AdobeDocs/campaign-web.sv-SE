---
audience: end-user
title: Designa en leverans av push-meddelanden
description: Så här utformar du ett push-meddelande med Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 965c2d72d81233c98beb4e4bc3c76692c7bf3990
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 6%

---

# Designa en push-leverans {#content-push}

## Meddelande {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Med Firebase Cloud Messaging kan du välja mellan två typer av meddelanden:

* The **Datameddelande**, hanteras av klientprogrammet. Meddelanden skickas direkt till mobilprogrammet som genererar och visar android-meddelandet till enheten. Datameddelanden innehåller bara dina anpassade programvariabler.

   Klicka på **[!UICONTROL Message]** och använd uttrycksredigeraren för att definiera innehåll, anpassa data och lägga till dynamiskt innehåll.

* Meddelandet som hanteras automatiskt av FCM SDK. FCM visar automatiskt meddelandet på användarnas enheter för klientappens räkning. Meddelanden innehåller en fördefinierad uppsättning parametrar och alternativ, men de kan fortfarande anpassas ytterligare med anpassade programvariabler.

   Klicka på knappen **[!UICONTROL Title]** och **[!UICONTROL Body]** fält. Använd uttrycksredigeraren för att definiera innehåll, anpassa data och lägga till dynamiskt innehåll.

   Om du vill anpassa ditt push-meddelande ytterligare kan du välja en bild som du vill lägga till i ditt push-meddelande, meddelandeikonen som visas på dina profilers enheter och dess färg.

>[!TAB iOS]

Klicka på knappen **[!UICONTROL Title]** och **[!UICONTROL Body]** fält. Använd uttrycksredigeraren för att definiera innehåll, anpassa data och lägga till dynamiskt innehåll.

Du kan lägga till en **[!UICONTROL Subtitle]**, värdet för undertitelparametern för iOS-meddelandenyttolasten. Se det här avsnittet.

I läget för tyst överföring kan ett tyst meddelande skickas till ett mobilprogram. Användaren har inte informerats om meddelandets ankomst. Den överförs direkt till programmet.

>[!ENDTABS]

## Avancerade inställningar {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

* **[!UICONTROL Sound]**: Ställ in ljudet som ska spelas upp när enheten får ditt meddelande.

* **[!UICONTROL Notification Count]**: Ange antalet nya olästa uppgifter som ska visas direkt på programikonen.

* **[!UICONTROL Channel ID]**: Ange kanal-ID för meddelandet. Appen måste skapa en kanal med detta channel-id innan något meddelande med detta channel-id tas emot.

* **[!UICONTROL Click action]**: Ange åtgärden som är associerad med en användare genom att klicka på meddelandet.

* **[!UICONTROL Tag]**: Ange den identifierare som ska användas för att ersätta befintliga meddelanden i meddelandelådan.

* **[!UICONTROL Priority]**: Ange prioritetsnivåerna för dina meddelanden till standard, minimum, low eller high. Mer information finns i FCM-dokumentationen.

* **[!UICONTROL Visibility]**: Ange visningsnivåerna för meddelandet till public, private eller secrets. Mer information finns i FCM-dokumentationen.

* **[!UICONTROL Sticky]**: Om det är inaktiverat stängs meddelandet automatiskt när användaren klickar på det. Om det är aktiverat visas meddelandet fortfarande även när användaren klickar på det.

>[!TAB iOS]

* **[!UICONTROL Critical alert mode]**: aktivera det här alternativet för att lägga till ljud i meddelandet även om användarens telefon är inställd på fokusläge eller om iPhone är avstängt.

* **[!UICONTROL Clean Badge]**: aktivera det här alternativet för att uppdatera badge-värdet.

* **[!UICONTROL Notification count]**: Ange ett tal som ska användas för att visa antalet nya olästa uppgifter direkt på programikonen.

* **[!UICONTROL Volume]**: ljudvolymen från 0 till 100.

* **[!UICONTROL Mutable content]** (Endast iOS): Skickar flaggan för ändringsbart innehåll i push-nyttolasten och tillåter att push-meddelandeinnehållet ändras med ett meddelandetjänstprogramtillägg som tillhandahålls i iOS SDK. Mer information om detta hittar du i [Apples dokumentation för utvecklare](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). aktivera det här alternativet om du vill tillåta att mobilprogrammet hämtar medieinnehåll.

* **[!UICONTROL Relevance score]**: Ange ett relevansvärde mellan 0 och 100. Systemet använder detta för att sortera meddelandena i meddelandesammanfattningen.

* **[!UICONTROL Interruption level]**:

   * **[!UICONTROL Active]**: Som standard visas meddelandet omedelbart, skärmen visas och ett ljud kan spelas upp. Meddelanden går inte igenom fokusläget.

   * **[!UICONTROL Passive]**: Systemet lägger till meddelandet i meddelandelistan utan att skärmen eller ljudet ljussätts upp. Meddelanden går inte igenom fokusläget.

   * **[!UICONTROL Time sensitive]**: Systemet visar meddelandet omedelbart, lyser upp skärmen, kan spela upp ett ljud och gå igenom fokus-lägen. Den här nivån kräver inget särskilt tillstånd från Apple.

   * **[!UICONTROL Critical]**: Systemet visar meddelandet omedelbart, lyser upp skärmen och kringgår avstängningsväxeln eller fokusläget. Observera att den här nivån kräver ett särskilt tillstånd från Apple.

* **[!UICONTROL Thread-id]**: identifierare som används för att gruppera relaterade meddelanden tillsammans.

* **[!UICONTROL Category]**: namnet på ditt kategori-ID som kommer att visa åtgärdsknappar. Dessa meddelanden ger användaren ett snabbare sätt att utföra olika åtgärder som svar på ett meddelande utan att öppna eller navigera i programmet.

* **[!UICONTROL Target content ID]**: Identifierare som används för att ange vilket programfönster som ska flyttas fram när meddelandet öppnas.

* **[!UICONTROL Launch image]**: namnet på startbildfilen som ska visas. Om användaren väljer att starta programmet visas den valda bilden i stället för programmets startskärm.

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->


