---
audience: end-user
title: Designa ett omfattande leveransmeddelande
description: Lär dig hur du utformar en omfattande push-meddelandetjänst från Android med Adobe Campaign Web
exl-id: a87cb933-b564-4fa4-b173-6a94d7e27da5
source-git-commit: f48e9a6d75429d9038b4e6b0af65a15bcb6fe929
workflow-type: tm+mt
source-wordcount: '3053'
ht-degree: 1%

---

# Designa en omfattande Android-leverans {#rich-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_remind_later"
>title="Knappen Påminn senare"
>abstract="Med knappen **Påminn senare** kan du schemalägga en påminnelse. Tidsstämpelfältet kräver ett värde som representerar epok i sekunder."

>[!IMPORTANT]
>
>Innan du utformar ett push-meddelande måste du först konfigurera V2-anslutningen. Mer information finns på [den här sidan](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/sending-push-notifications/configure-the-mobile-app/configuring-the-mobile-application-android#configuring-external-account-android).

Med Firebase Cloud Messaging kan du välja mellan två typer av meddelanden:

* **[!UICONTROL Data message]** hanteras av klientprogrammet. Dessa meddelanden skickas direkt till mobilprogrammet som genererar och visar ett Android-meddelande på enheten. Datameddelanden innehåller bara dina anpassade programvariabler.

* **[!UICONTROL Notification message]**, hanteras automatiskt av FCM SDK. FCM visar automatiskt meddelandet på användarnas enheter för klientprogrammets räkning. Meddelanden innehåller en fördefinierad uppsättning parametrar och alternativ, men de kan fortfarande anpassas ytterligare med anpassade programvariabler.

![](assets/rich_push.png){zoomable="yes"}

## Definiera innehållet i meddelandet {#push-message}

När du har skapat din push-leverans kan du definiera innehållet med någon av följande mallar:

* Med **Standard** kan du skicka meddelanden med en enkel ikon och en medföljande bild.

* **Grundläggande** kan innehålla text, bilder och knappar i dina meddelanden.

* Med **Carousel** kan du skicka meddelanden med text och flera bilder som användare kan svepa igenom.

* Med ikonknapparna **kan du skicka meddelanden med en ikon och en motsvarande bild.**

* **Inmatningsrutan** samlar in användarindata och feedback direkt via meddelandet.

* **Produktkatalogen** visar en mängd olika produktbilder.

* **Med produktklassificering** kan användare ge feedback och betygsätta produkter.

* **Timer** innehåller en nedräkningstimer i dina meddelanden.

* **Nollkantsram** använder hela bakgrundsytan för en bild, med text utan synliga skarvar.

Gå igenom flikarna nedan för att lära dig mer om hur du anpassar mallarna.

>[!BEGINTABS]

>[!TAB Standard]

1. Välj **[!UICONTROL Default]** i listrutan **[!UICONTROL Template]**.

   ![](assets/rich_push_default.png)

1. Skriv texten i fälten **[!UICONTROL Title]** och **[!UICONTROL Message]** för att skapa meddelandet.

   ![](assets/rich_push_default_2.png)

1. Använd uttrycksredigeraren för att definiera innehåll, anpassa data och lägga till dynamiskt innehåll. [Läs mer](../personalization/personalize.md)

1. Definiera **[!UICONTROL Click action]** som är associerad med en användare och klicka på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja en **[!UICONTROL Image]**-URL att lägga till i ditt push-meddelande och meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

   ![](assets/rich_push_default_3.png)

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Grundläggande]

1. Välj **[!UICONTROL Basic]** i listrutan **[!UICONTROL Template]**.

   ![](assets/rich_push_basic.png)

1. Skriv texten i fälten **[!UICONTROL Title]**, **[!UICONTROL Message]** och **[!UICONTROL Expanded message]** för att skapa meddelandet.

   Texten **[!UICONTROL Message]** visas i den komprimerade vyn när **[!UICONTROL Expanded message]** visas när meddelandet expanderas.

   ![](assets/rich_push_basic_2.png)

1. Använd uttrycksredigeraren för att definiera innehåll, anpassa data och lägga till dynamiskt innehåll. [Läs mer](../personalization/personalize.md)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web URL]**: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja en **[!UICONTROL Image]**-URL att lägga till i ditt push-meddelande och meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

