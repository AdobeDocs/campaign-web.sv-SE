---
audience: end-user
title: Skicka ditt första mejl
description: Lär dig hur du skickar ditt första e-postmeddelande med användargränssnittet i Campaign Web
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
badge: label="Begränsad tillgänglighet"
source-git-commit: db06e0f54984991e1d6b1056932a9974e340546e
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 1%

---


# Skapa din första e-postadress {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Kom igång med e-post"
>abstract="Du kan skapa en fristående e-postleverans eller skapa ett e-postmeddelande i ett kampanjarbetsflöde. Lär dig hur du skapar leveransen, väljer målgrupp och utformar e-postinnehållet."


<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Kom igång med e-post"
>abstract="Du kan skapa en fristående e-postleverans eller skapa ett e-postmeddelande i ett kampanjarbetsflöde. Lär dig hur du skapar leveransen, väljer målgrupp och utformar e-postinnehållet."

<!--TO REMOVE ABOVE-->



Lär dig hur du skapar ditt första riktade e-postmeddelande. I det här fallet schemalägger du att ett e-postmeddelande skickas till Silver- och Gold-lojalitetsmedlemmar på ett visst datum.

Baserat på en fördefinierad [designmall](../email/create-email-templates.md), innehåller e-postmeddelandet även personaliserat innehåll baserat på kundprofilattribut.

## Skapa e-postleveransen {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Välj en e-postmall"
>abstract="En e-postmall är en specifik leveranskonfiguration som innehåller fördefinierade inställningar, till exempel typologiregler, personalisering eller routningsparametrar. Mallar definieras i Campaign-klientkonsolen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Definiera e-postegenskaper"
>abstract="Egenskaperna är de vanligaste leveransparametrarna som hjälper dig att namnge och klassificera leveransen. De extra inställningarna är valfria. Om leveransen baseras på ett utökat schema som har definierats i Adobe Campaign v8-konsolen, kan vissa specifika **Anpassade alternativ** fält är tillgängliga."

Du kan skapa en fristående e-postleverans eller skapa ett e-postmeddelande i ett kampanjarbetsflöde. Stegen nedan beskriver proceduren för en fristående (enshot) e-postleverans. Läs mer om leveransstegen i Adobe Campaign i [den här sidan](../msg/gs-deliveries.md).

Följ stegen nedan för att skapa en ny fristående e-postleverans.

1. Gå till **[!UICONTROL Deliveries]** till vänster och klicka på  **[!UICONTROL Create delivery]** -knappen.

   ![](../msg/assets/create-a-delivery.png)

1. Välj **[!UICONTROL Email]** som kanal och välj en e-postleveransmall i listan.

   >[!NOTE]
   >
   >Mallar är förkonfigurerade leveransinställningar som sparas för framtida bruk. [Läs mer](../msg/delivery-template.md)

   ![](assets/channel-template.png)

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.
1. Ange en etikett för leveransen och konfigurera ytterligare alternativ baserat på dina behov:

   * **[!UICONTROL Internal name]**: tilldela leveransens unika identifierare.
   * **[!UICONTROL Folder]**: lagra leveransen i en viss mapp.
   * **[!UICONTROL Delivery code]**: använd det här fältet för att ordna leveranser baserat på din egen namnkonvention.
   * **[!UICONTROL Description]**: ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange vilken typ av e-post det gäller för klassificeringsändamål.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Om du har utökat ditt schema med specifika anpassade fält kan du komma åt dem i **[!UICONTROL Custom options]** -avsnitt.

   ![](assets/email-properties.png)

1. Dessutom finns avancerade inställningar, som typologiregler och målmappningar, via **[!UICONTROL Settings]** på skärmens övre högra hörn. Dessa inställningar är förkonfigurerade i den valda mallen, men kan redigeras efter behov för det här specifika e-postmeddelandet. [Läs mer](../advanced-settings/delivery-settings.md)

## Definiera målgruppen {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Välj en målgrupp för leveransen"
>abstract="Välj den bästa målgruppen för ert marknadsföringsbudskap. Du kan välja en befintlig målgrupp (som redan definierats i en Campaign v8-instans eller från Adobe Experience Platform), skapa en ny målgrupp med frågemodelleraren eller överföra en fil som innehåller målgruppen. Kontrollgrupper är inte aktiverade för **Välj från fil** och vice versa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html" text="Välj huvudmålgrupper"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Ange en kontrollgrupp"

I det här fallet skickar du e-postmeddelandet till en befintlig målgrupp.

Ytterligare instruktioner om hur du arbetar med målgrupper finns i [det här avsnittet](../audience/about-recipients.md).

1. Om du vill välja målgrupp för e-postmeddelandet klickar du på **[!UICONTROL Select audience]** och välj en befintlig målgrupp i listan.

   I det här exemplet vill vi använda en befintlig målgrupp som riktar sig till kunder som tillhör lojalitetsnivåerna silver och guld.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >De målgrupper som är tillgängliga i listan kommer antingen från din Campaign v8-instans eller från Adobe Experience Platform om integreringen Mål/Källa har konfigurerats på din instans. Tack vare den här integreringen kan ni skicka segment från Experience Platform till Adobe Campaign och skicka iväg kampanjleverans och spårningsloggar till Adobe Experience Platform. Läs om hur du arbetar med Campaign och Adobe Experience Platform i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. När målgruppen har valts kan du förfina målgruppen ytterligare genom att tillämpa ytterligare regler.

   ![](assets/audience-selected.png)

1. Du kan också ställa in en kontrollgrupp för att analysera beteendet hos e-postmottagarna jämfört med dem som inte var det. [Lär dig hur du arbetar med kontrollgrupper](../audience/control-group.md)

