---
audience: end-user
product: campaign
title: Arbeta med innehållsmallar
description: Lär dig hur du skapar mallar för att återanvända innehåll i Adobe Campaign e-postmeddelanden
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="Begränsad tillgänglighet"
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: bf4ee4b5f672dc91b7f5a494026c7df934a806f4
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Arbeta med innehållsmallar {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Innehållsmallar"
>abstract="För en snabbare och förbättrad designprocess kan du skapa fristående e-postmallar för att enkelt återanvända anpassat innehåll i Adobe Campaign. Dessa innehållsmallar kan utformas från grunden, baserat på inbyggda eller anpassade mallar, skapas från ett befintligt innehåll eller importeras i innehållsmallens redigerare."

För en snabbare och förbättrad designprocess kan du skapa fristående mallar för att enkelt återanvända anpassat innehåll i [!DNL Adobe Campaign]. Dessa innehållsmallar kan utformas från grunden, baserat på inbyggda eller anpassade mallar, skapas från ett befintligt innehåll eller importeras i innehållsmallens redigerare.

Med den här funktionen kan innehållsorienterade användare arbeta med fristående mallar så att marknadsföringsanvändare kan återanvända och anpassa dem i sina egna e-postkampanjer.

>[!NOTE]
>
>Endast för närvarande **e-post** Innehållsmallar stöds.

## Åtkomst till innehållsmallar {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Redigera mallinnehåll"
>abstract="Klicka på **Redigera innehåll** för att uppdatera innehållet med e-postdesignern."

Bläddra till innehållsmallslistan för att komma åt den **[!UICONTROL Content Management]** > **[!UICONTROL Content Templates]** menyn från den vänstra listen.

![](assets/content-template-list.png)

På den här instrumentpanelen visas alla tillgängliga innehållsmallar som en lista. Du kan filtrera på en viss [mapp](../get-started/permissions.md#folders) använda listrutan eller lägga till regler med [frågemodellerare](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

I listan kan du redigera, duplicera eller ta bort befintliga innehållsmallar. Använd knappen i det övre avsnittet för att skapa en innehållsmall.


## Skapa innehållsmallar {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Design av innehållsmall"
>abstract="Design av innehållsmall"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Val av innehållsmall"
>abstract="Val av innehållsmall"

Innehållsmallar kan skapas av [spara ett befintligt e-postmeddelande som en mall](#save-as-template)eller från listan med e-postmallar via **Skapa innehållsmall** knapp, [enligt nedan](#create-template-from-scratch).

När du har sparat mallen kan du nu använda den när du skapar [e-post](../email/create-email.md) inom [!DNL Adobe Campaign]. [Lär dig mer](use-email-templates.md)

>[!NOTE]
>
>* Ändringar som görs i innehållsmallar sprids inte till e-postmeddelanden.
>
>* När mallar används i ett e-postmeddelande påverkas inte heller de ändringar du gör i e-postinnehållet av den tidigare använda innehållsmallen.

### Skapa en ny innehållsmall {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Definiera mallegenskaper"
>abstract="Definiera egenskaper för e-postinnehållsmallar som ska hämtas enkelt när det behövs."

Så här skapar du en ny innehållsmall från kontrollpanelen för innehållsmallar:

1. Bläddra till innehållsmallslistan från **[!UICONTROL Content Management]** > **[!UICONTROL Content templates]** vänster räl.

1. Välj **[!UICONTROL Create template]**.

   ![](assets/content-template-create.png)

1. Ange malletiketten och -egenskaperna. Du kan välja den mapp där du vill spara mallen. Som standard lagras innehållsmallar i en dedikerad mapp i Adobe Campaign-hierarkin: **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Templates]** > **[!UICONTROL Content templates]**. Läs mer om mappar i [den här sidan](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

1. Klicka **[!UICONTROL Create]** och välja hur du vill utforma mallen bland de olika alternativen:

   * [Designa ditt innehåll från grunden](create-email-content.md) via e-postdesignerns gränssnitt.

   * [Kod eller kopiera-klistra in Raw-HTML](code-content.md) direkt in i e-postdesignern.

   * [Importera befintligt HTML-innehåll](existing-content.md) från en fil eller en ZIP-mapp.

   * Använd befintligt innehåll från en lista med inbyggda eller anpassade mallar. Stegen för hur du använder en innehållsmall i ett e-postmeddelande beskrivs i [det här avsnittet](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. E-postdesignern visas. Redigera ditt innehåll efter behov, på samma sätt som för alla e-postmeddelanden, beroende på vilket alternativ du har valt. Lär dig hur du använder e-postdesignern i [det här avsnittet](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. När mallen är klar klickar du **[!UICONTROL Save]**.

   Klicka vid behov på pilen bredvid mallnamnet för att gå tillbaka till **[!UICONTROL Details]** och redigera mallen.

   ![](assets/content-template-save-back.png)

Mallen är tillgänglig i **[!UICONTROL Content templates]** lista. [Läs mer](#access-templates)

Du kan nu använda den här mallen för att skapa nytt innehåll: det är tillgängligt i **[!UICONTROL Saved templates]** i e-postdesignern. [Lär dig mer](use-email-templates.md)

### Spara e-postinnehåll som mall {#save-as-template}

En gång [har utformat ett e-postmeddelande](create-email-content.md)kan du spara innehållet som en mall för framtida återanvändning. Sparade mallar är tillgängliga för alla användare i din Adobe Campaign-miljö.

Så här sparar du ett e-postinnehåll som en mall:

1. Klicka på knappen **[!UICONTROL More]** överst till höger på skärmen.

1. Välj **[!UICONTROL Save as content template]** i listrutan.

   ![](assets/email_designer-save-template.png)

1. Ange ett namn för mallen och spara.

   ![](assets/email_designer-template-name.png)

Mallen sparas och visas i **[!UICONTROL Content templates]** lista. Det blir en fristående innehållsmall som du kan komma åt, redigera och ta bort som alla andra objekt i listan. [Läs mer](#access-manage-templates)

Du kan nu använda den här mallen för att skapa nytt innehåll: det är tillgängligt i **[!UICONTROL Saved templates]** i e-postdesignern. [Lär dig mer](use-email-templates.md)

![](assets/email_designer-saved-template.png)


>[!NOTE]
>
>Ändringar i den nya mallen sprids inte till det e-postmeddelande som den kommer från. På samma sätt ändras inte den nya mallen när det ursprungliga innehållet redigeras i det e-postmeddelandet.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->


## Ändra en innehållsmall {#modify-delete}

Så här uppdaterar du en befintlig innehållsmall:

1. I listan med innehållsmallar klickar du på mallens etikett för att redigera den.

1. Klicka på **[!UICONTROL Edit content]** för att uppdatera innehållet med [E-postdesigner](get-started-email-designer.md).

![](assets/content-template-edition.png)

>[!NOTE]
>
>Ändringar som görs i innehållsmallar sprids inte till e-postmeddelanden med den här innehållsmallen.

## Ta bort en innehållsmall {#content-delete}

Du kan ta bort en innehållsmall på två sätt:

* i listan med innehållsmallar klickar du på ellipsknappen och väljer **Ta bort**

  ![Ta bort en innehållsmall från instrumentpanelen](assets/content-template-list-delete.png)

* från själva innehållsmallen klickar du på **Mer** knapp och markera **Ta bort**


>[!NOTE]
>
>När du tar bort en innehållsmall påverkas inte leveranser som skapats med den här mallen.


## Duplicera en innehållsmall {#content-duplicate}

Du kan duplicera en innehållsmall på två sätt:

* i listan med innehållsmallar klickar du på ellipsknappen och väljer **Duplicera**

* från själva innehållsmallen klickar du på **Mer** knapp och markera **Duplicera**

I båda fallen måste du bekräfta dupliceringen för att skapa den nya innehållsmallen. Den nya innehållsmallens etikett är **Kopia av`<label of the initial campaign`**. Bläddra till mallinställningarna för att uppdatera den här etiketten.