1. Klicka på **[!UICONTROL Add button]** och fyll i följande fält:

   * **[!UICONTROL Label]**: Texten visas på knappen.
   * **[!UICONTROL Link URI]**: Ange den URI som ska köras när du klickar på knappen.
   * **[!UICONTROL Link type]**: Typ av länk antingen **[!UICONTROL Web URL]**, **[!UICONTROL Deeplink]** eller **[!UICONTROL Open App]**.

   Du kan inkludera upp till tre knappar i ditt push-meddelande. Om du väljer att använda **[!UICONTROL Remind later button]** kan du bara inkludera högst två knappar.

   ![](assets/rich_push_basic_4.png)

1. Klicka på knappen **[!UICONTROL Add remind later]** om du vill lägga till ett alternativ för Påminn mig senare i ditt push-meddelande. Ange **[!UICONTROL Label]** och **[!UICONTROL Timestamp]**.

   Ett värde som representerar epok i sekunder förväntas för fältet Tidsstämpel.

   ![](assets/rich_push_basic_5.png)

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Carousel]

1. Välj **[!UICONTROL Carousel]** i listrutan **[!UICONTROL Template]**.

   ![](assets/rich_push_carousel.png)

1. Skriv texten i fälten **[!UICONTROL Title]**, **[!UICONTROL Message]** och **[!UICONTROL Expanded message]** för att skapa meddelandet.

   Texten **[!UICONTROL Message]** visas i den komprimerade vyn när **[!UICONTROL Expanded message]** visas när meddelandet expanderas.

   ![](assets/rich_push_carousel_1.png)

1. Använd uttrycksredigeraren för att definiera innehåll, anpassa data och lägga till dynamiskt innehåll. [Läs mer](../personalization/personalize.md)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web UR]**L: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

   ![](assets/rich_push_carousel_2.png)

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

1. Välj hur **[!UICONTROL Carousel]** ska användas:

   * **[!UICONTROL Auto]**: bläddrar automatiskt igenom bilder som bildrutor och övergår i fördefinierade intervall.
   * **[!UICONTROL Manual]**: gör att användare kan svepa mellan bildrutor manuellt för att navigera bland bilderna.

     Aktivera alternativet **[!UICONTROL Filmstrip]** om du vill inkludera förhandsvisningar av föregående och nästa bild bredvid huvudbildrutan.

1. Klicka på **[!UICONTROL Add image]** och ange bildens URL och text.

   Se till att du inkluderar minst tre bilder och högst fem bilder.

   ![](assets/rich_push_carousel_3.png)

1. Hantera bildens ordning med nedpil och uppåtpil.

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Ikonknappar]

1. Välj **[!UICONTROL Icon buttons]** i listrutan **[!UICONTROL Template]**.

   ![](assets/rich_push_icon_1.png)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web URL]**: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

   ![](assets/rich_push_icon_2.png)

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

1. Lägg till URL:en för din **[!UICONTROL Cancel button image]**.

1. Klicka på **[!UICONTROL Add icon]** och ange din **bild-URL**, **[!UICONTROL Link URI]** och välj **[!UICONTROL Link type]**.

   Se till att du inkluderar minst tre ikoner och högst fem ikoner.

   ![](assets/rich_push_icon_3.png)

1. Hantera bildens ordning med nedpil och uppåtpil.

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

   ![](assets/rich_push_icon_4.png)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Inmatningsruta]

1. Välj **[!UICONTROL Input box]** i listrutan **[!UICONTROL Notification type]**.

   ![](assets/rich_push_input_1.png)

1. Skriv texten i fälten **[!UICONTROL Title]**, **[!UICONTROL Message]** och **[!UICONTROL Expanded message]** för att skapa meddelandet.

   Texten **[!UICONTROL Message]** visas i den komprimerade vyn när **[!UICONTROL Expanded message]** visas när meddelandet expanderas.

   ![](assets/rich_push_input_2.png)

1. Använd dynamiska personaliseringsfält för att definiera innehåll, personalisera data och lägga till dynamiskt innehåll. [Läs mer](../personalization/personalize.md)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web URL]**: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja en **[!UICONTROL Image]**-URL att lägga till i ditt push-meddelande och meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

1. Fyll i följande alternativ för **Inmatningsrutan**:

   * **[!UICONTROL Input receiver name]**: Ange namnet eller identifieraren för mottagaren av indata.
   * **[!UICONTROL Input text]**: Ange texten för **Inmatningsrutan**.
   * **[!UICONTROL Feedback text]**: Ange texten som ska visas efter ett svar.
   * **[!UICONTROL Feedback image]**: Lägg till URL:en för bilden som visas efter ett svar.

   ![](assets/rich_push_input_3.png)

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Produktkatalog]

