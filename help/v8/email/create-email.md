---
audience: end-user
title: Skicka ditt första mejl
description: Lär dig hur du skickar ditt första e-postmeddelande med användargränssnittet i Campaign Web
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 8006eeb6088d7d6ef99f374b2b846978cd679c01
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 1%

---

# Skapa din första e-postadress {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Kom igång med e-post"
>abstract="Du kan skapa en fristående e-postleverans eller skapa ett e-postmeddelande i ett kampanjarbetsflöde. Lär dig hur du skapar leveransen, väljer målgrupp och utformar e-postinnehållet."

Lär dig hur du skapar ditt första riktade e-postmeddelande. I det här fallet schemalägger du att ett e-postmeddelande skickas till Silver- och Gold-lojalitetsmedlemmar på ett visst datum.

Baserat på en fördefinierad [designmall](../email/create-email-templates.md) innehåller e-postmeddelandet även anpassat innehåll baserat på kundprofilattribut.

➡️ [Upptäck den här funktionen i videon](#video)

## Skapa e-postleveransen {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Välj en e-postmall"
>abstract="En e-postmall är en specifik leveranskonfiguration som innehåller fördefinierade inställningar, till exempel typologiregler, personalisering eller routningsparametrar. Mallar definieras i Campaign-klientkonsolen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Definiera e-postegenskaper"
>abstract="Egenskaperna är de vanligaste leveransparametrarna som hjälper dig att namnge och klassificera leveransen. De extra inställningarna är valfria. Om leveransen baseras på ett utökat schema som har definierats i Adobe Campaign v8-konsolen finns det vissa specifika **anpassade alternativ** -fält tillgängliga."

Du kan skapa en fristående e-postleverans eller skapa ett e-postmeddelande i ett kampanjarbetsflöde. Stegen nedan beskriver proceduren för en fristående (enshot) e-postleverans. Läs mer om stegen för leveransskapande i Adobe Campaign på [den här sidan](../msg/gs-deliveries.md).

Följ stegen nedan för att skapa en ny fristående e-postleverans.

1. Bläddra till menyn **[!UICONTROL Deliveries]** i den vänstra listen och klicka på knappen **[!UICONTROL Create delivery]**.

   ![Skärmbild som visar knappen Skapa leverans på menyn Leveranser](../msg/assets/create-a-delivery.png)

1. Välj **[!UICONTROL Email]** som kanal och välj en e-postleveransmall i listan.

   >[!NOTE]
   >
   >Mallar är förkonfigurerade leveransinställningar som sparas för framtida bruk. [Läs mer](../msg/delivery-template.md)

   ![Skärmbild som visar valet av e-postkanal och mall](assets/channel-template.png){zoomable="yes"}

1. Bekräfta genom att klicka på knappen **[!UICONTROL Create delivery]**.
1. Ange en etikett för leveransen och konfigurera ytterligare alternativ baserat på dina behov:

   * **[!UICONTROL Internal name]**: Tilldela en unik identifierare till leveransen.
   * **[!UICONTROL Folder]**: Lagra leveransen i en specifik mapp.
   * **[!UICONTROL Delivery code]**: Använd det här fältet för att ordna leveranser baserat på din egen namnkonvention.
   * **[!UICONTROL Description]**: Ange en beskrivning för leveransen.
   * **[!UICONTROL Nature]**: Ange typ av e-post för klassificeringssyften.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Om du har utökat ditt schema med specifika anpassade fält kan du komma åt dem i avsnittet **[!UICONTROL Custom options]**.

   ![Skärmbild som visar e-postegenskapskonfigurationen](assets/email-properties.png){zoomable="yes"}

1. Dessutom kan du komma åt avancerade inställningar, som typologiregler och målmappningar, via knappen **[!UICONTROL Settings]** längst upp till höger på skärmen. Dessa inställningar är förkonfigurerade i den valda mallen men kan redigeras efter behov för det här specifika e-postmeddelandet. [Läs mer](../advanced-settings/delivery-settings.md)

## Definiera målgruppen {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Välj en målgrupp för leveransen"
>abstract="Välj den bästa målgruppen för ert marknadsföringsbudskap. Du kan välja en befintlig målgrupp (som redan definierats i en Campaign v8-instans eller från Adobe Experience Platform), skapa en ny målgrupp med frågemodelleraren eller överföra en fil som innehåller målgruppen. Kontrollgrupper är inte aktiverade för alternativet **Välj från fil** och vice versa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html?lang=sv-SE" text="Välj huvudmålgrupper"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=sv-SE" text="Ange en kontrollgrupp"

I det här fallet skickar du e-postmeddelandet till en befintlig målgrupp.

Ytterligare instruktioner om hur du arbetar med målgrupper finns i [det här avsnittet](../audience/about-recipients.md).

1. Om du vill välja målgrupp för e-postmeddelandet klickar du på knappen **[!UICONTROL Select audience]** och väljer en befintlig målgrupp i listan.

   I det här exemplet vill vi använda en befintlig målgrupp som riktar sig till kunder som tillhör poängen Silver och Gold.

   ![Skärmbild som visar målgruppsurvalsprocessen](assets/create-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >De målgrupper som är tillgängliga i listan kommer antingen från din Campaign v8-instans eller från Adobe Experience Platform om integreringen med Destination/Source har konfigurerats på din instans. Med den här integreringen kan ni skicka Experience Platform-segment till Adobe Campaign och skicka leverans- och spårningsloggar för Campaign till Adobe Experience Platform. Lär dig hur du arbetar med Campaign och Adobe Experience Platform i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=sv-SE){target="_blank"}.

1. När målgruppen har valts kan du förfina målgruppen ytterligare genom att tillämpa ytterligare regler.

   ![Skärmbild som visar målgruppens förfiningsprocess](assets/audience-selected.png){zoomable="yes"}

1. Du kan också ställa in en kontrollgrupp för att analysera beteendet hos e-postmottagarna jämfört med dem som inte var det. [Lär dig arbeta med kontrollgrupper](../audience/control-group.md)

## Definiera e-postinnehållet {#create-content}

Följ stegen nedan när du vill börja skapa ditt e-postinnehåll. I det här fallet använder du en fördefinierad e-postmall [för leverans](../msg/delivery-template.md) för att utforma e-postmeddelandet.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. Klicka på knappen **[!UICONTROL Edit content]** på kontrollpanelen för e-postleverans.

   ![Skärmbild med knappen Redigera innehåll](assets/email-edit-content.png){zoomable="yes"}

   Då kommer du till ett dedikerat gränssnitt där du kan konfigurera e-postinnehållet och få tillgång till e-postprogrammet Designer. [Läs mer](edit-content.md)

   ![Skärmbild som visar e-post-Designer-gränssnittet](assets/edit-content.png){zoomable="yes"}

1. Ange ämnesraden i ditt e-postmeddelande och anpassa det med Expression Editor. [Lär dig anpassa ditt innehåll](../personalization/personalize.md)

   ![Skärmbild som visar ämnesradkonfigurationen](assets/subject-line.png){zoomable="yes"}

1. Om du vill utforma innehållet i e-postmeddelandet klickar du på knappen **[!UICONTROL Edit email body]**.

   Välj den metod du vill använda för att skapa e-postinnehåll. I det här exemplet använder du en [fördefinierad innehållsmall](create-email-templates.md).

   ![Skärmbild som visar valet av en fördefinierad innehållsmall](assets/select-template.png){zoomable="yes"}

1. När du har valt mallen visas den i [e-postmeddelandet för Designer](create-email-content.md), där du kan göra nödvändiga ändringar och lägga till personalisering.

   Om du till exempel vill lägga till anpassning i e-posttiteln markerar du komponentblocket och klickar på **[!UICONTROL Add Personalization]**.

   ![Skärmbild som visar personaliseringsprocessen](assets/add-perso.png){zoomable="yes"}

1. När du är nöjd med innehållet sparar och stänger du designen. Klicka på **[!UICONTROL Save]** för att återgå till skärmen där e-postmeddelanden skapas.

   ![Skärmbild med knappen Spara](assets/save-content.png){zoomable="yes"}

## Schemalägg sändning {#schedule}

När en leverans skickas i ett arbetsflödes kontext måste du använda aktiviteten **Schemaläggaren**. Läs mer på [den här sidan](../workflows/activities/scheduler.md). Stegen nedan gäller endast fristående leveranser.

1. Bläddra till avsnittet **[!UICONTROL Schedule]** i leveransegenskaperna.

1. Använd växlingsknappen **[!UICONTROL Enable scheduling]** för att aktivera den.

1. Ange önskat datum och klockslag för sändning.

   ![Skärmbild som visar schemaläggningskonfigurationen](assets/schedule.png){zoomable="yes"}

När du har skickat leveransen börjar den faktiska avsändaren på det kontaktdatum som du har angett.

Läs mer om leveransplanering i [det här avsnittet](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Förhandsgranska ett e-postmeddelande och skicka korrektur {#preview-test}

Innan du skickar e-postmeddelandet kan du förhandsgranska och testa det för att kontrollera att det uppfyller dina förväntningar.

I det här fallet förhandsgranskar du e-postmeddelandet och skickar korrektur till specifika e-postadresser samtidigt som du personifierar vissa av målprofilerna.

Mer information om hur du förhandsgranskar ett e-postmeddelande och skickar korrektur finns i [det här avsnittet](../preview-test/preview-test.md).

1. Klicka på **[!UICONTROL Review and send]** om du vill granska din e-post. Då visas en förhandsgranskning av ditt e-postmeddelande tillsammans med alla konfigurerade egenskaper, målgrupp och schema. Du kan redigera dessa element genom att klicka på knappen Ändra.

1. Klicka på knappen **[!UICONTROL Simulate content]** om du vill förhandsgranska e-postmeddelandet och skicka korrektur.

   ![Skärmbild som visar knappen Simulera innehåll](assets/review-email.png){zoomable="yes"}

   >[!NOTE]
   >
   >Knappen **[!UICONTROL Simulate content]** är inaktiverad i specifika sammanhang. Begränsningar anges [i det här avsnittet](#content-simulation-limitations).

1. Till vänster markerar du de profiler som du vill använda för att förhandsgranska e-postmeddelandet.

   I den högra rutan visas en förhandsgranskning av e-postmeddelandet baserat på den valda profilen. Om du har lagt till flera profiler kan du växla mellan dem för att förhandsgranska motsvarande e-postmeddelande.

   ![Skärmbild som visar e-postförhandsvisningen baserat på valda profiler](assets/preview.png){zoomable="yes"}

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using multiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Om du vill skicka korrektur klickar du på knappen **[!UICONTROL Send proofs]** och väljer sedan det läge som du vill använda.

   I det här exemplet använder du läget **[!UICONTROL Substitute from main target]** som skickar korrektur till specifika e-postadresser samtidigt som vissa profiler som e-postmeddelandet riktar sig till personifieras.

   ![Skärmbild som visar valet av korrekturutskicksläge](assets/proof-mode.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Add address]** och ange den eller de e-postadresser som tar emot korrekturen.

   För varje e-postadress väljer du den profil som ska personifieras. Du kan också låta Adobe Campaign välja en slumpmässig profil från målet.

   ![Skärmbild som visar tillägg av e-postadresser för korrektur](assets/proof-test-profile.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Send proof]** och bekräfta sändningen.

   Korrektur skickas till de angivna e-postadresserna med den valda profilen med prefixet **[Korrektur x]** .

   ![Skärmbild som visar bekräftelse på att bevis har skickats](assets/proof-sent.png){zoomable="yes"}

   Du kan när som helst kontrollera status för det skickade materialet och komma åt det skickade korrekturet genom att klicka på knappen **[!UICONTROL View proofs]** på skärmen för att simulera innehåll.

### Begränsningar för innehållssimulering {#content-simulation-limitations}

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_multilingual"
>title="Simulering av innehåll stöds inte"
>abstract="Knappen **Simulera innehåll** är inaktiverad eftersom den flerspråkiga leveransen bara innehåller en språkinställning."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_reconcilied_deliveries"
>title="Simulering av innehåll stöds inte"
>abstract="Knappen **Simulera innehåll** är inaktiverad eftersom den inte är kompatibel med avstämda leveranser i den här fasen."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_ffda"
>title="Simulering av innehåll stöds inte"
>abstract="Knappen **Simulera innehåll** är inaktiverad eftersom den inte stöds i FFDA-läge (Campaign Enterprise Full Federated Access)."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_no_file"
>title="Simulering av innehåll stöds inte"
>abstract="Knappen **Simulera innehåll** är inaktiverad eftersom inget innehåll har överförts."

I vissa fall kan du inte utföra innehållssimulering och knappen **[!UICONTROL Simulate content]** är inaktiverad.

Simulering av innehåll stöds inte i följande fall:

<!--* When a multilingual delivery contains only one locale,-->
* Med avstämda leveranser,
* När din Campaign-distributionsmodell är [Adobe Campaign Enterprise Full Federated Access (FFDA)](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/config/architecture/ffda/enterprise-deployment){target="_blank"}
* När ingen fil har överförts.

## Skicka och övervaka e-postmeddelandet {#prepare-send}

När du har granskat och testat ditt e-postmeddelande kan du starta det och skicka det.

1. Klicka på **[!UICONTROL Prepare]** om du vill starta förberedelsen av e-postmeddelandet. [Lär dig förbereda ett e-postmeddelande](../monitor/prepare-send.md)

   ![Skärmbild med knappen Förbered](assets/preparation.png){zoomable="yes"}

1. När ditt e-postmeddelande är klart att skickas klickar du på knappen **[!UICONTROL Send]** (eller **[!UICONTROL Send as scheduled]** om du har schemalagt att skicka det) och bekräftar att du skickat det.

1. Under sändningsprocessen kan du spåra dess förlopp och visa statistik i realtid direkt på den här skärmen.

   ![Skärmbild som visar e-postsändningsförloppet](assets/sending-email.png){zoomable="yes"}

   <!--
    ![Screenshot showing the email sent confirmation](assets/sent-email.png){zoomable="yes"}-->

   Du kan även få tillgång till detaljerad information om sändningen genom att klicka på knappen **[!UICONTROL Logs]**. [Lär dig övervaka leveransloggar](../monitor/delivery-logs.md)

1. När e-postmeddelandet har skickats kan du komma åt dedikerade rapporter för ytterligare analys genom att klicka på knappen **[!UICONTROL Reporting]**.

![Skärmbild med rapportknappen](assets/reports.png){zoomable="yes"}

## Instruktionsvideo {#video}

Lär dig hur du skapar en e-postleverans från grunden, definierar målgruppen, utformar innehållet, simulerar förhandsgranskning och skickar ett korrektur.

>[!VIDEO](https://video.tv.adobe.com/v/3454009/?quality=12&captions=swe)