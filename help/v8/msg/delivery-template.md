---
product: campaign
title: Använd leveransmallar
description: Lär dig hur du skapar och använder leveransmallar på Campaign Web
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
exl-id: cd3d4c2d-7bb2-4574-aeb8-6aac0683ec59
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 2%

---

# Använd leveransmallar {#work-with-delivery-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="Leveransmallar"
>abstract="Om du vill snabba upp och förbättra designprocessen skapar du leveransmallar för att återanvända anpassat innehåll och anpassade inställningar i alla era kampanjer. Den här funktionen standardiserar den kreativa utseendet och känslan, vilket ger snabbare genomförande och lansering av kampanjer."

Om du vill snabba upp och förbättra designprocessen skapar du leveransmallar för att återanvända anpassat innehåll och anpassade inställningar i alla era kampanjer. Den här funktionen standardiserar den kreativa utseendet och känslan, vilket ger snabbare genomförande och lansering av kampanjer.

En mall innehåller:

* Mallens **mapp** och **körningsmapp**. Mappen är den plats där leveransmallen sparas. Körningsmappen är den mapp där leveranser som skapats utifrån den här mallen sparas.
* [Typologier](../advanced-settings/delivery-settings.md#typology),
* Avsändarens adress.
* En [målgrupp](../audience/about-recipients.md), inklusive [kontrollgrupper](../audience/control-group.md),
* Anpassat [innehåll](../email/edit-content.md),
* [Personaliserade fält](../personalization/personalize.md) och [villkorligt innehåll](../personalization/conditions.md),
* Länkar till [spegelsida](../email/mirror-page.md) och [länkar](../email/message-tracking.md) som du inte prenumererar på,
* Andra leveransegenskaper, som resursgiltighet, återförsöksparametrar eller karantäninställningar.

>[!NOTE]
>
>Leveransmallar skiljer sig från [innehållsmallar](../email/create-email-templates.md) som gör att du kan återanvända endast innehållet i dina e-postmeddelanden och börja skapa innehåll med någon av de färdiga exempelmallarna.

## Få åtkomst till och hantera leveransmallar {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="Arbeta med leveransmallar"
>abstract="Använd leveransmallar för att skapa och spara leveransinställningar för framtida bruk i alla era kampanjer. Skapa leveransmallar från scratch, duplicera en befintlig mall eller konvertera en leverans till en mall."

Om du vill komma åt innehållsmalllistan väljer du **[!UICONTROL Campaign Management]** > **[!UICONTROL Deliveries]** på den vänstra menyn och bläddrar till fliken **Mallar**.

![Fliken Mallar på menyn Leveranser](assets/templates-tab.png){zoomable="yes"}

Alla mallar som skapas i den aktuella miljön visas.

Du kan filtrera innehållsmallar efter kanaler och mappar. Du kan också ange avancerade filter genom att skapa en regel med hjälp av leveransattribut. [Läs mer om frågemodelleraren](../audience/../query/query-modeler-overview.md)

![Filtreringsalternativ för mallar](assets/templates-filters.png){zoomable="yes"}

Om du vill redigera en mall klickar du på önskat objekt i listan. Därifrån:

* Ändra innehåll, egenskaper, målgrupp och eventuella erbjudanden som är kopplade till den.
* Testa mallen. [Läs mer](#test-template)

![Redigera en mall](assets/templates-edition.png){zoomable="yes"}

Om du vill ta bort eller [duplicera](#copy-an-existing-template) en mall väljer du motsvarande åtgärd på menyn **[!UICONTROL More actions]** , antingen från listan **[!UICONTROL Templates]** eller från en mallversionsskärm.

![Menyn Fler åtgärder för mallar](assets/templates-more-actions.png){zoomable="yes"}

>[!NOTE]
>
>När en mall redigeras eller tas bort påverkas inte leveranser som skapats med den här mallen.

## Skapa en leveransmall {#create-a-delivery-template}

Om du vill skapa en leveransmall kan du:

* Duplicera en befintlig mall - [Läs mer](#copy-an-existing-template)
* Konvertera en befintlig leverans till en mall - [Läs mer](#convert-an-existing-delivery)
* Skapa en leveransmall från grunden - [Läs mer](#create-a-new-template)

### Duplicera en befintlig leveransmall {#copy-an-existing-template}

Campaign innehåller inbyggda mallar för varje kanal: e-post, push och SMS. Det enklaste sättet att skapa en leveransmall är att duplicera och anpassa en inbyggd mall.

>[!NOTE]
>
>Du kan också duplicera en anpassad mall.

Så här duplicerar du en leveransmall:

1. Bläddra till fliken **Mallar** på den vänstra menyn i **Leveranser**. [Läs mer](#access-manage-templates)
1. Klicka på knappen **[!UICONTROL More actions]** till höger om det önskade mallnamnet och välj **[!UICONTROL Duplicate]**.

   Du kan också välja en mall i listan och välja det här alternativet på mallversionsskärmen.

1. Bekräfta duplicering.

   ![Bekräftelsedialogruta för duplicering av en mall](assets/templates-duplicate-confirm.png){zoomable="yes"}

1. Den nya mallkontrollpanelen öppnas på den centrala skärmen. Redigera mallinställningarna efter behov.

   ![Duplicerad mallkontrollpanel](assets/templates-duplicated-item.png){zoomable="yes"}

1. Klicka på knappen **[!UICONTROL Review]** om du vill spara och granska mallen. Du kan fortfarande redigera alla dess inställningar, ta bort och duplicera den.

   ![Granskningsskärmen för en mall](assets/templates-review-screen.png){zoomable="yes"}

1. Testa mallåtergivningen vid behov. [Läs mer](#test-template)

Den nya mallen läggs till i listan [**Mallar**](#access-manage-templates). Du kan nu välja den när du skapar en ny leverans.

### Konvertera en leverans till en mall {#convert-an-existing-delivery}

Alla leveranser kan konverteras till mallar för framtida upprepade leveransåtgärder.

Så här sparar du en leverans som en mall:

1. Bläddra till menyn **[!UICONTROL Campaign management]** > **[!UICONTROL Deliveries]**.
1. Klicka på knappen **[!UICONTROL More actions]** till höger om leveransnamnet på fliken **[!UICONTROL Browse]** och välj **[!UICONTROL Copy as a template]**.

   ![Alternativ för att kopiera en leverans som en mall](assets/templates-convert-delivery.png){zoomable="yes"}

   Du kan också välja en mall i listan och välja det här alternativet på mallversionsskärmen.

1. Bekräfta duplicering.

1. Den nya mallkontrollpanelen öppnas på den centrala skärmen. Redigera mallinställningarna efter behov.

1. Klicka på knappen **[!UICONTROL Review]** om du vill spara och granska mallen. Du kan fortfarande redigera alla dess inställningar, ta bort och duplicera den.

1. Testa mallåtergivningen vid behov. [Läs mer](#test-template)

Den nya mallen läggs till i listan [**Mallar**](#access-manage-templates). Du kan nu välja den när du skapar en ny leverans.

### Skapa en ny leveransmall {#create-a-new-template}

>[!NOTE]
>
>För att undvika konfigurationsfel rekommenderar Adobe [att du duplicerar en inbyggd mall](#copy-an-existing-template) och anpassar dess egenskaper i stället för att skapa en ny mall.

Så här konfigurerar du en leveransmall från grunden:

1. Bläddra till fliken **Mallar** på den vänstra menyn i **Leveranser**. [Läs mer](#access-manage-templates)
1. Klicka på knappen **[!UICONTROL Create template]**.

   ![Skapa mallknapp](assets/templates-create-button.png){zoomable="yes"}

1. Välj den kanal som du vill använda för mallen.
1. Den inbyggda leveransmallen för den kanalen används som standard för att hjälpa dig att skapa en egen mall. Använd den dedikerade knappen till höger om den valda kanalen för att välja en annan mall vid behov.

   ![Kanalval för en ny mall](assets/templates-channel-browse.png){zoomable="yes"}


1. Klicka på knappen **[!UICONTROL Create template]** igen.

1. Definiera mallegenskaperna, [målgrupp](../audience/add-audience.md) och innehåll beroende på den valda kanalen.

   >[!NOTE]
   >
   >Läs mer om distributionskanaler och hur du utformar respektive innehåll i avsnitten nedan:
   >
   > * [E-postkanal](../email/create-email.md)
   > * [Push-meddelandekanal](../push/gs-push.md)
   > * [SMS-kanal](../sms/create-sms.md)

1. För e-postmallar går det dessutom att komma åt avancerade inställningar, som typologiregler och målmappningar, via knappen **[!UICONTROL Settings]** längst upp till höger på skärmen. [Läs mer](../advanced-settings/delivery-settings.md)

1. Klicka på knappen **[!UICONTROL Review]** om du vill spara och granska mallen. Du kan fortfarande redigera alla dess inställningar, ta bort och duplicera den.

1. Testa mallåtergivningen vid behov. [Läs mer](#test-template)

Den nya mallen läggs till i listan [**Mallar**](#access-manage-templates). Du kan nu välja den när du skapar en ny leverans.

## Testa en leveransmall {#test-template}

Du kan testa återgivningen av alla leveransmallar, oavsett om de har skapats från grunden eller från ett befintligt innehåll. Gör så här:

1. Bläddra till fliken **Mallar** via menyn **[!UICONTROL Campaign management]** > **[!UICONTROL Deliveries]** och välj en mall. [Läs mer](#access-manage-templates)

1. Klicka på knappen **[!UICONTROL Simulate content]** längst upp till höger på skärmen.

   ![Knappen Simulera innehåll](assets/templates-simulate-button.png){zoomable="yes"}

1. Markera en eller flera testprofiler för att kontrollera e-poståtergivningen. Du kan också välja riktiga profiler från databasen. [Läs mer om testprofiler](../audience/test-profiles.md)

1. Växla mellan de olika profilerna för att få en personlig representation av meddelandet enligt den valda profilen. Du kan också justera zoomnivån och välja skrivbordsvy eller mobilvy.

[Läs mer om hur du förhandsgranskar innehåll](../preview-test/preview-content.md)

   ![Förhandsvisning av simulerat innehåll](assets/templates-stimulate.png){zoomable="yes"}

1. Stäng fönstret för att återgå till mallversionen.

>[!NOTE]
>
>Du kan inte använda e-poståtergivning eller skicka korrektur i en leveransmall.