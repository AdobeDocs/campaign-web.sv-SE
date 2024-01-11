---
title: Skapa villkorsstyrt innehåll
description: Lär dig hur du definierar villkor för att anpassa ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Skapa villkorsstyrt innehåll{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Lägga till villkorligt innehåll"
>abstract="Konfigurera villkorsstyrda innehållsfält för att skapa avancerad dynamisk personalisering baserat på mottagarens profildata. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt."

## Kom igång med villkorsstyrt innehåll {#gs}

Villkorligt innehåll är en kraftfull funktion som gör att du kan skapa dynamisk personalisering baserat på mottagarens profil och automatiskt ersätta textblock och bilder när vissa villkor uppfylls. Den här funktionen kan lyfta era kampanjer till nya höjder och leverera målinriktade, personaliserade upplevelser till er målgrupp.

Genom att konfigurera fält för villkorligt innehåll kan du skapa avancerad dynamisk personalisering som till exempel baseras på mottagarens profil. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt. Du kan t.ex. visa&quot;Herr&quot; eller&quot;fru&quot; enligt värdet i fältet Kön i Adobe Campaign-databasen, eller inkludera en annan länk baserat på vilket mottagarspråk som föredras.

Om du vill skapa villkorligt innehåll måste du skapa villkor i **uttrycksredigerare** med specifika hjälpfunktioner. Den här metoden är tillgänglig för alla leveranskanaler, i alla fält där du kan komma åt uttrycksredigeraren, till exempel ämnesraden, e-postlänkar och text-/knappinnehållskomponenter. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md/#access)

<!--In addition to the expression editor, you can leverage a dedicated **conditional content builder** when designing an email that allows you to build conditions using profile attributes only. [Learn how to create conditional content in emails](#condition-condition-builder)-->

## Skapa villkor i uttrycksredigeraren {#condition-perso-editor}

Följ stegen nedan för att definiera villkorligt innehåll för en leverans med uttrycksredigeraren. I det här exemplet vill vi skapa villkorligt innehåll baserat på mottagarens språk (franska eller engelska).

1. Öppna en leverans och navigera till delen för innehållsredigering.

1. Leta reda på fältet där du vill lägga till villkorligt innehåll. Du kan till exempel lägga till villkorligt innehåll i ett SMS-meddelande.

1. Klicka på **[!UICONTROL Open personalization dialog]** -ikonen bredvid fältet för att öppna uttrycksredigeraren.

   ![](assets/open-perso-editor-sms.png)

1. I personaliseringsredigeraren går du till **[!UICONTROL Helper functions]** till vänster.

1. Klicka på plustecknet bredvid ikonen för att börja skapa villkoret **If** funktion. Följande rad ska läggas till på den centrala skärmen:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Ersätt `<FIELD>` med ett anpassningsfält, t.ex. mottagarens språk: `recipient.language`.
   * Ersätt `<VALUE>` med det värde som ska uppfyllas. Till exempel: `'French'`.
   * Ersätt `Ìnsert content here` med det innehåll som du vill visa för de profiler som uppfyller det angivna villkoret.

     ![](assets/condition-sample1.png){width="800" align="center"}

1. Ange det innehåll som ska visas om mottagarna inte uppfyller villkoret. För att göra detta använder du **else** hjälpfunktion:

   1. Placera markören före uttryckets avslutande tagg `%>` och klicka på `+` bredvid **Annars** funktion.

   1. Ersätt `Ìnsert content here` med det innehåll som du vill visa för de profiler som inte uppfyller if-funktionens villkor.

   ![](assets/condition-sample2.png){width="800" align="center"}

   Du kan också använda **else if** hjälpfunktion för att skapa villkor med flera innehållsvarianter. Uttrycket nedan visar till exempel tre varianter av ett meddelande beroende på mottagarens språk:

   ![](assets/condition-sample3.png){width="800" align="center"}

   >[!NOTE]
   >
   >Varje gång en hjälpfunktion läggs till öppnas (`<%`) och avslutande (`%>`) läggs taggar automatiskt till före och efter funktionen.
   >
   >Exempel efter att du har lagt till en Else-hjälpfunktion i ett uttryck: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Se till att du tar bort de här taggarna för att undvika syntaxfel. I det här exemplet har det korrigerade uttrycket tagits bort **else** funktionstaggar är:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. När villkoret är klart kan du spara innehållet och kontrollera återgivningen genom att simulera innehållet.

<!--SECTION REMOVED FOR LA > CONDITIONAL CONTENT NOT AVAILABLE ANYMORE FROM THE DEDICATED MENU IN THE EMAIL DESIGNER. ONLY THE EXPRESSION EDITOR IS AVAILABLE FOR NOW

## Create conditional content in emails {#condition-condition-builder}

Conditional content in emails can be created in two ways:
* In the expression editor by building a condition with helper functions,
* In a dedicated conditional content builder that is accessible when designing an email.

Detailed information on how to create conditions using the expression editor is available [here](#condition-perso-editor). The following section provides step-by-step instructions on how to create conditions using the email designer's conditional content capability. In this example, we want to create an email message with multiple variants based on the recipients' language. Follow these steps:

1. Create or open an email delivery, edit its content, and click the **[!UICONTROL Edit email body]** button to open the email designing workspace.

1. Select a content component and click the **[!UICONTROL Enable conditional content]** icon.

    ![](assets/condition-email-enable.png){width="800" align="center"}

1. The **[!UICONTROL Conditional Content]** pane opens on the left-hand side of the screen. In this pane, you can create multiple variants of the selected content component using conditions.

1. Configure your first variant. Hover over **[!UICONTROL Variant - 1]** in the **[!UICONTROL Conditional Content]** pane and click the **[!UICONTROL Add condition]** icon.

1. A query modeler appears. Use profile attributes to create the condition for the first variant of the message and click **[!UICONTROL Confirm]**. In this example, we are creating a rule targeting recipients whose language is 'French'.

    ![](assets/condition-email-rule.png){width="800" align="center"}

1. The rule is now associated to the variant. For better readability, we recommend renaming the variant by clicking the ellipsis menu.

1. Configure how the component should display if the rule is met when sending the message. In this example, we want to display the text in French if it is the recipient's preferred language.

    ![](assets/condition-email-variant1.png){width="800" align="center"}

1. Add as many variants as needed for the content component. You can switch between the variants at any time to check how the content component will display based on their conditional rules.

    >[!NOTE]
    >If none of the rules defined in the variants are met when sending the message, the content component will display the content defined in the **[!UICONTROL Default variant]** from the **[!UICONTROL Conditional Content]** pane.
-->