---
audience: end-user
title: Använda e-postdesigners innehållskomponenter
description: Lär dig hur du använder innehållskomponenter i e-postmeddelanden
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '1296'
ht-degree: 0%

---

# Använda innehållskomponenter {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Om innehåll"
>abstract="Innehållskomponenterna är tomma platshållare för innehåll som du kan använda för att skapa layouten för ett e-postmeddelande."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Om innehåll"
>abstract="Innehållskomponenterna är tomma platshållare för innehåll som du kan använda för att skapa layouten för en landningssida."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Om innehåll"
>abstract="Innehållskomponenter är tomma platshållare för innehåll som du kan använda för att skapa layouten för ett innehållsfragment."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Om innehåll"
>abstract="Innehållskomponenter är tomma platshållare för innehåll som du kan använda för att skapa layouten för en mall."

När du skapar ditt e-postinnehåll kan du med **[!UICONTROL Content]**-komponenter anpassa din e-post med tomma komponenter som du kan använda en gång i ett e-postmeddelande.

Du kan lägga till så många **[!UICONTROL Contents]** som behövs inuti en **[!UICONTROL Structure]** som definierar layouten för ditt e-postmeddelande.

## Lägg till innehållskomponenter {#add-content-components}

Följ stegen nedan för att lägga till innehållskomponenter i e-postmeddelanden och anpassa dem efter dina behov.

1. Använd ett [befintligt innehåll](existing-content.md) eller dra och släpp en **[!UICONTROL Structure]** i ditt tomma innehåll för att definiera layouten för e-postmeddelandet i e-postmeddelandet. [Lär dig hur](create-email-content.md)

1. Dra och släpp **[!UICONTROL Content]** i de relevanta strukturerna.

   ![Skärmbild som visar hur du drar och släpper innehållskomponenter i strukturer i e-postens Designer.](assets/email_designer_add_content_components.png){zoomable="yes"}

   >[!NOTE]
   >
   >Du kan lägga till flera komponenter i en enda struktur och i varje kolumn i en struktur.

1. Justera alternativen för varje komponent med hjälp av fliken **[!UICONTROL Settings]**. Du kan till exempel välja att visa den enbart på stationära eller mobila enheter, eller både och. Du kan också hantera länkalternativ på den här fliken. [Läs mer om att hantera länkar](message-tracking.md)

1. Justera formatattributen för varje komponent på fliken **[!UICONTROL Style]**. Du kan till exempel ändra textstil, utfyllnad eller marginal för varje komponent. [Läs mer om justering och utfyllnad](alignment-and-padding.md)

   ![Skärmbild som visar inställningsfliken för innehållskomponenter i e-post-Designer.](assets/email_designer_content_components_settings.png){zoomable="yes"}

1. Ta bort eller duplicera en innehållskomponent efter behov på den avancerade menyn i **[!UICONTROL Content]** på den högra panelen.

## Behållare {#container}

Du kan lägga till en enkel behållare i vilken du lägger till en annan innehållskomponent. På så sätt kan du använda en särskild formatering för behållaren, vilket skiljer sig från den komponent som används inuti.

