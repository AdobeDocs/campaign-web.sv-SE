---
audience: end-user
title: Skicka ditt första e-postmeddelande
description: Lär dig hur du skickar ditt första e-postmeddelande med Campaign Web UI
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 871737ba2ab444eaaafde2a3822879629d956e1c
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 0%

---

# Skicka ditt första e-postmeddelande {#first-email}

![](../assets/do-not-localize/badge.png)

Lär dig hur du skapar din första riktade e-postadress i det här fallet. Vi planerar att skicka ett e-postmeddelande till kunder med silver- och guldkunder på en viss dag.

Med hjälp av en fördefinierad designmall kommer e-postmeddelandet även att innehålla anpassat innehåll baserat på kundprofilattribut.

![](assets/delivery-list.png)

## Skapa e-postmeddelandet {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Välj en e-postmall"
>abstract="En mall definieras i Adobe Campaign v8-konsolen. Detta är en specifik leveranskonfiguration som innehåller fördefinierade parametrar som typologiregler, personalisering eller routningsparametrar."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="E-postegenskaper"
>abstract="Egenskaperna är de vanligaste leveransparametrarna som hjälper dig att namnge och klassificera leveransen. Om leveransen baseras på ett utökat schema som har definierats i Adobe Campaign v8-konsolen, kan vissa specifika **Anpassade alternativ** fält är tillgängliga."

1. Om du vill skapa en ny leverans går du till **[!UICONTROL Deliveries]** meny och välj **[!UICONTROL Email]** som kanal.

