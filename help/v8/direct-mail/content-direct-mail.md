---
audience: end-user
title: Designa direktutskick
description: Lär dig hur du utformar direktreklam med Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 1%

---

# Utforma extraheringsfilen {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Extrahera filinnehåll"
>abstract="Klicka på knappen **Redigera innehåll** för att börja designa den extraheringsfil som krävs av din direktmeddelandeleverantör. På så sätt kan du definiera filegenskaperna, till exempel filens etikett och format, och ange de kolumner som du vill inkludera i filen."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Filegenskaper"
>abstract="Konfigurera egenskaperna för extraheringsfilen, till exempel dess namn och format. Du kan anpassa filnamnet med attribut från databasen med hjälp av uttrycksredigeraren."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Innehåll"
>abstract="I det här avsnittet anger du vilka kolumner som ska visas i extraheringsfilen. När du är klar kan du förhandsgranska extraheringsfilen med knappen **Simulera innehåll** ."

Om du vill designa innehållet i extraheringsfilen som genereras av din direktmeddelandeleverans klickar du på knappen **[!UICONTROL Edit content]** på leveranssidan och konfigurerar sedan filegenskaperna och innehållet.

## Konfigurera egenskaper för extraheringsfilen {#properties}

1. I fältet **[!UICONTROL File name]** anger du önskat namn för extraheringsfilen. Du kan anpassa filnamnet med attribut från databasen. Klicka på ikonen **[!UICONTROL Open personalization dialog]** för att öppna uttrycksredigeraren. [Lär dig anpassa ditt innehåll](../personalization/personalize.md)

1. I fältet **[!UICONTROL File format]** väljer du önskat format för extraheringsfilen: **Text**, **Text som använder kolumner med fast bredd**, **CSV (Excel)** eller **XML**.

1. Expandera avsnittet **[!UICONTROL Extraction format]** för att få åtkomst till specifika alternativ som är relaterade till extraheringsfilens format. Vilka värden som är tillgängliga beror på det valda formatet.

   +++ Tillgängliga alternativ för extraheringsformat

   * **[!UICONTROL Use first line as column header]** (Text-/CSV-format (Excel)): Aktivera det här alternativet om du vill använda den första kolumnen som rubrik.
   * **[!UICONTROL Column separator]** (Textformat): Ange det tecken som ska användas som kolumnavgränsare i extraheringsfilen.
   * **[!UICONTROL String delimiter]** (Textformat): Ange hur strängar i extraheringsfilen ska avgränsas.
   * **[!UICONTROL End of line]** (Textformat): Ange hur radslut i extraheringsfilen ska avgränsas.
   * **[!UICONTROL Encoding]**: Välj kodning för extraheringsfilen.
   * **[!UICONTROL Date format and separators]**: Ange hur datum ska formateras i extraheringsfilen.
   * **[!UICONTROL Number format]**: Ange hur tal ska formateras i extraheringsfilen.
   * **[!UICONTROL Export labels instead of internal values of enumerations]**: Växla det här alternativet på om du exporterar uppräkningsvärden och vill hämta kolumnetiketter, som är lättare att förstå, i stället för interna ID:n.

   +++

1. Växla på alternativet **[!UICONTROL Requested quantity]** om du vill begränsa antalet mottagare för leveransen.

   ![Skärmbild som visar konfigurationsalternativen för innehållsinformation för extraheringsfilen.](assets/dm-content-details.png){zoomable="yes"}

## Konfigurera kolumnerna för extraheringsfilen {#content}

I avsnittet **[!UICONTROL Content]** anger du vilka kolumner som ska visas i extraheringsfilen. Följ dessa steg för att göra detta:

1. Klicka på knappen **[!UICONTROL Add Attribute]** för att skapa en ny kolumn.
1. Välj det attribut som ska visas i kolumnen och bekräfta sedan. Observera att du kan använda uttrycksredigeraren för att välja attributet genom att klicka på knappen **[!UICONTROL Edit expression]**. [Lär dig hur du väljer attribut och lägger till dem i favoriter](../get-started/attributes.md)

   ![Skärmbild med knappen Lägg till attribut och alternativ för att lägga till attribut i extraheringsfilen.](assets/dm-add-attribute.png)

1. När kolumnen har lagts till kan du ändra dess etikett och det tillhörande attributet med hjälp av redigeringsikonen.
1. Upprepa dessa steg om du vill lägga till så många kolumner som behövs för extraheringsfilen.
1. Om du vill sortera extraheringsfilen med en av kolumnerna klickar du på ikonen i kolumnen **[!UICONTROL Sorting]** och väljer önskad sorteringsmetod.
1. Om du vill ändra en kolumns placering använder du upp- och nedpilarna.

![Skärmbild som visar attributkonfigurationsalternativen för extraheringsfilen.](assets/dm-content-attributes.png)

Nu kan du förhandsgranska extraheringsfilen och skicka leveransen för att generera extraheringsfilen. [Lär dig hur du testar och skickar direktmeddelanden](send-direct-mail.md)