Lägg till exempel till en **[!UICONTROL Container]**-komponent och lägg sedan till en [ Button](#button) -komponent i den behållaren. Använd en specifik bakgrund för behållaren och en annan för knappen.

![Skärmbild som visar hur du lägger till en behållarkomponent i e-post-Designer.](assets/email_designer_container_component.png){zoomable="yes"}

## Knapp {#buttons}

Använd komponenten **[!UICONTROL Button]** för att infoga en eller flera knappar i e-postmeddelandet och dirigera om din e-postmålgrupp till en annan sida.

1. Dra och släpp **[!UICONTROL Button]**-komponenten från listan **[!UICONTROL Contents]** till en **[!UICONTROL Structure]**-komponent.

   ![Skärmbild som visar hur du drar och släpper en knappkomponent i e-post-Designer.](assets/email_designer_13.png){zoomable="yes"}

1. Klicka på den nyligen tillagda knappen om du vill anpassa texten och komma åt flikarna **[!UICONTROL Settings]** och **[!UICONTROL Styles]**.

   ![Skärmbild som visar inställningsfliken för knappkomponenter i e-post-Designer.](assets/email_designer_14.png){zoomable="yes"}

1. På fliken **[!UICONTROL Settings]** i fältet **[!UICONTROL URL]** lägger du till den URL som ska omdirigeras när du klickar på knappen.

1. Välj hur innehållet ska visas i den nedrullningsbara listan **[!UICONTROL Target]**:

   * **[!UICONTROL None]**: öppnar länken i samma ram som den klickades på (standard).
   * **[!UICONTROL Blank]**: öppnar länken i ett nytt fönster eller på en ny flik.
   * **[!UICONTROL Self]**: öppnar länken i samma ram som den klickades på.
   * **[!UICONTROL Parent]**: öppnar länken i den överordnade ramen.
   * **[!UICONTROL Top]**: öppnar länken i hela fönstrets brödtext.

   ![Skärmbild som visar målalternativen för knappkomponenter i e-post-Designer.](assets/email_designer_15.png){zoomable="yes"}

1. Anpassa knappen ytterligare genom att ändra formatattribut som **[!UICONTROL Border]**, **[!UICONTROL Size]**, **[!UICONTROL Margin]** och andra på fliken **[!UICONTROL Styles]**.

## Text {#text}

Använd komponenten **[!UICONTROL Text]** för att infoga text i e-postmeddelandet och justera formatet (kantlinje, storlek, utfyllnad osv.) med flikarna **[!UICONTROL Settings]** och **[!UICONTROL Styles]**.

1. Dra och släpp **[!UICONTROL Text]** från menyn **[!UICONTROL Contents]** till en **[!UICONTROL Structure]**-komponent.

   ![Skärmbild som visar hur du drar och släpper en textkomponent i e-post-Designer.](assets/email_designer_11.png){zoomable="yes"}

1. Klicka på den nya komponenten som du har lagt till för att anpassa texten och komma åt flikarna **[!UICONTROL Settings]** och **[!UICONTROL Styles]**.

1. Ändra texten med följande alternativ i det sammanhangsberoende verktygsfältet:

   ![Skärmbild som visar verktygsfältet för textredigering i e-post-Designer.](assets/email_designer_27.png){zoomable="yes"}

   * **[!UICONTROL Change text style]**: Använd fet, kursiv, understrykning eller genomstrykning i texten.
   * **Ändra justering**: välj mellan vänsterjustering, högerjustering, centrering eller marginaljustering för texten.
   * **[!UICONTROL Create list]**: lägg till punkt- eller nummerlistor i texten.
   * **[!UICONTROL Set heading]**: lägg till upp till sex rubriknivåer i texten.
   * **Teckensnittsstorlek**: välj teckensnittsstorleken för texten i pixlar.
   * **[!UICONTROL Edit image]**: lägg till en bild eller en resurs i textkomponenten.
   * **[!UICONTROL Show the source code]**: visa källkoden för texten. Den kan inte ändras.
   * **[!UICONTROL Duplicate]**: lägg till en kopia av textkomponenten.
   * **[!UICONTROL Delete]**: ta bort den markerade textkomponenten från e-postmeddelandet.
   * **[!UICONTROL Add personalization]**: lägg till anpassningsfält för att anpassa innehållet från dina profildata.
   * **[!UICONTROL Enable conditional content]**: lägg till villkorligt innehåll för att anpassa komponentens innehåll till målprofilerna.

1. Justera andra formateringsattribut, till exempel textfärg, teckensnittsfamilj, kantlinje, utfyllnad, marginal och andra på fliken **[!UICONTROL Styles]**.

   ![Skärmbild som visar formatfliken för textkomponenter i e-post-Designer.](assets/email_designer_12.png){zoomable="yes"}

## Delare {#divider}

Använd komponenten **[!UICONTROL Divider]** för att infoga en delningslinje för att ordna layouten och innehållet i ditt e-postmeddelande.

Du kan justera formatattribut som linjefärg, format och höjd på fliken **[!UICONTROL Styles]**.

![Skärmbild som visar hur du lägger till en avdelarkomponent i e-postens Designer.](assets/email_designer_16.png){zoomable="yes"}

## HTML {#HTML}

Använd komponenten **[!UICONTROL HTML]** för att kopiera och klistra in delar av din befintliga HTML. På så sätt kan du skapa kostnadsfria modulära HTML-komponenter för att återanvända externt innehåll.

1. Dra och släpp **[!UICONTROL HTML]**-komponenten från **[!UICONTROL Components]** till en **[!UICONTROL Structure]**-komponent.

   ![Skärmbild som visar hur du drar och släpper en HTML-komponent i e-post-Designer.](assets/email_designer_22.png){zoomable="yes"}

1. Klicka på den nya komponenten och välj sedan **[!UICONTROL Show the source code]** i det sammanhangsberoende verktygsfältet för att lägga till din HTML.

   ![Skärmbild som visar källkodsalternativet för HTML-komponenter i e-post-Designer.](assets/email_designer_23.png){zoomable="yes"}

>[!NOTE]
>
>Om du vill att externt innehåll ska vara kompatibelt med e-post-Designer rekommenderar Adobe att [skapa ett meddelande från början](create-email-content.md) och kopiera innehållet från din befintliga e-post till komponenter.

## Bild {#image}

>[!IMPORTANT]
>
>Åtkomsten till Assets-menyn är begränsad till användare som har en aktiv Adobe Experience Manager as a Cloud Service-licens. Om du inte har den här licensen är Assets-menyn inte tillgänglig.

Använd komponenten **[!UICONTROL Image]** för att infoga en bildfil från datorn i e-postmeddelandet.

1. Dra och släpp **[!UICONTROL Image]** från menyn **[!UICONTROL Content]** till en **[!UICONTROL Structure]**-komponent.

   ![Skärmbild som visar hur du drar och släpper en bildkomponent i e-postprogrammet Designer.](assets/email_designer_9.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Browse]** om du vill välja en bildfil bland dina resurser. Du kan också välja att **[!UICONTROL Import your media]**.

   Mer information om hur du överför och lägger till resurser i Adobe Experience Manager finns i [Adobe Experience Manager as a Cloud Service-dokumentationen](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html).

   ![Skärmbild som visar bläddringsalternativet för bildkomponenter i e-post-Designer.](assets/email_designer_28.png){zoomable="yes"}

1. Navigera i mapparna för att hitta den resurs du behöver, eller använd sökfältet för att hitta den effektivt.

   Klicka på **[!UICONTROL Select]** när du har hittat resursen du söker efter.

   ![Skärmbild som visar resursurvalsprocessen i e-post-Designer.](assets/email_designer_29.png){zoomable="yes"}

1. Klicka på den nya komponenten och ange bildegenskaper på fliken **[!UICONTROL Settings]**:

   * Med **[!UICONTROL Image title]** kan du definiera en titel för bilden.
   * Med **[!UICONTROL Alt text]** kan du definiera bildtexten som är länkad till bilden. Detta motsvarar alt-HTML-attributet.

   ![Skärmbild som visar inställningsfliken för bildkomponenter i e-post-Designer.](assets/email_designer_10.png){zoomable="yes"}

1. Lägg till en länk för att dirigera om er målgrupp till ett annat innehåll. [Läs mer](message-tracking.md)

1. Justera andra formatattribut, till exempel marginal, kant och andra, med fliken **[!UICONTROL Styles]**.

## Social {#social}

Använd komponenten **[!UICONTROL Social]** för att infoga länkar till sidor för sociala medier i ditt e-postinnehåll.

1. Dra och släpp **[!UICONTROL Social]**-komponenten i en **[!UICONTROL Structure]** -komponent från menyn **[!UICONTROL Components]**.

1. Klicka på den nya komponenten.

1. I fältet **[!UICONTROL Social]** på fliken **[!UICONTROL Settings]** väljer du vilka sociala medier du vill lägga till eller ta bort.

   ![Skärmbild som visar inställningsfliken för sociala komponenter i e-post-Designer.](assets/email_designer_20.png){zoomable="yes"}

1. Välj storleken på ikonerna i fältet **[!UICONTROL Size of images]**.

1. Klicka på var och en av dina ikoner för sociala medier för att konfigurera **[!UICONTROL URL]** som din målgrupp omdirigeras till.

   ![Skärmbild som visar URL-konfigurationen för ikoner för sociala medier i e-post-Designer.](assets/email_designer_21.png){zoomable="yes"}

1. Ändra ikonerna för alla dina sociala medier om det behövs i fältet **[!UICONTROL Source]**.

1. Justera andra formatattribut, till exempel format, marginal, kant och andra på fliken **[!UICONTROL Styles]**.