1. Markera den mall som du vill använda och klicka på **[!UICONTROL Create delivery]**.

   >[!NOTE]
   >
   >Mallar är förkonfigurerade leveransinställningar som sparas för framtida bruk. De kan skapas av administratörsanvändare i Adobe Campaign Console. [Lär dig hur du arbetar med leveransmallar](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. Ange en etikett för e-postmeddelandet och konfigurera ytterligare alternativ baserat på dina behov:

   * **[!UICONTROL Internal name]**: tilldela en unik identifierare till leveransen,
   * **[!UICONTROL Folder]**: lagra leveransen i en viss mapp,
   * **[!UICONTROL Delivery code]**: Använd det här fältet för att ordna leveranser baserat på din egen namnkonvention,
   * **[!UICONTROL Description]**: ange en beskrivning av leveransen,
   * **[!UICONTROL Nature]**: Ange vilken typ av e-post det gäller för klassificeringsändamål.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Om du har utökat ditt schema med specifika anpassade fält kan du komma åt dem i **[!UICONTROL Custom options]** -avsnitt.

   ![](assets/email-properties.png)

   Dessutom kan du komma åt avancerade inställningar, t.ex. typologiregler och målmappningar, genom att klicka på knappen bredvid leveransnamnet. Dessa inställningar är förkonfigurerade i den valda mallen, men kan redigeras efter behov för det här specifika e-postmeddelandet.

## Skapa e-postinnehåll {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Lär dig hur du utformar e-postinnehåll"
>abstract="Lär dig hur du använder e-postdesignern."

I det här fallet använder vi en fördefinierad mall för att utforma e-postmeddelandet.

kommer att utforma e-postmeddelandet med en fördefinierad mall. Detaljerade instruktioner om hur du konfigurerar e-postinnehåll finns i [det här avsnittet](../content/edit-content.md).

1. Klicka på knappen **[!UICONTROL Edit content]** -knappen.

   Då kommer du till ett dedikerat gränssnitt där du kan konfigurera e-postinnehållet och utforma det med e-postdesignern.

   ![](assets/edit-content.png)

1. Skriv in ämnesraden i ditt e-postmeddelande och anpassa det med Expression Editor. [Lär dig anpassa ditt innehåll](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Klicka på knappen **[!UICONTROL Edit email body]** -knappen.

   Välj den metod du vill använda för att skapa e-postinnehåll. I det här exemplet använder vi en fördefinierad designmall.

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. När du har valt mallen visas den i e-postdesignern där du kan göra nödvändiga ändringar och lägga till personlig anpassning.

   Om du till exempel vill lägga till en anpassning i e-posttiteln markerar du komponentblocket och klickar på **[!UICONTROL Add Personalization]**.

   ![](assets/add-perso.png)

1. När du är nöjd med innehållet sparar och stänger du designen. Klicka **[!UICONTROL Save]** för att återgå till skärmen där e-postmeddelanden skapas.

   ![](assets/save-content.png)

## Definiera målgruppen {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definiera målgruppen"
>abstract="Välj den bästa målgruppen för ert marknadsföringsbudskap. Du kan välja en befintlig målgrupp som redan definierats i en Campaign v8-instans eller från Adobe Experience Platform, eller så kan du välja att skapa en ny målgrupp med regelbyggaren."

I det här fallet skickar vi e-postmeddelandet till en befintlig målgrupp. Ytterligare instruktioner om hur du arbetar med målgrupper finns i [det här avsnittet](../audience/about-audiences.md).

1. Klicka på knappen **[!UICONTROL Select audience]** och välj en befintlig målgrupp i listan.

   I det här exemplet vill vi använda en befintlig målgrupp som riktar sig till kunder som tillhör lojalitetsnivåerna silver och guld.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >De målgrupper som är tillgängliga i listan kommer antingen från Campaign V8-instansen eller från Adobe Experience Platform om integreringen av mål/källor har konfigurerats på din instans.
   >
   >Med integreringen Destination/Sources kan ni skicka segment från Experience Platform till Adobe Campaign och skicka loggar för leverans och spårning av kampanjer till Adobe Experience Platform. [Lär dig hur du arbetar med Campaign och Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. När målgruppen har valts kan du förfina målgruppen ytterligare genom att tillämpa ytterligare regler.

   Du kan också ställa in en kontrollgrupp för att analysera beteendet hos e-postmottagarna jämfört med dem som inte var det. [Lär dig hur du arbetar med kontrollgrupper](../audience/control-group.md)

   ![](assets/audience-selected.png)

## Schemalägg sändningen {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Schemalägg sändningen"
>abstract="Ange datum och exakt tid för sändningen. Genom att välja den tid som passar bäst för ert marknadsföringsbudskap kan ni maximera öppningsfrekvensen."

Om du vill schemalägga sändning av e-post klickar du på **[!UICONTROL Enable]** och ange önskat datum och klockslag för sändningen.

Som standard är **[!UICONTROL Confirm before sending]** är aktiverat, vilket kräver att du bekräftar att e-postmeddelandet ska skickas vid det schemalagda datumet och den schemalagda tidpunkten. Om du vill skicka e-postmeddelandet automatiskt på det schemalagda datumet och den schemalagda tidpunkten kan du inaktivera det här alternativet.

![](assets/schedule.png)

## Förhandsgranska och testa e-postmeddelandet {#preview-test}

Innan du skickar e-postmeddelandet kan du förhandsgranska och testa det för att kontrollera att det uppfyller dina förväntningar.

I det här fallet förhandsgranskar vi e-postmeddelandet och skickar testversioner till specifika e-postadresser samtidigt som vi personifierar några av målprofilerna.

Mer information om hur du förhandsgranskar och testar e-postmeddelanden finns i [det här avsnittet](../preview-test/preview-test.md).

1. Om du vill granska och skicka e-postmeddelandet klickar du på **[!UICONTROL Review and send]**. Då visas en förhandsgranskning av e-postmeddelandet tillsammans med alla konfigurerade egenskaper, målgrupp och schema. Du kan redigera dessa element genom att klicka på knappen Ändra.

1. Om du vill förhandsgranska e-postmeddelandet och skicka testversioner klickar du på **[!UICONTROL Simulate content]** -knappen. Förhandsvisningsgränssnittet öppnas.

   ![](assets/review-email.png)

1. Till vänster markerar du de profiler som du vill använda för att förhandsgranska e-postmeddelandet.

   Den högra rutan visar en förhandsgranskning av e-postmeddelandet baserat på den valda profilen. Om du har lagt till flera profiler kan du växla mellan dem för att förhandsgranska motsvarande e-postmeddelande.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Om du vill skicka testversioner av ditt e-postmeddelande klickar du på **[!UICONTROL Test]** väljer du sedan det läge som du vill använda.

   I det här exemplet använder vi **[!UICONTROL Substitute from main target]** läge, som skickar testversioner till specifika e-postadresser och personifierar några av profilerna som e-postmeddelandet riktar sig till.

   ![](assets/proof-mode.png)

1. Klicka **[!UICONTROL Add address]** och ange den eller de e-postadresser som ska ta emot testversionerna.

   För varje e-postadress väljer du den profil som ska personifieras. Du kan också låta Adobe Campaign välja en slumpmässig profil från målet.

   ![](assets/proof-test-profile.png)

1. Klicka **[!UICONTROL Send test email ]** och bekräfta sändningen.

   Testversioner skickas till de angivna e-postadresserna med den valda profilen med **[Korrektur x]** prefix.

   ![](assets/proof-sent.png)

   Du kan när som helst kontrollera status för det skickade e-postmeddelandet och få tillgång till det skickade testmeddelandet genom att klicka på **[!UICONTROL View test email log]** på skärmen för simulering av innehåll.

## Skicka och övervaka e-postmeddelandet {#prepare-send}

När du har granskat och testat ditt e-postmeddelande kan du starta det och skicka det.

1. Klicka på **[!UICONTROL Prepare]**. [Lär dig hur du förbereder ett e-postmeddelande](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. När e-postmeddelandet är klart att skickas klickar du på **[!UICONTROL Send]** knapp (eller **[!UICONTROL Send as scheduled]** om du har schemalagt sändning) och bekräfta sändningen.

1. Under sändningsprocessen kan du spåra dess förlopp och visa statistik i realtid direkt på den här skärmen.

   ![](assets/sent-mail.png)

   Du kan även få tillgång till detaljerad information om sändningen genom att klicka på **[!UICONTROL Logs]** -knappen. [Lär dig övervaka leveransloggar](../monitor/delivery-logs.md)

1. När e-postmeddelandet har skickats kan du få åtkomst till dedikerade rapporter för ytterligare analys genom att klicka på **[!UICONTROL Reporting]** -knappen.

![](assets/reports.png)
