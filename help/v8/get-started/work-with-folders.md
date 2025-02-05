---
audience: end-user
title: Arbeta med mappar
description: Lär dig hantera en mapp i Adobe Campaign
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Arbeta med mappar {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="Mappegenskaper"
>abstract="Mappegenskaper"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="Mappsäkerhet"
>abstract="Mappsäkerhet"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="Mappbegränsningar"
>abstract="Mappbegränsningar"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="Mappschema"
>abstract="Mappschema"

## Om mappar {#about-folders}

Mappar är objekt i Adobe Campaign som gör att du kan ordna komponenter och data.

Du kan skapa, byta namn på, ordna om och flytta mappar i navigeringsträdet. Du kan även ta bort dem enligt dina rättigheter.

![](assets/folders.png){zoomable="yes"}

Du kan ställa in en mapptyp. Exempel: en mapp med leveranser.
Mappens ikon ändras beroende på den här typen.

## Skapa en ny mapp {#create-a-folder}

Så här skapar du en ny mapp i Adobe Campaign Web UI:

1. I **[!UICONTROL Explorer]** går du till den mapp där du vill skapa den nya mappen.
Under menyn **[!UICONTROL ...]** har du **[!UICONTROL Create new folder]**

![](assets/folder_create.png){zoomable="yes"}

När du skapar en ny mapp är mapptypen som standard den överordnade mappens typ. I vårt exempel skapar vi en mapp i mappen **[!UICONTROL Deliveries]**.

![](assets/folder_new.png){zoomable="yes"}

1. Ändra typ av mapp genom att klicka på ikonen för mapptyp om det behövs och välj den i listan nedan:

![](assets/folder_type.png){zoomable="yes"}

Konfigurera mapptypen genom att klicka på knappen **[!UICONTROL Confirm]**.

Om du vill skapa en mapp utan en viss typ väljer du typen **[!UICONTROL Generic Folder]**.

Du kan även [skapa och hantera mappar i Adobe Campaign-konsolen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/folders-and-views).


## Ordna om mappar {#reorder-folders}

Du kan ordna om mapparna efter behov. Om du vill göra det klickar du på **[!UICONTROL Reorder folders]** enligt nedan.

I vårt exempel innehåller mappen **Leveranser** 4 mappar.

![](assets/folder-reorder.png){zoomable="yes"}

Du kan ändra ordningen på mapparna antingen genom att **dra och släppa** eller genom att använda **upp- och nedpilarna**.

![](assets/folder-draganddrop.png){zoomable="yes"}


## Ta bort en mapp {#delete-a-folder}

>[!CAUTION]
>
>När du tar bort en mapp tas även alla data som lagras i mappen bort.

Om du vill ta bort en mapp markerar du den i ditt **[!UICONTROL Explorer]**-träd och klickar på menyn **[!UICONTROL ...]**.
Välj **[!UICONTROL Delete folder]**.

![](assets/folder_delete.png){zoomable="yes"}

## Distribution av värden i en mapp {#distribution-values-folder}

Värdefördelningen gör det lättare att känna till procentandelen av ett värde i en kolumn i en tabell.

Om du vill veta hur värden distribueras i en mapp gör du så här:

Bland leveranserna vill vi till exempel veta hur värdena i kolumnen **Kanal** är fördelade.

Om du vill hämta den här informationen går du till mappen **[!UICONTROL Deliveries]** och klickar på ikonen **[!UICONTROL Configure columns]** .

I fönstret **[!UICONTROL Configure columns]** klickar du på ikonen **[!UICONTROL Information]** för den kolumn du vill veta. Klicka sedan på knappen **[!UICONTROL Distribution of values]**.

![](assets/values_deliveries.png){zoomable="yes"}

Du får procentandelen av värdena i kolumnen **[!UICONTROL Channel]**.

![](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
> För kolumner med många värden visas bara de första tjugo värdena. Ett meddelande från **[!UICONTROL Partial load]** varnar dig.

Du kan också distribuera värden för en länk.

Klicka på knappen **+** bredvid den önskade länken i attributlistan, enligt nedan. Detta lägger till länken till **[!UICONTROL Output columns]**. Nu kan du ha ikonen **[!UICONTROL Information]**, som gör att du kan visa fördelningen av dess värden. Om du inte vill behålla länken i **[!UICONTROL Output columns]** måste du klicka på knappen **[!UICONTROL Cancel]**.

![](assets/values_link.png){zoomable="yes"}

Det går också att distribuera värden i en frågemodellerare. [Läs mer här](../query/build-query.md#distribution-of-values-in-a-query).

### Filtrera värdena {#filter-values}

Genom att använda **[!UICONTROL Advanced filters]** i fönstret för värdedistribution kan du filtrera dina resultat baserat på angivna villkor.

I exemplet med leveranslistan ovan, som visar fördelningen per kanal, kan du till exempel filtrera den så att endast leveranser som har statusen **Slutförd** visas.

![](assets/values_filter.png){zoomable="yes"}