1. Välj **[!UICONTROL Product catalog]** i listrutan **[!UICONTROL Notification type]**.

   ![](assets/rich_push_catalog_1.png)

1. Skriv texten i fälten **[!UICONTROL Title]** och **[!UICONTROL Message]** för att skapa meddelandet.

   ![](assets/rich_push_catalog_2.png)

1. Använd dynamiska personaliseringsfält för att definiera innehåll, personalisera data och lägga till dynamiskt innehåll. [Läs mer](../personalization/personalize.md)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web URL]**: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

1. Ange din **Klicka-för-åtgärd-text** och **bild**.

1. Välj **[!UICONTROL Display type]** mellan vågrät och lodrät.

1. Fyll i din **[!UICONTROL Catalog]**-objektinformation.

   Se till att du inkluderar minst tre objekt och högst fem.

   ![](assets/rich_push_catalog_3.png)

1. Hantera bildens ordning med nedpil och uppåtpil.

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Produktklassificering]

1. Välj **[!UICONTROL Product rating]** i listrutan **[!UICONTROL Notification type]**.

   ![](assets/rich_push_rating_1.png)

1. Skriv texten i fälten **[!UICONTROL Title]**, **[!UICONTROL Message]** och **[!UICONTROL Expanded message]** för att skapa meddelandet.

   Texten **[!UICONTROL Message]** visas i den komprimerade vyn när **[!UICONTROL Expanded message]** visas när meddelandet expanderas.

   ![](assets/rich_push_rating_2.png)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web URL]**: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja en **[!UICONTROL Image]**-URL att lägga till i ditt push-meddelande och meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

1. Lägg till dina **[!UICONTROL Rating icon in unselected state]**- och **[!UICONTROL Rating icon in selected state]**-URL:er.

   ![](assets/rich_push_rating_3.png)

1. Klicka på **[!UICONTROL Add rating]** och ange **[!UICONTROL Link URI]** och **[!UICONTROL Link type]**.

   Se till att du inkluderar minst tre omdömen och högst fem.

   ![](assets/rich_push_rating_4.png)

1. Hantera bildens ordning med nedpil och uppåtpil.

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Timer]

1. Välj **[!UICONTROL Timer]** i listrutan **[!UICONTROL Notification type]**.

   ![](assets/rich_push_timer_1.png)

1. Skriv texten i fälten **[!UICONTROL Title]** och **[!UICONTROL Message]** för att skapa meddelandet.

   Använd dynamiska personaliseringsfält för att definiera innehåll, personalisera data och lägga till dynamiskt innehåll. [Läs mer](../personalization/personalize.md)

   ![](assets/rich_push_timer_2.png)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web URL]**: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

   ![](assets/rich_push_timer_3.png)

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja en **[!UICONTROL Image]**-URL att lägga till i ditt push-meddelande och meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

1. Ange **[!UICONTROL Timer duration]** i sekunder eller **[!UICONTROL Timer end timestamp]** till en specifik epok-tidsstämpel.

   ![](assets/rich_push_timer_4.png)

1. Ange den text och bild som ska visas när timern har gått ut i fälten **[!UICONTROL Alternate title]**, **[!UICONTROL Alternate message]**, **[!UICONTROL Alternate expanded message]** och **[!UICONTROL Alternate launch image]**.

   ![](assets/rich_push_timer_5.png)

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!TAB Nollkantlinje]

1. Välj **[!UICONTROL Zero bezel]** i listrutan **[!UICONTROL Notification type]**.

   ![](assets/rich_push_bezel_1.png)

1. Skriv texten i fälten **[!UICONTROL Title]**, **[!UICONTROL Message]** och **[!UICONTROL Expanded message]** för att skapa meddelandet.

   Texten **[!UICONTROL Message]** visas i den komprimerade vyn när **[!UICONTROL Expanded message]** visas när meddelandet expanderas.

   ![](assets/rich_push_bezel_2.png)

1. Använd dynamiska personaliseringsfält för att definiera innehåll, personalisera data och lägga till dynamiskt innehåll. [Läs mer](../personalization/personalize.md)

1. Lägg till den URL som definierar den **[!UICONTROL Click action]** som är associerad med en användare som klickar på meddelandet. Detta avgör beteendet när användaren interagerar med meddelandet, till exempel öppnar en viss skärm eller utför en viss åtgärd i programmet.

