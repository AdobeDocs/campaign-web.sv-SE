---
audience: end-user
title: Använda arbetsflödesaktiviteten Extrahera fil
description: Lär dig hur du använder arbetsflödesaktiviteten för Extract-filen
exl-id: fa50ab5b-2539-4517-9d7b-93315f1e505c
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---

# Extrahera fil {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Extrahera fil"
>abstract="Med aktiviteten **Extrahera fil** kan du exportera data från Adobe Campaign i form av en extern fil. Data kan sedan exporteras till en serverplats som SFTP, molnlagring eller kampanjservern med hjälp av en överföringsfilaktivitet."

Aktiviteten **Extrahera fil** är en **datahanteringsaktivitet**. Använd den här aktiviteten om du vill exportera data från Adobe Campaign i form av en extern fil. Data kan sedan exporteras till en serverplats som SFTP, molnlagring eller kampanjservern med hjälp av en överföringsfilaktivitet.

Om du vill konfigurera aktiviteten **Extrahera fil** lägger du till en **Extrahera fil**-aktivitet i arbetsflödet och följer sedan stegen nedan.

## Konfigurera filen som ska extraheras {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Fil att extrahera"
>abstract="Markera den fil som ska extraheras."

I avsnittet **[!UICONTROL File to extract]** kan du konfigurera filegenskaperna och de data som ska inkluderas.

![](../assets/extract-file-file.png)

1. I fältet **[!UICONTROL File name]** anger du önskat namn på filen som ska extraheras.

   Du kan anpassa filens namn med hjälp av händelsevariabler, villkor och datum/tid-funktioner. Klicka på ikonen **[!UICONTROL Open personalization dialog]** för att öppna uttrycksredigeraren. [Lär dig hur du arbetar med händelsevariabler och uttrycksredigeraren](../event-variables.md)

1. Ange de kolumner som ska finnas i den extraherade filen. Följ dessa steg för att göra detta:

   1. Klicka på **[!UICONTROL Add output column]**.
   1. Välj det attribut som ska visas i kolumnen och bekräfta. Vilka attribut som är tillgängliga beror på arbetsflödets måldimension. [Lär dig hur du väljer attribut och lägger till dem i favoriter](../../get-started/attributes.md)
   1. När kolumnen har lagts till kan du ändra dess **[!UICONTROL Label]** och tillhörande **[!UICONTROL Attribute]**.
   1. Om du vill använda en omformning på kolumnens värden, markerar du den i listrutan. Du kan till exempel växla alla värden i den markerade kolumnen till versaler.

1. Upprepa dessa steg om du vill lägga till så många kolumner som behövs i extraheringsfilen. Om du vill ändra en kolumns placering använder du upp- och nedpilarna.

1. Om du vill ta bort alla dubblettrader från den extraherade filen aktiverar du alternativet **[!UICONTROL Remove duplicate rows(Listing)]**.

1. Om du vill sortera den extraherade filen baserat på ett attribut växlar du på alternativet **[!UICONTROL Enable Sorting]** och väljer sedan det attribut som du vill sortera filen efter, tillsammans med önskad sorteringsmetod (stigande eller fallande). Du kan sortera efter vilket attribut som helst från den aktuella måldimensionen, oavsett om det har lagts till i filens kolumner eller inte.

## Konfigurera det extraherade filformatet {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Målformat"
>abstract="Välj de olika alternativen för att konfigurera hur den extraherade filen ska formateras."

I formatavsnittet **[!UICONTROL Destination]** kan du konfigurera hur den extraherade filen ska formateras.

1. Välj **[!UICONTROL Output format]** för den extraherade filen: **Text**, **Text som använder fasta kolumner**, **CSV (Excel)** eller **XML**.

1. Klicka på knappen **[!UICONTROL Extraction format]** om du vill visa specifika alternativ för det valda formatet. Expandera avsnittet nedan om du vill ha mer information.

+++ Tillgängliga alternativ för extraheringsformat

   * **[!UICONTROL Use first line as column header]** (Text-/CSV-format (Excel)): Aktivera det här alternativet om du vill använda den första kolumnen som rubrik.
   * **[!UICONTROL Column separator]** (Textformat): Ange tecknet som ska användas som kolumnavgränsare i utdatafilen.
   * **[!UICONTROL String delimiter]** (Textformat): Ange hur strängar i utdatafilen ska avgränsas.
   * **[!UICONTROL End of line]** (Textformat): Ange hur radslut i utdatafilen ska avgränsas.
   * **[!UICONTROL Encoding]**: Välj kodning för utdatafilen.
   * **[!UICONTROL Date format and separators]**: Ange hur datum ska formateras i utdatafilen.
   * **[!UICONTROL Number format]**: Ange hur tal ska formateras i utdatafilen.
   * **[!UICONTROL Export labels instead of internal values of enumerations]**: Aktivera det här alternativet om du vill exportera uppräkningsvärden och om du vill hämta kolumnrubriker som är lättare att förstå, i stället för interna ID:n.

+++

   ![](../assets/extract-file-format.png)

## Lägga till ett efterbearbetningsstadium {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Efterbearbetning"
>abstract="Definiera ett steg för efterbearbetning som ska användas, till exempel för komprimering eller kryptering."

Med **[!UICONTROL Export modification script]** kan du använda en bearbetningsfas som ska köras under dataextraheringen, till exempel zipping (komprimering) eller encryption (kryptering). Klicka på knappen **[!UICONTROL Edit script]** om du vill göra det.

Uttrycksredigeraren öppnas och du kan ange det kommando som ska användas för filen. Den vänstra rutan innehåller fördefinierade syntaxer som du kan använda för att skapa skriptet. [Lär dig hur du arbetar med händelsevariabler och uttrycksredigeraren](../event-variables.md)

![](../assets/extract-file-script.png)

## Ytterligare alternativ {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Utgående övergång"
>abstract="Växla alternativet **Generera en utgående övergång** om du vill lägga till en utgående övergång efter den aktuella aktiviteten."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Processfel"
>abstract="Växla alternativet **Processfel** om du vill lägga till en utgående övergång som innehåller fel."

När extraheringen av utdatafilen har konfigurerats finns ytterligare alternativ för övergångar och felhantering:

* **[!UICONTROL Generate outbound transition]**: Aktivera det här alternativet om du vill lägga till en utgående övergång och konfigurera dess etikett.
* **[!UICONTROL Do not generate a file if the inbound transition is empty]**: Aktivera det här alternativet om du vill hoppa över filextraheringen om den inkommande övergången inte innehåller några data.
* **[!UICONTROL Process error]**: Aktivera det här alternativet om du vill lägga till en utgående övergång om något fel inträffar under filextraheringen.

## Exempel {#example}

I följande exempel använder vi en **Skapa målgrupp**-aktivitet följt av en **Extrahera fil**-aktivitet för att extrahera alla målprofiler till en CSV-fil.

![](../assets/extract-file-example.png)

* Fältet **[!UICONTROL File name]** är konfigurerat att inkludera datumet för extraheringen.

  ![](../assets/extract-file-example-name.png)

* Kolumner läggs till för att visa profilernas för- och efternamn, deras kund-ID och datum när de skapades i databasen.

  ![](../assets/extract-file-example-columns.png)
