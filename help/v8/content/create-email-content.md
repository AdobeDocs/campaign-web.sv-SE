---
audience: end-user
title: Designa e-postmeddelanden i Journey Optimizer
description: Lär dig designa e-postinnehåll från grunden
source-git-commit: 9def5ea791e4ef42968cd34536f3ddeac7fc238c
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---


# Börja från början {#create-email-content}

>[!NOTE]
>
>Dokumentationen håller på att byggas och uppdateras ofta. Den slutliga versionen av detta innehåll är klar i januari 2023.

>[!CONTEXTUALHELP]
>id="ac_structure_components_email"
>title="Om strukturkomponenter"
>abstract="Strukturkomponenter definierar layouten för e-postmeddelandet."

>[!CONTEXTUALHELP]
>id="ac_structure_components_landing_page"
>title="Om strukturkomponenter"
>abstract="Strukturkomponenter definierar landningssidans layout."

>[!CONTEXTUALHELP]
>id="ac_structure_components_fragment"
>title="Om strukturkomponenter"
>abstract="Strukturkomponenter definierar fragmentets layout."

>[!CONTEXTUALHELP]
>id="ac_structure_components_template"
>title="Om strukturkomponenter"
>abstract="Strukturkomponenter definierar mallens layout."


>[!CONTEXTUALHELP]
>id="ac_edition_columns_email"
>title="Definiera e-postkolumner"
>abstract="Med e-postdesignern kan du enkelt definiera layouten för e-postmeddelandet genom att definiera kolumnstrukturen."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_landing_page"
>title="Definiera landningssidans kolumner"
>abstract="Med e-postdesignern kan du enkelt definiera layouten för landningssidan genom att definiera kolumnstrukturen."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_fragment"
>title="Definiera fragmentkolumner"
>abstract="Med e-postdesignern kan du enkelt definiera fragmentets layout genom att definiera kolumnstrukturen."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_template"
>title="Definiera mallkolumner"
>abstract="Med e-postdesignern kan du enkelt definiera mallens layout genom att definiera kolumnstrukturen."

Med e-postdesignern kan du enkelt definiera e-postens struktur. Genom att lägga till och flytta strukturella element med enkla dra-och-släpp-åtgärder kan du designa formen på e-postmeddelandet på några sekunder.

Följ stegen nedan för att börja skapa e-postinnehåll med e-postdesignern:

1. På e-postdesignerns hemsida väljer du **[!UICONTROL Design from scratch]** alternativ.

   ![](assets/email_designer.png)

1. Börja designa e-postinnehåll genom att dra och släppa **[!UICONTROL Structure components]** för att definiera layouten för e-postmeddelandet.

   >[!NOTE]
   >
   >Observera att stapeln med kolumner inte är kompatibel med alla e-postprogram. Om det inte finns stöd för det här alternativet staplas inte kolumner.
   >
   >När du har placerat i e-postmeddelandet kan du inte flytta eller ta bort dina komponenter om det inte redan finns en innehållskomponent eller ett fragment inuti.

   ![](assets/email_designer_2.png)

1. Lägg till så många **[!UICONTROL Structure components]** efter behov.

   Välj **[!UICONTROL n:n column]** -komponent för att definiera hur många kolumner du vill ha (mellan 3 och 10). Du kan också definiera bredden på varje kolumn genom att flytta pilarna längst ned i varje kolumn.

   >[!NOTE]
   >
   >Varje kolumnstorlek får inte vara mindre än 10 % av strukturkomponentens totala bredd. Du kan inte ta bort en kolumn som inte är tom.

1. Från **[!UICONTROL Content components]** nedrullningsbar meny, du kan lägga till så många **[!UICONTROL Content components]** som du behöver i strukturkomponenten. [Läs mer om innehållskomponenter](content-components.md).

   ![](assets/email_designer_3.png)

1. Varje komponent kan anpassas ytterligare med **[!UICONTROL Component settings]** -avsnitt. Du kan till exempel ändra textstil, utfyllnad eller marginal för komponenten. [Läs mer om justering och utfyllnad](adjusting-vertical-alignment-and-padding.md).

   ![](assets/email_designer_4.png)

1. Från **[!UICONTROL Assets picker]** kan du lägga till resurser som lagras i **[!UICONTROL Assets library]** till din e-postadress.

   Dubbelklicka på den mapp som innehåller dina resurser och dra och släpp den resurs som du vill lägga till i e-postmeddelandet.

   ![](assets/email_designer_5.png)

1. Lägg till anpassningsfält för att anpassa innehållet utifrån dina profildata.

   ![](assets/email_designer_6.png)

1. Lägg till dynamiskt innehåll för att anpassa innehållet till målprofilerna baserat på villkorliga regler.

   ![](assets/email_designer_dynamic-content.png)

1. I **[!UICONTROL Links]** i den vänstra rutan kontrollerar du listan med alla URL:er för ditt innehåll som ska spåras. Du kan ändra deras **[!UICONTROL Tracking Type]**, **[!UICONTROL Label]** och **[!UICONTROL Tags]** vid behov.

   ![](assets/email_designer_7.png)

   >[!NOTE]
   >
   >Läs mer om länkar och meddelandespårning i [den här sidan](message-tracking.md).

1. Om det behövs kan du växla till kodredigeraren för att anpassa e-postmeddelandet ytterligare genom att klicka på **[!UICONTROL Switch to code editor]** på den avancerade menyn. Mer information om kodredigeraren finns i [den här sidan](code-content.md#).

   >[!NOTE]
   >
   >Du kommer inte att kunna använda den visuella designern för det här e-postmeddelandet när du har växlat till kodredigeraren.

   ![](assets/email_designer_26.png)

1. Klicka **[!UICONTROL Show preview]** för att kontrollera din e-poståtergivning. Du kan välja skrivbordsvy eller mobilvy.

   ![](assets/email_designer_8.png)

1. När e-postmeddelandet är klart klickar du på **[!UICONTROL Save & Close]**.
