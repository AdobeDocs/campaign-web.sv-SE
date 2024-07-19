---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 45cdd310-7c0c-4b57-bb7f-0576d8eca19d
source-git-commit: 70028ebe3e87498a5ef5778838491d8f964e8e87
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Lägg till inbyggda innehållsblock {#ootb-content-blocks}

Adobe Campaign erbjuder en lista med förkonfigurerade innehållsblock. Dessa innehållsblock är dynamiska, personaliserade och har en specifik rendering som du kan infoga i leveranserna. Du kan till exempel lägga till en logotyp, ett gratulationsmeddelande eller en länk till en spegelsida.

Så här lägger du till ett innehållsblock i en leverans:

1. Öppna en leverans och redigera innehållet.

1. Leta reda på fältet där du vill lägga till ett innehållsblock och klicka på ikonen **[!UICONTROL Open personalization dialog]** för att öppna uttrycksredigeraren.

   ![](assets/content-block-access.png){zoomable="yes"}{width="800" align="center"}

1. I uttrycksredigeraren bläddrar du till den vänstra menyn **[!UICONTROL Content blocks]**.

1. Om du vill lägga till ett innehållsblock placerar du markören på önskad plats i innehållet och infogar det genom att klicka på plusknappen (+).

   ![](assets/content-blocks.png){zoomable="yes"}{width="800" align="center"}

Inbyggda innehållsblock är:

* **[!UICONTROL Default opt-out banner]**
* **[!UICONTROL Enabled by Adobe Campaign]**: infogar logotypen&quot;Enabled by Adobe Campaign&quot;.
* **[!UICONTROL Formatting function for proper nouns]**: genererar funktionen **[!UICONTROL toSmartCase]** JavaScript, som ändrar den första bokstaven i varje ord till versaler.
* **[!UICONTROL Greetings]**: infogar hälsningar med mottagarens fullständiga namn följt av ett komma. Exempel:&quot;Hello John Doe,&quot;.
* **[!UICONTROL Insert Logo]**: infogar en logotyp som är definierad i instansinställningarna.
* **[!UICONTROL Link to mirror page]**: infogar en länk till [spegelsidan](../email/mirror-page.md). Standardformatet är:&quot;Om du inte kan visa det här meddelandet korrekt klickar du här&quot;.
* **[!UICONTROL Mirror page URL]**: infogar spegelsidans URL, vilket gör att leveransdesigners kan kontrollera länken.
* **[!UICONTROL Notification style]**
* **[!UICONTROL Offer acceptance URL in unitary mode]**: infogar en URL som gör att ett erbjudande kan anges till **[!UICONTROL Accepted]**. (Det här blocket är tillgängligt om interaktionsmodulen är aktiverad)
* **[!UICONTROL Registration confirmation]**: infogar en länk som bekräftar prenumerationen.
* **[!UICONTROL Registration link]**: infogar en prenumerationslänk. Den här länken definieras i instansinställningarna. Standardinnehållet är:&quot;Klicka här om du vill registrera dig.&quot;
* **[!UICONTROL Registration link (with referrer)]**: infogar en prenumerationslänk som gör det möjligt att identifiera besökaren och leveransen. Den här länken definieras i instansinställningarna.
* **[!UICONTROL Registration page URL]**: infogar en prenumerations-URL
* Delningslänkar för sociala nätverk
* **[!UICONTROL Style of content emails]** och **[!UICONTROL Notification style]**: generera kod som formaterar ett e-postmeddelande med fördefinierade HTML-format.
* **[!UICONTROL Unsubscription link]**: infogar en länk som gör det möjligt att avbryta prenumerationen på alla leveranser (blockeringslista). Standardinnehållet är:&quot;Du får det här meddelandet eftersom du har varit i kontakt med ***ditt organisationsnamn*** eller ett dotterbolag. Klicka här om du inte längre vill få meddelanden från ***din organisation***.&quot;

>[!NOTE]
>
>Du kan definiera nya block från Adobe Campaign v8-konsolen som gör att du kan optimera din leveranspersonalisering. Läs mer i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}.