## Definiera e-postinnehållet {#create-content}

Följ stegen nedan när du vill börja skapa ditt e-postinnehåll. I det här fallet använder du ett fördefinierat e-postmeddelande [leveransmall](../msg/delivery-template.md) för att utforma e-postmeddelanden.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. Klicka på **[!UICONTROL Edit content]** -knappen.

   ![](assets/email-edit-content.png)

   Då kommer du till ett dedikerat gränssnitt där du kan konfigurera e-postinnehållet och komma åt e-postdesignern. [Läs mer](edit-content.md)

   ![](assets/edit-content.png)

1. Ange ämnesraden i ditt e-postmeddelande och anpassa det med Expression Editor. [Lär dig anpassa ditt innehåll](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Om du vill utforma innehållet i e-postmeddelandet klickar du på knappen **[!UICONTROL Edit email body]** -knappen.

   Välj den metod du vill använda för att skapa e-postinnehåll. I det här exemplet använder du [fördefinierad innehållsmall](create-email-templates.md).

   ![](assets/select-template.png)

1. När du har valt mallen visas den i [E-postdesigner](create-email-content.md), där du kan göra nödvändiga ändringar och lägga till personalisering.

   Om du till exempel vill lägga till en anpassning i e-posttiteln markerar du komponentblocket och klickar på **[!UICONTROL Add Personalization]**.

   ![](assets/add-perso.png)

1. När du är nöjd med innehållet sparar och stänger du designen. Klicka **[!UICONTROL Save]** för att återgå till skärmen där e-postmeddelanden skapas.

   ![](assets/save-content.png)

## Schemalägg sändning {#schedule}

Följ stegen nedan för att schemalägga sändning av e-post.

Ytterligare instruktioner om hur leveranssändningen schemaläggs finns i [det här avsnittet](../msg/gs-messages.md#gs-schedule).

1. Gå till **[!UICONTROL Schedule]** -avsnitt.

1. Använd **[!UICONTROL Enable scheduling]** för att aktivera den.

1. Ange önskat datum och klockslag för sändning.

   ![](assets/schedule.png)

När du har skickat leveransen börjar den faktiska avsändaren på det kontaktdatum som du har angett.

## Förhandsgranska och testa e-postmeddelandet {#preview-test}

Innan du skickar e-postmeddelandet kan du förhandsgranska och testa det för att kontrollera att det uppfyller dina förväntningar.

I det här fallet förhandsgranskar du e-postmeddelandet och skickar testversioner till specifika e-postadresser samtidigt som du personifierar vissa av målprofilerna.

Mer information om hur du förhandsgranskar och testar e-postmeddelanden finns i [det här avsnittet](../preview-test/preview-test.md).

1. Om du vill granska din e-post klickar du på **[!UICONTROL Review and send]**. Då visas en förhandsgranskning av ditt e-postmeddelande tillsammans med alla konfigurerade egenskaper, målgrupp och schema. Du kan redigera dessa element genom att klicka på knappen Ändra.

1. Om du vill förhandsgranska e-postmeddelandet och skicka testversioner klickar du på **[!UICONTROL Simulate content]** -knappen.

   ![](assets/review-email.png)

1. Till vänster markerar du de profiler som du vill använda för att förhandsgranska e-postmeddelandet.

   I den högra rutan visas en förhandsgranskning av e-postmeddelandet baserat på den valda profilen. Om du har lagt till flera profiler kan du växla mellan dem för att förhandsgranska motsvarande e-postmeddelande.

   ![](assets/preview.png)

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Om du vill skicka testversioner av e-postmeddelandet klickar du på **[!UICONTROL Test]** väljer du sedan det läge som du vill använda.

   I det här exemplet använder du **[!UICONTROL Substitute from main target]** läge, som skickar testversioner till specifika e-postadresser och personifierar några av profilerna som e-postmeddelandet riktar sig till.

   ![](assets/proof-mode.png)

1. Klicka **[!UICONTROL Add address]** och ange den eller de e-postadresser som tar emot testversionerna.

   För varje e-postadress väljer du den profil som ska personifieras. Du kan också låta Adobe Campaign välja en slumpmässig profil från målet.

   ![](assets/proof-test-profile.png)

1. Klicka **[!UICONTROL Send test email]** och bekräfta sändningen.

   Testversioner skickas till de angivna e-postadresserna med den valda profilen med **[Korrektur x]** prefix.

   ![](assets/proof-sent.png)

   Du kan när som helst kontrollera status för det skickade e-postmeddelandet och få tillgång till det skickade testmeddelandet genom att klicka på **[!UICONTROL View test email log]** på skärmen för simulering av innehåll.

## Skicka och övervaka e-postmeddelandet {#prepare-send}

När du har granskat och testat ditt e-postmeddelande kan du starta det och skicka det.

1. Klicka på **[!UICONTROL Prepare]**. [Lär dig förbereda ett e-postmeddelande](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. När mejlet är klart att skickas klickar du på **[!UICONTROL Send]** knapp (eller **[!UICONTROL Send as scheduled]** om du har schemalagt sändning) och bekräfta sändningen.

1. Under sändningsprocessen kan du spåra dess förlopp och visa statistik i realtid direkt på den här skärmen.

   ![](assets/sending-email.png)

   <!--
    ![](assets/sent-email.png)-->

   Du kan även få tillgång till detaljerad information om sändningen genom att klicka på knappen **[!UICONTROL Logs]** -knappen. [Lär dig övervaka leveransloggar](../monitor/delivery-logs.md)

1. När e-postmeddelandet har skickats kan du få åtkomst till dedikerade rapporter för ytterligare analys genom att klicka på **[!UICONTROL Reporting]** -knappen.

![](assets/reports.png)