1. Välj **[!UICONTROL Link type]** för den URL som du lade till i fältet **[!UICONTROL Click action]**:

   * **[!UICONTROL Web URL]**: Webb-URL:er dirigerar användare till onlineinnehåll. När de klickar uppmanas de enhetens standardwebbläsare att öppna och navigera till den angivna URL:en.

   * **[!UICONTROL Deeplink]**: Djuplänkar är URL-adresser som vägleder användare till specifika avsnitt i ett program även om programmet stängs. När du klickar på det här alternativet kan en dialogruta visas så att användarna kan välja mellan olika appar som kan hantera länken.

   * **[!UICONTROL Open App]**: Med öppna app-URL:er kan du ansluta direkt till innehåll i ett program. Det gör att ditt program kan etablera sig som standardhanterare för en viss typ av länk, utan att dialogrutan för olika betydelser visas.

   Mer information om hur du hanterar Android App Links finns i [dokumentationen för Android-utvecklare](https://developer.android.com/training/app-links).

1. Om du vill anpassa ditt push-meddelande ytterligare kan du välja en **[!UICONTROL Image]**-URL att lägga till i ditt push-meddelande och meddelandets **[!UICONTROL Icon]** som ska visas på dina profilers enheter.

   ![](assets/rich_push_bezel_3.png)

1. Välj **[!UICONTROL Collapsed notification style]** för ditt meddelande om du vill att meddelandet i första hand ska visa en bild eller text.

1. Konfigurera **[!UICONTROL Advanced settings]** för push-meddelandet. [Läs mer](#push-advanced)

När du har definierat meddelandeinnehållet kan du använda testprenumeranter för att förhandsgranska och testa meddelandet.

>[!ENDTABS]

## Avancerade inställningar för push-meddelanden {#push-advanced}

![](assets/push_content_5.png){zoomable="yes"}

| Parameter | Beskrivning |
|---------|---------|
| **[!UICONTROL Icon color]** | Ställ in färgen på ikonen med de hexadecimala färgkoderna. |
| **[!UICONTROL Title color]** | Ange färgen på titeln med de hexadecimala färgkoderna. |
| **[!UICONTROL Message text color]** | Ange färgen på meddelandetexten med de hexadecimala färgkoderna. |
| **[!UICONTROL Timer color]** | Ställ in färgen på Timer med de hexadecimala färgkoderna. |
| **[!UICONTROL Notification background color]** | Ange färgen på meddelandebakgrunden med de hexadecimala färgkoderna. |
| **[!UICONTROL Sound]** | Ställ in ljudet som ska spelas upp när enheten får ditt meddelande. |
| **[!UICONTROL Notification Count]** | Ange hur många nya olästa uppgifter som ska visas direkt på programikonen. På så sätt kan användaren snabbt se antalet väntande meddelanden. |
| **[!UICONTROL Channel ID]** | Ange meddelandets kanal-ID. Appen måste skapa en kanal med det här channel-id:t innan något meddelande med det här channel-id:t tas emot. |
| **[!UICONTROL Tag]** | Ange en identifierare som ska användas för att ersätta befintliga meddelanden i meddelanderutan. Detta förhindrar att flera meddelanden ackumuleras och säkerställer att endast den senaste relevanta aviseringen visas. |
| **[!UICONTROL Priority]** | Ange prioritetsnivån för meddelandet, som kan vara standard, minimum, low eller high. Prioritetsnivån avgör hur viktigt och brådskande meddelandet är, vilket påverkar hur det visas och om det kan kringgå vissa systeminställningar. Mer information finns i [FCM-dokumentationen](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibility]** | Ange synlighetsnivån för ditt meddelande, som kan vara offentlig, privat eller hemlig. Synlighetsnivån avgör hur mycket av meddelandets innehåll som visas på låsskärmen och andra känsliga områden. Mer information finns i [FCM-dokumentationen](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Sticky notification]** | När det är aktiverat visas meddelandet även när användaren klickar på det. <br>Om det inaktiveras stängs meddelandet automatiskt när användaren interagerar med det. Tack vare det klibbiga beteendet kan viktiga meddelanden finnas kvar på skärmen under längre perioder. |
| **[!UICONTROL Application variables]** | Gör att du kan definiera meddelandebeteende. Dessa variabler är helt anpassningsbara och ingår som en del av den meddelandenyttolast som skickas till den mobila enheten. |
