---
title: Konfigurera [!DNL Campaign] alternativ
description: Lär dig konfigurera Campaign-alternativ och skapa egna anpassade alternativ.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Konfigurera alternativ för [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Alternativ"
>abstract="Alternativ"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Alternativet Skapa"
>abstract="Alternativet Skapa"

Adobe Campaign Web innehåller tekniska alternativ som gör att du kan konfigurera programmet mer specifikt. Vissa av dessa alternativ är inbyggda, medan andra kan läggas till manuellt efter behov.

>[!IMPORTANT]
>
>Inbyggda alternativ är förkonfigurerade och bör endast ändras av avancerade användare. Om du har några frågor eller frågor kan du kontakta Adobe.

## Åtkomst till kampanjalternativ {#access}

Det finns alternativ på menyn **[!UICONTROL Administration]** / **[!UICONTROL Options]**. Använd filterpanelen för att begränsa listan och snabbt hitta det alternativ du behöver.

![](assets/options-list.png)

>[!NOTE]
>
>Även om alternativmenyns placering skiljer sig mellan Adobe Campaign konsol och webbgränssnittet är listan identisk och fungerar som en spegel. Mer information om de tillgängliga alternativen finns i listan med alternativ i [dokumentationen för Campaign v7](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}

I alternativlistan kan du:

* **Duplicera eller ta bort ett alternativ**: Klicka på ellipsknappen och välj önskad åtgärd.
* **Ändra ett alternativ**: Klicka på alternativets namn för att öppna dess egenskaper. Gör ändringarna och spara.
* **Skapa ett anpassat alternativ**: Klicka på knappen **[!UICONTROL Create option]**.

## Skapa ett alternativ {#create}

Med Adobe Campaign webbgränssnitt kan du skapa egna alternativ som passar dina behov. Detta är särskilt användbart när du arbetar med **[!UICONTROL JavaScript code]**-arbetsflödesaktiviteter för att lagra mellanliggande data.

Så här skapar du ett alternativ:

1. Öppna alternativlistan och klicka på **[!UICONTROL Create option]**.
1. Ange ett namn för alternativet, markera dess typ och ange det önskade värdet.
1. Klicka på **[!UICONTROL Create]** för att skapa alternativet.

   ![](assets/options-create.png)

Alternativ kan fungera som ett tillfälligt lagringsutrymme för data och ge följande fördelar:

* Typade värden: Alternativ har stöd för särskilda datatyper, t.ex. datum, heltal, strängar...
* Flexibilitet: Med alternativen kan användare lagra och hämta data effektivt utan att behöva hantera databastabeller.

I exemplet nedan skapar vi ett anpassat alternativ med namnet `sampleOption` och det inledande värdet a. En **[!UICONTROL JavaScript code]**-aktivitet i ett arbetsflöde ändrar det här alternativets värde och lagrar det i en variabel. Det uppdaterade värdet visas i arbetsflödesloggarna och återspeglas på menyn **[!UICONTROL Options]**.

1. Skapa alternativet.

   ![](assets/options-sample-create.png)

1. Konfigurera en **[!UICONTROL JavaScript code]**-aktivitet och starta arbetsflödet.

   ![](assets/options-sample-javascript.png)

1. Kör arbetsflödet för att se det uppdaterade värdet i arbetsflödesloggarna.

   ![](assets/options-sample-logs.png)

1. Det uppdaterade värdet visas nu på menyn **[!UICONTROL Options]**.

   ![](assets/options-sample-updated.png)
