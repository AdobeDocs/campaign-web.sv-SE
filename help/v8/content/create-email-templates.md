---
audience: end-user
product: campaign
title: Arbeta med innehållsmallar
description: Lär dig hur du skapar mallar för att återanvända innehåll i Adobe Campaign e-postmeddelanden
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="LA"
source-git-commit: d52b3c31cbb3a045e9fab4b15b0e69e3303f16d2
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Arbeta med innehållsmallar {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Definiera ditt eget innehåll"
>abstract="Skapa en egen mall från grunden för att göra innehållet återanvändbart i flera e-postmeddelanden."

För en snabbare och förbättrad designprocess kan du skapa fristående mallar för att enkelt återanvända anpassat innehåll i [!DNL Adobe Campaign].

Med den här funktionen kan innehållsorienterade användare arbeta med fristående mallar så att marknadsföringsanvändare kan återanvända och anpassa dem i sina egna e-postkampanjer.

>[!NOTE]
>
>Endast för närvarande **e-post** Innehållsmallar stöds.

## Få åtkomst till och hantera mallar {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Redigera mallinnehåll"
>abstract="Klicka på **Redigera innehåll** för att uppdatera innehållet med e-postdesignern."

Om du vill komma åt innehållsmalllistan väljer du **[!UICONTROL Content Management]** > **[!UICONTROL Content Templates]** från den vänstra menyn.

![](assets/content-template-list.png)

Alla mallar som har skapats - antingen från ett e-postmeddelande med [Spara som mall](#save-as-template) alternativ, antingen från **[!UICONTROL Content Templates]** -menyn visas.

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

Du kan filtrera på en viss [mapp](../get-started/permissions.md#folders) använda listrutan eller lägga till regler med [frågemodellerare](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

Om du vill redigera ett mallinnehåll klickar du på önskat objekt i listan. Du kan:

* Redigera dess egenskaper.

* Klicka på **[!UICONTROL Edit content]** för att uppdatera innehållet med [E-postdesigner](get-started-email-designer.md).

![](assets/content-template-edition.png)

Om du vill ta bort en mall väljer du motsvarande alternativ i dialogrutan **[!UICONTROL More actions]** -menyn.

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>När en mall tas bort påverkas inte leveranser som skapats med den här mallen.

## Skapa innehållsmallar {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Design av innehållsmall"
>abstract="Design av innehållsmall"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Val av innehållsmall"
>abstract="Val av innehållsmall"

Det finns två sätt att skapa innehållsmallar:

* Skapa en innehållsmall från grunden med den vänstra listen **[!UICONTROL Content templates]** -menyn. [Lär dig mer](#create-template-from-scratch)

* När du utformar ett e-postmeddelande sparar du ditt e-postinnehåll som en mall. [Lär dig mer](#save-as-template)

När du har sparat, oavsett om du skapat från grunden eller från ett tidigare e-postmeddelande, kan du nu använda den här mallen när du skapar [e-post](../email/create-email.md) inom [!DNL Adobe Campaign]. [Lär dig mer](use-email-templates.md)

>[!NOTE]
>
>* Ändringar som görs i innehållsmallar sprids inte till e-postmeddelanden.
>
>* När mallar används i ett e-postmeddelande påverkas inte heller de ändringar du gör i e-postinnehållet av den tidigare använda innehållsmallen.

### Skapa mall från grunden {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Definiera mallegenskaper"
>abstract="När du skapar en mall från grunden kan du enkelt definiera vilka egenskaper som ska hämtas när det behövs."

Följ stegen nedan för att skapa en innehållsmall från grunden.

1. Få åtkomst till innehållsmalllistan via **[!UICONTROL Content Management]** > **[!UICONTROL Content templates]** vänster meny.

1. Välj **[!UICONTROL Create template]**.

   ![](assets/content-template-create.png)

1. Fyll i mallinformationen.

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >För närvarande bara **E-post** kanal och **HTML** type stöds.

1. Välj den mapp där du vill lagra mallen. Som standard lagras innehållsmallar i en dedikerad nod i Adobe Campaign-hierarkin: **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Templates]** > **[!UICONTROL Content templates]**. [Lär dig hur du skapar mappar](../get-started/permissions.md#folders)

1. Klicka **[!UICONTROL Create]** och välja hur du vill utforma mallen bland de olika alternativen:

   * [Designa din e-post från grunden](create-email-content.md) via e-postdesignerns gränssnitt.

   * [Kod eller kopiera-klistra in Raw-HTML](code-content.md) direkt in i e-postdesignern.

   * [Importera befintligt HTML-innehåll](existing-content.md) från en fil eller en ZIP-mapp.

   * Använd befintligt innehåll från en lista med inbyggda eller anpassade mallar. Stegen för hur du använder en innehållsmall i ett e-postmeddelande beskrivs i [det här avsnittet](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. The [E-postdesigner](get-started-email-designer.md) visas. Redigera ditt innehåll efter behov, på samma sätt som för alla e-postmeddelanden, beroende på vilket alternativ du har valt.

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. När mallen är klar klickar du **[!UICONTROL Save]**.

   Klicka vid behov på pilen bredvid mallnamnet för att gå tillbaka till **[!UICONTROL Details]** och redigera mallen.

   ![](assets/content-template-save-back.png)

Den här mallen kan nu användas när du skapar e-post i [!DNL Adobe Campaign]. [Lär dig mer](use-email-templates.md)

## Spara e-postinnehåll som mall {#save-as-template}

En gång [har utformat ett e-postmeddelande](create-email-content.md)kan du spara innehållet som en mall för framtida återanvändning. Sparade mallar är tillgängliga för alla användare i din Adobe Campaign-miljö.

Så här sparar du ett e-postinnehåll som en mall:

1. Klicka på knappen **[!UICONTROL More]** överst till höger på skärmen.

1. Välj **[!UICONTROL Save as content template]** i listrutan.

   ![](assets/email_designer-save-template.png)

1. Ange ett namn för mallen och spara.

   ![](assets/email_designer-template-name.png)

Du kan nu använda den här mallen för att skapa nytt innehåll: det är tillgängligt i **[!UICONTROL Saved templates]** i e-postdesignern. [Lär dig mer](use-email-templates.md)

![](assets/email_designer-saved-template.png)

Mallen sparas i **[!UICONTROL Content templates]** lista, tillgänglig från [!DNL Adobe Campaign] egen meny. Det blir en fristående innehållsmall som du kan komma åt, redigera och ta bort som alla andra objekt i listan. [Läs mer](#access-manage-templates)

>[!NOTE]
>
>Ändringar i den nya mallen sprids inte till det e-postmeddelande som den kommer från. På samma sätt ändras inte den nya mallen när det ursprungliga innehållet redigeras i det e-postmeddelandet.

<!--
Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list through the **[!UICONTROL Content Management]** > **[!UICONTROL Content Templates]** menu and select any template.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view. [Learn more](../content-management/preview-test.md)

    ![](../email/assets/content-template-stimulate.png)

1. You can send a proof to test your content and have it approved by some internal users before using it in a journey or a campaign.

    * To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in [this section](../content-management/proofs.md).
    
    * Before sending the proof, you must select the [email surface](../configuration/channel-surfaces.md) that will be used to test your content.

        ![](../email/assets/content-template-stimulate-proof-surface.png)

>[!CAUTION]
>
>Currently tracking is not supported when testing email content templates, meaning that tracking events, UTM parameters and landing page links will not be effective in the proofs that are being sent from a template. To test tracking, [use the content template](
use-email-templates.md) in an email and [send a proof](../content-management/preview-test.md#send-proofs).-->


