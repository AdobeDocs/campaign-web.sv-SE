---
audience: end-user
title: Använda e-postdesigners innehållskomponenter
description: Lär dig hur du använder innehållskomponenter i e-postmeddelanden
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
badge: label="Alpha" type="Informative"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 0%

---

# Använda e-postdesignerns innehållskomponenter {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Om innehållskomponenter"
>abstract="Innehållskomponenterna är tomma platshållare för innehåll som du kan använda för att skapa layouten för ett e-postmeddelande."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Om innehållskomponenter"
>abstract="Innehållskomponenterna är tomma platshållare för innehåll som du kan använda för att skapa layouten för en landningssida."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Om innehållskomponenter"
>abstract="Innehållskomponenter är tomma platshållare för innehåll som du kan använda för att skapa layouten för ett fragment."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Om innehållskomponenter"
>abstract="Innehållskomponenter är tomma platshållare för innehåll som du kan använda för att skapa layouten för en mall."

## Lägga till innehållskomponenter {#add-content-components}

Följ stegen nedan för att lägga till innehållskomponenter i e-postmeddelanden och anpassa dem efter dina behov.

1. Använd ett befintligt innehåll i e-postdesignern eller dra och släpp **[!UICONTROL Structure components]** till ditt tomma innehåll för att definiera layouten för ditt e-postmeddelande. [Lär dig mer](create-email-content.md)

1. Så här öppnar du **[!UICONTROL Content components]** markerar du motsvarande knapp i den vänstra rutan i E-postdesignern.

   ![](assets/email_designer_content_components.png)

1. Dra och släpp de innehållskomponenter du vill ha inuti de relevanta strukturkomponenterna.

   ![](assets/email_designer_add_content_components.png)

   >[!NOTE]
   >
   >Du kan lägga till flera komponenter i en enda strukturkomponent och i varje kolumn i en strukturkomponent.

1. Justera formatattributen för varje komponent med **[!UICONTROL Component settings]** till höger. Du kan till exempel ändra textstil, utfyllnad eller marginal för varje komponent. [Läs mer om justering och utfyllnad](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png)

När du skapar ditt e-postinnehåll från grunden, **[!UICONTROL Content components]** gör att du kan anpassa e-postmeddelandet ytterligare med råa, tomma komponenter som du kan använda en gång i ett e-postmeddelande.
Du kan lägga till så många **[!UICONTROL Content components]** som du behöver i en **[!UICONTROL Structure component]** som definierar layouten för ditt e-postmeddelande.

## Behållare {#container}

Du kan lägga till en enkel behållare i vilken du lägger till en annan innehållskomponent. På så sätt kan du använda en särskild formatering för behållaren, som skiljer sig från den komponent som används inuti.

