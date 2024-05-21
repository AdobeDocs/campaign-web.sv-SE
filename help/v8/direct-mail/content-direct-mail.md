---
audience: end-user
title: Designa direktutskick
description: Lär dig hur du utformar direktreklam med Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: 60484d08a68a5caaf91074c9ce543d8a44d44ab7
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# Utforma extraheringsfilen {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Extrahera filinnehåll"
>abstract="Klicka på **Redigera innehåll** för att börja designa extraheringsfilen som krävs av din direktmeddelandeleverantör. På så sätt kan du definiera filegenskaperna, till exempel filens etikett och format, och ange de kolumner som du vill inkludera i filen."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Filegenskaper"
>abstract="Konfigurera egenskaperna för extraheringsfilen, t.ex. dess namn och format. Du kan anpassa filnamnet med attribut från databasen med uttrycksredigeraren."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Innehåll"
>abstract="I det här avsnittet anger du vilka kolumner som ska visas i extraheringsfilen. När du är klar kan du förhandsgranska extraheringsfilen med **Simulera innehåll** -knappen."

Om du vill designa innehållet i extraheringsfilen som genereras av din direktutskick klickar du på knappen **[!UICONTROL Edit content]** på din leveranssida och sedan konfigurera filens egenskaper och innehåll.

## Konfigurera egenskaper för extraheringsfilen {#properties}

1. I **[!UICONTROL File name]** anger du ett namn för extraheringsfilen. Du kan anpassa filnamnet med attribut från databasen. Klicka på **[!UICONTROL Open personalization dialog]** -ikonen för att öppna uttrycksredigeraren. [Lär dig anpassa ditt innehåll](../personalization/personalize.md)

1. I **[!UICONTROL File format]** Välj önskat format för extraheringsfilen. **Text**, **Text med fast teckenbredd**, **CSV (Excel)** eller **XML**.

1. Expandera **[!UICONTROL Extraction format]** för att komma åt specifika alternativ för extraheringsfilens format. Vilka värden som är tillgängliga beror på det valda formatet.

+++ Tillgängliga alternativ för extraheringsformat

   * **[!UICONTROL Use first line as column header]** (Text-/CSV-format (Excel): Aktivera det här alternativet om du vill använda den första kolumnen som rubrik.
   * **[!UICONTROL Column separator]** (Textformat): Ange det tecken som ska användas som kolumnavgränsare i extraheringsfilen.
   * **[!UICONTROL String delimiter]** (Textformat): Ange hur strängar i extraheringsfilen ska avgränsas.
   * **[!UICONTROL End of line]** (Textformat): Ange hur radslut i extraheringsfilen ska avgränsas.
   * **[!UICONTROL Encoding]**: Välj kodning för extraheringsfilen.
   * **[!UICONTROL Date format and separators]**: Ange hur datum ska formateras i extraheringsfilen.
   * **[!UICONTROL Number format]**: Ange hur tal ska formateras i extraheringsfilen.
   * **[!UICONTROL Export labels instead of internal values of enumerations]**: Aktivera det här alternativet om du vill exportera uppräkningsvärden och om du vill hämta kolumnrubriker, som är lättare att förstå, i stället för interna ID:n.

+++

1. Växla på **[!UICONTROL Requested quantity]** för att begränsa antalet mottagare för leveransen.

   ![](assets/dm-content-details.png){zoomable="yes"}

## Konfigurera kolumnerna för extraheringsfilen {#content}

I **[!UICONTROL Content]** anger du de kolumner som ska visas i extraheringsfilen. Följ dessa steg för att göra detta:

1. Klicka på **[!UICONTROL Add Attribute]** för att skapa en ny kolumn.
1. Välj det attribut som ska visas i kolumnen och bekräfta. Observera att du kan använda uttrycksredigeraren för att välja vilket attribut som ska användas genom att klicka på **[!UICONTROL Edit expression]** -knappen.

   ![](assets/dm-add-attribute.png)

1. När kolumnen har lagts till kan du ändra dess etikett och tillhörande attribut med hjälp av redigeringsikonen.
1. Upprepa dessa steg om du vill lägga till så många kolumner som behövs för extraheringsfilen.
1. Om du vill sortera extraheringsfilen med en av kolumnerna klickar du på ikonen i dialogrutan **[!UICONTROL Sorting]** och väljer önskad sorteringsmetod.
1. Om du vill ändra en kolumns placering använder du upp- och nedpilarna.

![](assets/dm-content-attributes.png)

Nu kan du förhandsgranska extraheringsfilen och skicka leveransen för att generera extraheringsfilen. [Lär dig hur du testar och skickar direktreklam](send-direct-mail.md)
