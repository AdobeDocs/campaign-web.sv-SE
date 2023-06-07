---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
source-git-commit: 573f0bbf396f795029c5e34b436521cb1c7b80a5
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Inbyggda innehållsblock {#ootb-content-blocks}

Inbyggda innehållsblock är:

* **[!UICONTROL Enabled by Adobe Campaign]**: infogar logotypen&quot;Enabled by Adobe Campaign&quot;.
* **[!UICONTROL Formatting function for proper nouns]**: genererar **[!UICONTROL toSmartCase]** Javascript-funktionen, som ändrar den första bokstaven i varje ord till versaler.
* **[!UICONTROL Greetings]**: infogar hälsningar med mottagarens fullständiga namn följt av ett kommatecken. Exempel: &quot;Hej John Doe.&quot;
* **[!UICONTROL Insert logo]**: infogar en logotyp som är definierad i instansinställningarna.
* **[!UICONTROL Link to mirror page]**: infogar en länk till [spegelsida](../content/mirror-page.md). Standardformatet är: &quot;Om du inte kan visa det här meddelandet korrekt klickar du här&quot;.
* **[!UICONTROL Mirror page URL]**: infogar spegelsidans URL, vilket gör att leveransdesigners kan kontrollera länken.
* **[!UICONTROL Offer acceptance URL in unitary mode]**: infogar en URL som gör att ett erbjudande kan anges till **[!UICONTROL Accepted]**. (Det här blocket är tillgängligt om interaktionsmodulen är aktiverad)
* **[!UICONTROL Registration confirmation]**: infogar en länk som bekräftar prenumerationen.
* **[!UICONTROL Registration link]**: infogar en prenumerationslänk. Den här länken definieras i instansinställningarna. Standardinnehållet är: &quot;Registrera dig genom att klicka här.&quot;
* **[!UICONTROL Registration link (with referrer)]**: infogar en prenumerationslänk som gör det möjligt att identifiera besökaren och leveransen. Den här länken definieras i instansinställningarna.
* **[!UICONTROL Registration page URL]**: infogar en prenumerations-URL
* **[!UICONTROL Style of content emails]** och **[!UICONTROL Notification style]**: generera kod som formaterar ett e-postmeddelande med fördefinierade HTML-format.
* **[!UICONTROL Unsubscription link]**: infogar en länk som gör det möjligt att avbryta prenumerationen på alla leveranser (blockeringslista). Standardinnehållet är: &quot;Du får det här meddelandet eftersom du har haft kontakt med ***ditt organisationsnamn*** eller ett närstående bolag. Ta inte längre emot meddelanden från ***ditt organisationsnamn*** klicka här.&quot;