Lägg till exempel till en **[!UICONTROL Container]** och sedan lägga till en [Knapp](#button) -komponenten i den behållaren. Du kan använda en specifik bakgrund för behållaren och en annan för knappen.

![](assets/email_designer_container_component.png)

## Knapp {#buttons}

Använd **[!UICONTROL Button]** om du vill infoga en eller flera knappar i e-postmeddelandet och dirigera om din e-postpublik till en annan sida.

1. Från **[!UICONTROL Content components]**, dra och släpp **[!UICONTROL Button]** till en **[!UICONTROL Structure component]**.

   ![](assets/email_designer_13.png)

1. Klicka på den nya knappen för att anpassa texten och få tillgång till **[!UICONTROL Components settings]** i det högra fönstret i e-postdesignern.

   ![](assets/email_designer_14.png)

1. I **[!UICONTROL Link]** lägger du till den URL som du vill omdirigera till när du klickar på knappen.

1. Välj hur innehållet ska visas med **[!UICONTROL Target]** nedrullningsbar lista:

   * **[!UICONTROL None]**: öppnar länken i samma ram som den klickades på (standard).
   * **[!UICONTROL Blank]**: öppnar länken i ett nytt fönster eller på en ny flik.
   * **[!UICONTROL Self]**: öppnar länken i samma ram som den klickades på.
   * **[!UICONTROL Parent]**: öppnar länken i den överordnade ramen.
   * **[!UICONTROL Top]**: öppnar länken i hela fönstret.

   ![](assets/email_designer_15.png)

1. Du kan anpassa knappen ytterligare genom att ändra formatattribut som **[!UICONTROL Border]**, **[!UICONTROL Size]**, **[!UICONTROL Margin]**, osv. från **[!UICONTROL Component settings]** fönster.

## Text {#text}

Använd **[!UICONTROL Text]** om du vill infoga text i e-postmeddelandet och justera formatet (kantlinje, storlek, utfyllnad osv.) med **[!UICONTROL Component settings]** fönster.

1. Från **[!UICONTROL Content Components]**, dra och släppa **[!UICONTROL Text]** i en **[!UICONTROL Structure component]**.

   ![](assets/email_designer_11.png)

1. Klicka på den nya komponenten som du har lagt till för att anpassa texten och få tillgång till **[!UICONTROL Components Settings]** i den högra rutan i e-postdesignern.

1. Ändra texten med följande alternativ i verktygsfältet:

   ![](assets/email_designer_27.png)

   * **[!UICONTROL Change text style]**: använda fet, kursiv, understrykning eller genomstrykning i texten.
   * **Ändra justering**: Välj mellan vänster, höger, centrerad eller marginaljusterad justering för texten.
   * **[!UICONTROL Create list]**: lägg till punkt- eller nummerlista i texten.
   * **[!UICONTROL Set heading]**: kan du lägga till upp till sex rubriknivåer i texten.
   * **Teckenstorlek**: markera teckensnittsstorleken för texten i pixlar.
   * **[!UICONTROL Edit image]**: lägga till en bild eller en resurs i textkomponenten.
   * **[!UICONTROL Show the source code]**: visa textens källkod. Den kan inte ändras.
   * **[!UICONTROL Duplicate]**: lägga till en kopia av textkomponenten.
   * **[!UICONTROL Delete]**: ta bort den markerade textkomponenten från e-postmeddelandet.
   * **[!UICONTROL Add personalization]**: lägga till anpassningsfält för att anpassa innehållet utifrån dina profildata.
   * **[!UICONTROL Enable conditional content]**: lägga till villkorsstyrt innehåll för att anpassa komponentens innehåll till målprofilerna.

1. Justera övriga formatattribut, t.ex. textfärg, teckensnittsfamilj, kantlinje, utfyllnad, marginal. från **[!UICONTROL Component settings]** fönster.

   ![](assets/email_designer_12.png)

## Delare {#divider}

Använd **[!UICONTROL Divider]** om du vill infoga en delningslinje för att ordna layouten och innehållet i ditt e-postmeddelande.

Du kan justera formatattribut som linjefärg, format och höjd på menyn **[!UICONTROL Component settings]** fönster.

![](assets/email_designer_16.png)

## HTML {#HTML}

Använd **[!UICONTROL HTML]** om du vill kopiera och klistra in de olika delarna av din befintliga HTML. På så sätt kan du skapa kostnadsfria modulära HTML-komponenter för att återanvända externt innehåll.

1. Från **[!UICONTROL Content Components]**, dra och släpp **[!UICONTROL HTML]** till en **[!UICONTROL Structure component]**.

   ![](assets/email_designer_22.png)

1. Klicka på den nya komponenten och välj sedan **[!UICONTROL Show the source code]** från kontextverktygsfältet för att lägga till HTML.

   ![](assets/email_designer_23.png)

>[!NOTE]
>
>Adobe rekommenderar att du skapar ett meddelande från grunden och kopierar innehållet från ditt befintliga e-postmeddelande till komponenter, så att det externa innehållet helt enkelt blir kompatibelt med e-postdesignern.

## Bild {#image}

Använd **[!UICONTROL Image]** om du vill infoga en bildfil från datorn i e-postmeddelandet.

1. I **[!UICONTROL Content Components]**, dra och släppa **[!UICONTROL Image]** i en **[!UICONTROL Structure component]**.

   ![](assets/email_designer_9.png)

1. Klicka **[!UICONTROL Browse]** om du vill välja en bildfil bland dina resurser.

1. Klicka på den nya komponenten och ange bildegenskaperna med **[!UICONTROL Components settings]** ruta:

   * **[!UICONTROL Image title]** I kan du definiera en titel för bilden.
   * **[!UICONTROL Alt text]** I kan du definiera den bildtext som är länkad till bilden. Detta motsvarar attributet alt HTML.

   ![](assets/email_designer_10.png)

1. Justera övriga formatattribut som marginal, kant osv. eller lägga till en länk för att dirigera om målgruppen till ett annat innehåll från **[!UICONTROL Component settings]** fönster.

## Social {#social}

Använd **[!UICONTROL Social]** för att infoga länkar till sidor för sociala medier i ditt e-postinnehåll.

1. Från **[!UICONTROL Content Components]**, dra och släpp **[!UICONTROL Social]** till en **[!UICONTROL Structure component]**.

1. Klicka på den nya komponenten.

1. I **[!UICONTROL Social]** fält för **[!UICONTROL Components settings]** väljer du vilka sociala medier du vill lägga till eller ta bort.

   ![](assets/email_designer_20.png)

1. Välj storlek på ikonerna i dialogrutan **[!UICONTROL Size of images]** fält.

1. Klicka på var och en av dina ikoner för sociala medier för att konfigurera **[!UICONTROL URL]** som er målgrupp omdirigeras till.

   ![](assets/email_designer_21.png)

1. Du kan också ändra ikonerna för vart och ett av dina sociala medier om det behövs i **[!UICONTROL Image]** fält.

1. Justera övriga formatattribut, t.ex. format, marginal, kant. från **[!UICONTROL Component settings]** fönster.
